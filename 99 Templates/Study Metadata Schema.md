# Study Metadata Schema

Canonical YAML frontmatter schema for study extraction notes in `07 Data/`. This documents the fields applied to the first 12 priority notes (see [[06 Synthesis/Study Dashboard]]) and is the field plan for a future Modal Forms form — no form is built yet, this is the specification a form would be built against.

Rules that apply to every field:

- Booleans are `true`/`false` only — never a string, never a third state. If the answer is genuinely unclear, use `null` instead of a boolean.
- Numeric fields contain numbers only. A single reported value is a plain number (`2.5`). A tested range is a two-element list of `[min, max]` (`[0.5, 4]`). A discrete list only where the source itself enumerates fixed variants (`fiber_diameter_um: [200, 400]` for two named fiber sizes).
- `null` means not reported / not applicable / unknown. Never infer or estimate a value to fill a field — this mirrors the vault-wide rule that `UNKNOWN` is preserved, not guessed.
- Never infer `measured_power_w` from `set_power_w`, and never infer `speed_mm_s` from procedure duration ÷ distance unless the source itself states the speed as a value (see AGENTS.md).
- Never infer a numerical measured-power value from a tolerance/deviation threshold (e.g. "±5% deviation triggers fiber-tip replacement"), a set/console value, or a manufacturer specification. A threshold or QC gate is evidence that measurement occurred, not evidence of what the measured number was.

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
| `measured_power` | boolean or `null` | `true` / `false` / `null` | Whether output was independently measured at all (e.g. a calibrated power meter checked delivered output), regardless of whether a distinct numerical value was tabulated. `null` only if the source text is genuinely ambiguous on whether measurement occurred. |
| `measured_power_value_reported` | boolean or `null` | `true` / `false` / `null` | Whether the source reports the actual numerical measured-output value (not just that measurement occurred). `false` when independent measurement is confirmed but only a QC pass/fail or deviation threshold is given, with no distinct wattage tabulated. See the worked comparison below. |
| `measured_power_w` | number or list or `null` | e.g. `[0.5, 4.5]` | The explicit measured value itself, in watts. Populated only when `measured_power_value_reported` is `true`; otherwise `null`. |
| `power_meter` | string or `null` | free text | Instrument/brand used for power verification, if named. |
| `measurement_location` | string or `null` | free text | Where the measurement was taken (e.g. "distal end of fiber", "fiber outflow"). `null` if not stated or if the meter was used only to set (not verify) power. |
| `incision_speed_reported` | boolean | `true` / `false` | `true` only if the source itself states a numeric incision/cutting speed (mm/s). Never derived by this vault from incision length ÷ procedure time. |
| `speed_mm_s` | number or `null` | e.g. `2` | The reported speed value. `null` whenever `incision_speed_reported` is `false`. |
| `speed_control` | string (controlled) | `mechanized`, `clinician-controlled`, `measured`, `descriptive`, `unknown` | How the speed value was produced: `mechanized` = driven by a programmed/motorized device (explicitly described as such); `clinician-controlled` = the source explicitly states a manual operator executed/held the target speed; `measured` = independently timed/instrumented verification; `descriptive` = qualitative only; `unknown` = not stated. **Default to `unknown` whenever a numeric speed is reported but the source does not explicitly describe the control/verification mechanism.** A reported numeric speed alone is never sufficient to infer `mechanized` or `clinician-controlled` — e.g. Al-Ani et al. 2023/2024 report 0.75 mm/s but do not describe how it was controlled or verified, so `speed_control: unknown` even though `incision_speed_reported: true`. |
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

## Modal Forms note

No script is implemented. If a Modal Forms form is built later, it should map 1:1 to the table above: dropdowns for the controlled-vocabulary fields (`classification`, `speed_control`, `cw_pw`, `tip_initiation`, `contact_mode`), toggles for the booleans, and free-text/number inputs for the rest, writing into the same frontmatter block this schema defines. Keep the field list here as the single source of truth — do not let a form definition drift from this table.
