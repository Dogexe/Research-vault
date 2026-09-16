# Study Metadata Schema

**Terminology cross-reference:** terminology normalization for extraction/synthesis prose should follow [[03 Concepts/Glossary/Glossary Index]]. That does not apply here — schema field meanings, allowed values, and boolean/null semantics are defined solely by this document, and a glossary alias must never be used to reinterpret a field's meaning or value.

**Status: v1.3, frozen pending the next rollout batch.** v1.3 adds `speed_varied` and `thermal_damage_measure`, clarifies `margin_quality`, and permits `wavelength_nm` for relevant non-diode comparator arms. `specimen_interpretability` remains distinct from `margin_quality`, `tissue_architecture`, and `diagnostic_outcome`: it captures a whole-specimen/slide readability or adequacy judgment such as a graded slide-quality score or "thermal damage unmeasurable but diagnosis still possible" finding. Do not add new fields, change controlled-vocabulary lists, or mass-tag additional `07 Data/` notes without revisiting this document first — this file is the single source of truth for the schema, and a form, script, or additional tagging pass that drifts from it is a bug, not a variant.

**v1.2 (2026-09-14, superseded by v1.3 above; history preserved):** Added `specimen_interpretability` without changing prior field meanings.

**v1.1 (2026-09-14 maintenance patch, superseded by v1.2 above; history preserved):** v1 was stress-tested on a 10-note batch (see [[06 Synthesis/Study Dashboard]] validation notes); this patch fixed the two demonstrated defects that batch surfaced — `speed_mm_s` couldn't represent a multi-point tested sweep, and Tables B/C could silently admit a non-diode or review-tier row. No fields were added and no field's meaning changed in v1.1; only `speed_mm_s`'s allowed type widened (see below) and the two Dataview queries gained filters.

Canonical YAML frontmatter schema for study extraction notes in `07 Data/`. It was first applied to a 12-note pilot batch and has since been rolled out further (23 tagged notes as of 2026-09-14 — re-verify against the repository rather than assuming this count stays fixed; see [[06 Synthesis/Study Dashboard]]) and is the field plan for a future Modal Forms form — no form is built yet, this is the specification a form would be built against.

Rules that apply to every field:

- Booleans are `true`/`false` only — never a string, never a third state. If the answer is genuinely unclear, use `null` instead of a boolean.
- Numeric fields contain numbers only. A single reported value is a plain number (`2.5`). A tested range is a two-element list of `[min, max]` (`[0.5, 4]`). A discrete list only where the source itself enumerates fixed variants (`fiber_diameter_um: [200, 400]` for two named fiber sizes).
- Never infer `measured_power_w` from `set_power_w`, and never infer `speed_mm_s` from procedure duration ÷ distance unless the source itself states the speed as a value (see AGENTS.md).
- Never infer a numerical measured-power value from a tolerance/deviation threshold (e.g. "±5% deviation triggers fiber-tip replacement"), a set/console value, or a manufacturer specification. A threshold or QC gate is evidence that measurement occurred, not evidence of what the measured number was.

### The meaning of `true` / `false` / `null`

Frontmatter is only added to a `07 Data/` note after its extraction table already exists and the source has been read in full. **`null` can therefore never mean "not checked yet," "not extracted yet," or "the agent didn't look."** Every value on a tagged note reflects an actual read of the source — `full_text` already records whether that read was full-text or abstract-only, and `needs_verification` already records when a human should re-check a specific extraction; no separate "extraction status" field is needed on top of those two.

Within that constraint, fields split into two kinds, checked differently:

- **Reporting fields** ask whether the source's text itself states or contains something: `incision_speed_reported`, `measured_power_value_reported`, `histology`, `thermal_damage`, `diagnostic_outcome`, `biopsy_oriented`. For these, silence in a fully-read source *is* the fact being recorded — if a complete Methods+Results section never states a numeric incision speed anywhere, `incision_speed_reported` is `false`, not `null`. Reserve `null` here only when the source itself is fragmentary (e.g. abstract-only — see `full_text`) or internally contradictory about whether the thing is reported.
- **State/descriptive fields** ask about the real-world procedure the source used: `contact_mode`, `tip_initiation`, `cw_pw`, and (with one vault-specific exception below) `measured_power`. A complete Methods section that fully describes the setup and simply never mentions the property (e.g. never says contact vs. non-contact) is genuine ambiguity about what actually happened, not evidence of absence — use `null`. Use `false` only when the source makes an affirmative statement ruling the property out.
- **Exception — `measured_power` specifically:** this vault treats a complete, fully-read Methods section that describes the power setup in detail without mentioning any independent verification step as sufficient for `false`, not `null` — a power-verification step is conventionally described when performed in this literature (the same convention already applied to `histology`), so its absence from a complete Methods section is treated as clearly indicating it was not done. `null` is reserved for `measured_power` only when the source is abstract-only or genuinely self-contradictory about whether verification occurred. (This is what caught the Merigo et al. 2012 correction below — the source's own Methods section explicitly states the diode arm *was* checked with a power meter, so `false` was a direct contradiction of the note's own prose, not a defensible reading of silence.)

