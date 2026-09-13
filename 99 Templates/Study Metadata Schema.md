# Study Metadata Schema

Canonical YAML frontmatter schema for study extraction notes in `07 Data/`. This documents the fields applied to the first 12 priority notes (see [[06 Synthesis/Study Dashboard]]) and is the field plan for a future Modal Forms form — no form is built yet, this is the specification a form would be built against.

Rules that apply to every field:

- Booleans are `true`/`false` only — never a string, never a third state. If the answer is genuinely unclear, use `null` instead of a boolean.
- Numeric fields contain numbers only. A single reported value is a plain number (`2.5`). A tested range is a two-element list of `[min, max]` (`[0.5, 4]`). A discrete list only where the source itself enumerates fixed variants (`fiber_diameter_um: [200, 400]` for two named fiber sizes).
- `null` means not reported / not applicable / unknown. Never infer or estimate a value to fill a field — this mirrors the vault-wide rule that `UNKNOWN` is preserved, not guessed.
- Never infer `measured_power_w` from `set_power_w`, and never infer `speed_mm_s` from procedure duration ÷ distance unless the source itself states the speed as a value (see AGENTS.md).

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
| `measured_power` | boolean | `true` / `false` | `true` only if the source reports an independently instrument-verified output value distinct from the set/console value. A per-incision QC check that is never itself tabulated as a number is recorded as `false` (see `needs_verification`). |
| `measured_power_w` | number or list or `null` | e.g. `[0.5, 4.5]` | The independently measured value itself. `null` whenever `measured_power` is `false`. |
| `power_meter` | string or `null` | free text | Instrument/brand used for power verification, if named. |
| `measurement_location` | string or `null` | free text | Where the measurement was taken (e.g. "distal end of fiber", "fiber outflow"). `null` if not stated or if the meter was used only to set (not verify) power. |
| `incision_speed_reported` | boolean | `true` / `false` | `true` only if the source itself states a numeric incision/cutting speed (mm/s). Never derived by this vault from incision length ÷ procedure time. |
| `speed_mm_s` | number or `null` | e.g. `2` | The reported speed value. `null` whenever `incision_speed_reported` is `false`. |
| `speed_control` | string (controlled) | `mechanized`, `clinician-controlled`, `measured`, `descriptive`, `unknown` | How the speed value was produced: `mechanized` = driven by a programmed/motorized device; `clinician-controlled` = a fixed manual target executed by an operator; `measured` = independently timed/instrumented verification; `descriptive` = qualitative only; `unknown` = not stated. |
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
