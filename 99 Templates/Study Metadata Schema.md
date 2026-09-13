# Study Metadata Schema

**Status: v1, frozen for the current 12 tagged notes.** This version has been audited for internal consistency (see the validation note at the bottom of [[06 Synthesis/Study Dashboard]]) and is stable for the existing Dataview workflow. Do not add new fields, change controlled-vocabulary lists, or mass-tag additional `07 Data/` notes without revisiting this document first — this file is the single source of truth for the schema, and a form, script, or additional tagging pass that drifts from it is a bug, not a variant.

Canonical YAML frontmatter schema for study extraction notes in `07 Data/`. This documents the fields applied to the first 12 priority notes (see [[06 Synthesis/Study Dashboard]]) and is the field plan for a future Modal Forms form — no form is built yet, this is the specification a form would be built against.

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
| `wavelength_nm` | number or list | e.g. `445`, `[810, 980]` | Wavelength(s) of the diode arm only. Dual-wavelength devices use a two-element list. |
| `set_power_w` | number or list | e.g. `2.5`, `[1, 6]` | Console/dial power setting(s) tested. A tested range is `[min, max]`. Never equated with measured output. |
| `measured_power` | boolean or `null` | `true` / `false` / `null` | Whether output was independently measured at all (e.g. a calibrated power meter checked delivered output), regardless of whether a distinct numerical value was tabulated. A complete Methods section that never mentions verification is `false` (see "The meaning of true/false/null" above); `null` is reserved for abstract-only or self-contradictory sources. |
| `measured_power_value_reported` | boolean or `null` | `true` / `false` / `null` | Whether the source reports the actual numerical measured-output value (not just that measurement occurred). `false` when independent measurement is confirmed but only a QC pass/fail or deviation threshold is given, with no distinct wattage tabulated. See the worked comparison below. |
| `measured_power_w` | number or list or `null` | e.g. `[0.5, 4.5]` | The explicit measured value itself, in watts. Populated only when `measured_power_value_reported` is `true`; otherwise `null`. |
| `power_meter` | string or `null` | free text | Instrument/brand used for power verification, if named. |
| `measurement_location` | string or `null` | free text | Where the measurement was taken (e.g. "distal end of fiber", "fiber outflow"). `null` if not stated or if the meter was used only to set (not verify) power. |
| `incision_speed_reported` | boolean | `true` / `false` | `true` only if the source itself states a numeric incision/cutting speed (mm/s). Never derived by this vault from incision length ÷ procedure time. |
| `speed_mm_s` | number or `null` | e.g. `2` | The reported speed value. `null` whenever `incision_speed_reported` is `false`. |
| `speed_control` | string (controlled) | `mechanized`, `clinician-controlled`, `measured`, `descriptive`, `unknown` | How the speed value was produced. See the precedence rule and worked examples immediately below the table — do not pick a value from the label definitions alone without checking precedence when a source describes more than one mechanism. |
| `cw_pw` | string | `CW`, `PW`, `CW+PW` | Operating mode(s) tested for the diode arm. |
| `fiber_diameter_um` | number or list or `null` | e.g. `320`, `[200, 400]` | Fiber core/outer diameter(s) tested. |
| `tip_initiation` | string or `null` | `initiated`, `non-initiated`, `both`, `null` | Whether the fiber tip was pre-charred/initiated before use. |
| `contact_mode` | string or `null` | `contact`, `non-contact`, `both`, `null` | Contact status of the fiber tip against tissue. |
| `histology` | boolean | `true` / `false` | Whether histologic evaluation (of any rigor — descriptive or quantified) was performed. |
| `thermal_damage` | boolean | `true` / `false` | Whether thermal damage/effect (quantified or qualitative) was reported as an outcome. |
| `margin_quality` | string or `null` | free text | Short description of any margin-condition finding (quantified distance, or a qualitative statement). `null` if not applicable or not reported. |
| `tissue_architecture` | string or `null` | free text | Short description of any statement about overall tissue-architecture preservation. `null` if not applicable or not reported. |
| `diagnostic_outcome` | boolean | `true` / `false` | Whether a clinical/histopathologic diagnosis was rendered from the specimen. Expected `false` for ex vivo/bench studies — this is not a limitation, see [[06 Synthesis/Study Dashboard]] legend. |
| `biopsy_oriented` | boolean | `true` / `false` | Whether the study excises/examines a real lesion as a biopsy specimen (as opposed to a standardized incision/block on non-lesional tissue). |
| `full_text` | boolean | `true` / `false` | Whether the extraction was performed from the full text (vs. abstract-only). |
| `needs_verification` | boolean | `true` / `false` | `true` if the note itself flags an internal source discrepancy, an ambiguous boundary case (e.g. a QC-only power check that doesn't cleanly map to `measured_power`), or another reason a human should re-check the extraction against the source before relying on it. |

### `speed_control` precedence

The five values are not mutually exclusive descriptions of the same source — a single study can have both a motion-generation mechanism and a separate verification step. When more than one applies, **use the value for how the motion was generated**, and record any additional verification detail in the note's prose rather than in this field:

1. `mechanized` — motion generated by a programmed/motorized device (e.g. a computer-controlled micropositioner, or a handpiece mounted on a motorized stage), explicitly described as such. Takes priority over `measured` even when the source also reports independent timing/verification of that motion — e.g. **Goharkhay et al. 1999** uses a motorized handpiece *and* times it with a stopwatch; the field records `mechanized` (how the motion was produced), and the stopwatch detail stays in the note's extraction table, not in this field.
2. `clinician-controlled` — the source explicitly states a manual operator executed or held a target speed. Only used when the source itself describes manual execution — never inferred merely because a device isn't mentioned.
3. `measured` — the speed value was obtained by timing/instrumentation, and the source does *not* also describe a mechanized or clinician-controlled generation mechanism (e.g. a value derived purely from an instrumented outcome measurement with no stated control method). No currently tagged note uses this value after the Goharkhay correction above — it remains in the vocabulary for a future note that fits this narrower case.
4. `descriptive` — a qualitative speed description only (e.g. "slow, steady movement"), no number.
5. `unknown` — the default whenever a numeric speed is reported but the source does not explicitly describe *any* control or verification mechanism. A reported number alone never justifies `mechanized` or `clinician-controlled` — e.g. **Al-Ani et al. 2023/2024** report 0.75 mm/s but never describe how it was controlled or verified, so both are `unknown` despite `incision_speed_reported: true`.

This audit found the single field usable for v1 as-is once this precedence order is written down; it does not need to be split into separate "generation mechanism" and "verification method" fields unless a future note has a genuine data-integrity conflict this ordering can't resolve.

### `margin_quality` and `tissue_architecture`: free text is the v1 decision, not a placeholder

Both fields stay free text for schema v1. The 12 currently tagged notes already show why a controlled vocabulary would be premature: values range from a quantified µm distance (Al-Ani et al. 2024's LTDE), to a qualitative descriptive statement with no number (Shnawa et al. 2025, Spille et al. 2026), to not applicable at all (any non-biopsy ex vivo study with no lesion or margin concept). Forcing these into fixed categories now would either lose the quantified/qualitative distinction or invent categories no second study yet confirms. Revisit only once enough additional notes are tagged that real, stable category boundaries become visible from the data itself — not before.

## Modal Forms note

No script is implemented. If a Modal Forms form is built later, it should map 1:1 to the table above: dropdowns for the controlled-vocabulary fields (`classification`, `speed_control`, `cw_pw`, `tip_initiation`, `contact_mode`), toggles for the booleans, and free-text/number inputs for the rest, writing into the same frontmatter block this schema defines. Keep the field list here as the single source of truth — do not let a form definition drift from this table.