In short: `true` = the source explicitly supports presence. `false` = the source explicitly supports absence, or (for reporting fields, and for `measured_power` specifically) a full-text read confirms the property is simply never stated. `null` = the source was read in full but is genuinely insufficient or contradictory to decide — never a stand-in for unprocessed material.

### `measured_power` vs. `measured_power_value_reported` vs. `measured_power_w`

These are three separate questions and must not be collapsed into one:

- **`measured_power`** — *Was output independently measured at all?* `true` if the source describes an independent instrument (power meter) verifying actual delivered output, regardless of whether a specific number is tabulated.
- **`measured_power_value_reported`** — *Did the source report the actual numerical measured output?* `true` only if an explicit measured wattage (or range of measured wattages) is given as a value, separate from the set/console power.
- **`measured_power_w`** — *The explicit measured value in watts, if reported.* Populated only when `measured_power_value_reported` is `true`; otherwise `null`.

| `measured_power` | `measured_power_value_reported` | `measured_power_w` | Meaning | Example |
|---|---|---|---|---|
| `true` | `false` | `null` | Independently measured (e.g. calibrated power meter checked before every incision), but no distinct numerical measured value is tabulated — only a QC pass/fail or deviation threshold. | Hanke et al. 2021, Strakas et al. 2023 |
| `true` | `true` | numeric | Independently measured, and the actual measured wattage(s) are reported as a value. | Goharkhay et al. 1999 (`measured_power_w: [0.5, 4.5]`, measured at fiber outflow) |
| `false` | `false` | `null` | No independent measurement reported — set/console power only. | Palaia et al. 2021, Gundlapalle et al. 2022 |
| `null` | `null` | `null` | Unclear / not enough information to determine whether independent measurement occurred. | (use only when the source text itself is ambiguous, not as a default) |

## Fields

| Field | Type | Allowed values | Description |
|---|---|---|---|
| `classification` | string (controlled) | `CORE BIOPSY`, `SUPPORTING TECHNICAL`, `BACKGROUND` | Vault-level role of the study. CORE BIOPSY = real diagnostic/excisional biopsy pathway. SUPPORTING TECHNICAL = controlled bench/ex vivo characterization, no diagnosis. BACKGROUND = general/contextual literature. |
| `oral_tissue` | boolean | `true` / `false` | Whether the tissue studied is oral-cavity tissue (gingiva, oral mucosa, tongue) as opposed to skin or another site. |
| `ex_vivo` | boolean | `true` / `false` | `true` for ex vivo/bench tissue, `false` for in vivo (live patient or animal) studies. |
| `human_tissue` | boolean | `true` / `false` | `true` if the tissue source is human; `false` for animal models (porcine, ovine, bovine, murine, etc.). |
| `diode_laser` | boolean | `true` / `false` | Whether a diode laser arm is present in the study (even if compared against a non-diode laser). |
| `wavelength_nm` | number or list or `null` | e.g. `445`, `[810, 980]`, `null` | Wavelength(s) of the relevant laser arm(s) represented in the extraction. For diode studies, record diode-arm wavelength(s); for comparator/non-diode records, retain the relevant study-arm wavelength(s) and keep `diode_laser: false`. |
| `set_power_w` | number or list | e.g. `2.5`, `[1, 6]` | Console/dial power setting(s) tested. A tested range is `[min, max]`. Never equated with measured output. |
| `measured_power` | boolean or `null` | `true` / `false` / `null` | Whether output was independently measured at all (e.g. a calibrated power meter checked delivered output), regardless of whether a distinct numerical value was tabulated. A complete Methods section that never mentions verification is `false` (see "The meaning of true/false/null" above); `null` is reserved for abstract-only or self-contradictory sources. |
| `measured_power_value_reported` | boolean or `null` | `true` / `false` / `null` | Whether the source reports the actual numerical measured-output value (not just that measurement occurred). `false` when independent measurement is confirmed but only a QC pass/fail or deviation threshold is given, with no distinct wattage tabulated. See the worked comparison below. |
| `measured_power_w` | number or list or `null` | e.g. `[0.5, 4.5]` | The explicit measured value itself, in watts. Populate when the reported value/range can be faithfully represented as one number or list; retain `null` when a multi-device or multi-mode source reports only table-level paired values that this scalar/list field cannot preserve without loss. |
| `power_meter` | string or `null` | free text | Instrument/brand used for power verification, if named. |
| `measurement_location` | string or `null` | free text | Where the measurement was taken (e.g. "distal end of fiber", "fiber outflow"). `null` if not stated or if the meter was used only to set (not verify) power. |
| `incision_speed_reported` | boolean | `true` / `false` | `true` only if the source itself states a numeric incision/cutting speed (mm/s). Never derived by this vault from incision length ÷ procedure time. |
| `speed_mm_s` | number, list, or `null` | e.g. `2`, `[12.5, 6.0, 3.0, 1.0, 0.0]` | The reported speed value(s). One explicitly reported speed is a plain number. A source-reported tested range uses `[min, max]`; discrete explicitly tested speed conditions use a list preserving the reported values in the order/precision the source gives them (added in v1.1 — see **Romanos et al. 2013**, a 5-point tested sweep via a programmable translation stage). `null` whenever `incision_speed_reported` is `false`, or when it is `true` but the source's values can't be faithfully captured (rare; prefer a list over dropping data). Still never derive a speed from distance ÷ time unless the source itself reports that derived speed as a value. |
| `speed_control` | string (controlled) | `mechanized`, `clinician-controlled`, `measured`, `descriptive`, `unknown` | How the speed value was produced. See the precedence rule and worked examples immediately below the table — do not pick a value from the label definitions alone without checking precedence when a source describes more than one mechanism. |
| `speed_varied` | boolean or `null` | `true` / `false` / `null` | Whether the source varies numeric incision speed as an independent experimental condition: `true` = multiple speed conditions tested; `false` = one reported speed held fixed; `null` = speed not reported or whether it varied is unclear. Never infer this from procedure duration. |
| `cw_pw` | string or `null` | `CW`, `PW`, `CW+PW`, `null` | Operating mode(s) tested for the relevant laser arm(s); `null` when not reported. |
| `fiber_diameter_um` | number or list or `null` | e.g. `320`, `[200, 400]` | Fiber core/outer diameter(s) tested. |
| `tip_initiation` | string or `null` | `initiated`, `non-initiated`, `both`, `null` | Whether the fiber tip was pre-charred/initiated before use. |
| `contact_mode` | string or `null` | `contact`, `non-contact`, `both`, `null` | Contact status of the fiber tip against tissue. |
| `histology` | boolean | `true` / `false` | Whether histologic evaluation (of any rigor — descriptive or quantified) was performed. |
| `thermal_damage` | boolean | `true` / `false` | Whether thermal damage/effect (quantified or qualitative) was reported as an outcome. |
| `thermal_damage_measure` | string or `null` | free text | Short, source-faithful description of the reported thermal-damage, coagulation, necrosis, or artifact measure, including its unit/scale where reported. `null` if no such outcome is reported. |
| `margin_quality` | string or `null` | free text | Short description of an actual specimen-margin condition or readability finding. Do not place a raw thermal-zone magnitude, carbonization score, or a margin-width recommendation derived only from thermal depth here; those belong in `thermal_damage_measure` or the extraction table. `null` if no margin-condition/readability outcome is reported. |
| `tissue_architecture` | string or `null` | free text | Short description of any statement about overall tissue-architecture preservation. `null` if not applicable or not reported. |
| `specimen_interpretability` | string or `null` | free text | Free-text reporting field describing the source's own explicit judgment, grade, score, or separate statement about overall specimen/slide readability, interpretability, or histopathologic adequacy — distinct from raw thermal-damage magnitude, an artifact-severity measurement alone, margin condition alone, tissue-architecture alone, or the binary fact that a diagnosis was rendered. Populate only when the source explicitly reports interpretability/readability/adequacy as its own outcome or conclusion, beyond `diagnostic_outcome`. `null` when no such distinct construct is reported — including when only a diagnosis count, or only thermal-damage/margin/architecture findings, are given. Added in v1.2; see examples below. |
| `diagnostic_outcome` | boolean | `true` / `false` | Whether a clinical/histopathologic diagnosis was rendered from the specimen. Expected `false` for ex vivo/bench studies — this is not a limitation, see [[06 Synthesis/Study Dashboard]] legend. |
| `biopsy_oriented` | boolean | `true` / `false` | Whether the study excises/examines a real lesion as a biopsy specimen (as opposed to a standardized incision/block on non-lesional tissue). |
| `full_text` | boolean | `true` / `false` | Whether the extraction was performed from the full text (vs. abstract-only). |
| `needs_verification` | boolean | `true` / `false` | `true` if the note itself flags an internal source discrepancy, an ambiguous boundary case (e.g. a QC-only power check that doesn't cleanly map to `measured_power`), or another reason a human should re-check the extraction against the source before relying on it. |

### `speed_control` precedence

The five values are not mutually exclusive descriptions of the same source — a single study can have both a motion-generation mechanism and a separate verification step. When more than one applies, **use the value for how the motion was generated**, and record any additional verification detail in the note's prose rather than in this field:

1. `mechanized` — motion generated by a programmed/motorized device (e.g. a computer-controlled micropositioner, or a handpiece mounted on a motorized stage), explicitly described as such. Takes priority over `measured` even when the source also reports independent timing/verification of that motion — e.g. **Goharkhay et al. 1999** uses a motorized handpiece *and* times it with a stopwatch; the field records `mechanized` (how the motion was produced), and the stopwatch detail stays in the note's extraction table, not in this field.
2. `clinician-controlled` — the source explicitly states a manual operator executed or held a target speed. Only used when the source itself describes manual execution — never inferred merely because a device isn't mentioned.
3. `measured` — the speed value was obtained by timing/instrumentation, and the source does *not* also describe a mechanized or clinician-controlled generation mechanism **for that same recorded value** (e.g. a value derived purely from an instrumented outcome measurement with no stated control method). Current example: **[[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]]** — the note's populated `speed_mm_s: 0.61` is the source's own defined outcome metric ("speed of incision," Sinc = surgical field perimeter ÷ incision time, timed with a digital chronometer), obtained purely by measurement/calculation, with no mechanized or clinician-controlled generation mechanism stated for *that value*. Isola et al. separately reports a distinct 2.5 mm/s visually-estimated operator target — a clinician-controlled quantity — but that target is **not** what populates `speed_mm_s`; it is preserved only in the note's own prose (see that note's "Notes" section), since this field holds one number and the source itself does not reconcile the two values. `measured` therefore describes the provenance of the recorded `speed_mm_s` value, not every speed-related mechanism mentioned anywhere in the source — this is the precedence rule's intended reading for a source reporting two distinct, non-reconcilable speed quantities, not a violation of rule 2's priority.
4. `descriptive` — a qualitative speed description only (e.g. "slow, steady movement"), no number.
5. `unknown` — the default whenever a numeric speed is reported but the source does not explicitly describe *any* control or verification mechanism. A reported number alone never justifies `mechanized` or `clinician-controlled` — e.g. **Al-Ani et al. 2023/2024** report 0.75 mm/s but never describe how it was controlled or verified, so both are `unknown` despite `incision_speed_reported: true`.

This audit found the single field usable for v1 as-is once this precedence order is written down; it does not need to be split into separate "generation mechanism" and "verification method" fields unless a future note has a genuine data-integrity conflict this ordering can't resolve.

### `margin_quality` and `tissue_architecture`: free text is the v1 decision, not a placeholder

Both fields stay free text for schema v1. The 12 currently tagged notes already show why a controlled vocabulary would be premature: values range from a quantified µm distance (Al-Ani et al. 2024's LTDE), to a qualitative descriptive statement with no number (Shnawa et al. 2025, Spille et al. 2026), to not applicable at all (any non-biopsy ex vivo study with no lesion or margin concept). Forcing these into fixed categories now would either lose the quantified/qualitative distinction or invent categories no second study yet confirms. Revisit only once enough additional notes are tagged that real, stable category boundaries become visible from the data itself — not before.

### `specimen_interpretability` (v1.2): examples and non-examples

Free text, same reasoning as `margin_quality`/`tissue_architecture` above — no controlled vocabulary.

Examples (source explicitly reports a distinct interpretability/readability/adequacy construct):

- **Gundlapalle et al. 2022**: pathologist-graded slide quality, 1 = good to 5 = non-diagnostic, scored separately at periphery and center.
- **Gobbo et al. 2017**: thermal damage was not measurable in some specimens, but correct histological sampling remained possible and diagnosis was not impaired.

Non-examples (stays `null` — the information belongs in a different field, or there is no distinct construct beyond `diagnostic_outcome`):

- A raw µm thermal-damage value alone → `margin_quality`.
- Incision regularity alone → `tissue_architecture`.
- An epithelial (or connective-tissue) artifact score alone → `tissue_architecture`.
- A bare "diagnosis rendered: yes" with no separate quality or adequacy commentary → `diagnostic_outcome` alone; do not duplicate the same fact here.

## Modal Forms note

No script is implemented. If a Modal Forms form is built later, it should map 1:1 to the table above: dropdowns for the controlled-vocabulary fields (`classification`, `speed_control`, `cw_pw`, `tip_initiation`, `contact_mode`), toggles for the booleans, and free-text/number inputs for the rest, writing into the same frontmatter block this schema defines. Keep the field list here as the single source of truth — do not let a form definition drift from this table.
