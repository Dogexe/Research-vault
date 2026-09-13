---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 810
set_power_w: null
measured_power: true
measured_power_value_reported: true
measured_power_w: [0.5, 4.5]
power_meter: "wattmeter (brand unspecified)"
measurement_location: "fiber outflow"
incision_speed_reported: true
speed_mm_s: 10
speed_control: mechanized
cw_pw: "CW+PW"
fiber_diameter_um: [200, 400]
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: SUPPORTING evidence — ex vivo incision-characterization study, not an oral-biopsy diagnostic-quality study.** This source makes standardized incisions in healthy (non-lesional) pig mandible mucosa to characterize incision geometry and collateral thermal damage across 33 parameter combinations; no lesion is excised and no histopathologic diagnosis is rendered. It is included in [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] for its power/mode/thermal-damage and incision-speed data, not as a diagnostic-yield source.

**Notable: this is the first source processed in this vault's biopsy-related literature that reports genuinely [[03 Concepts/Glossary/Measured Power|measured]]/delivered power, not a [[03 Concepts/Glossary/Set Power|set]]/console value.** The authors explicitly state the reported wattages were measured at the [[03 Concepts/Glossary/Measurement Location|fiber outflow]] with a [[03 Concepts/Glossary/Power Meter|wattmeter]] and do *not* correspond to the panel/instrument display. Per vault rule, this measured value is recorded as measured output; the panel/set value is UNKNOWN because the source does not report it.

## Source

- Citation: Goharkhay K, Moritz A, Wilder-Smith P, Schoop U, Kluger W, Jakolitsch S, Sperr W. "Effects on Oral Soft Tissue Produced by a Diode Laser In Vitro." *Lasers Surg Med.* 1999;25(5):401-406. DOI: [10.1002/(SICI)1096-9101(1999)25:5<401::AID-LSM6>3.0.CO;2-U](https://doi.org/10.1002/(SICI)1096-9101(1999)25:5%3C401::AID-LSM6%3E3.0.CO;2-U)
- Literature note: [[02 Literature/10.1002/(SICI)1096-9101(1999)25_5_401__AID-LSM6_3.0.CO;2-U]]
- Source type: Ex vivo bench study (standardized incisions, pig mandible mucosa), not a diagnostic-biopsy pathway
- Source locator: Full text (Introduction; Materials and Methods; Results; Tables 1–2; Discussion), retrieved from the attached PDF via the local Zotero library.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Dentek LD 15 diode laser (Dentek Austria GMBH, Gaisfeld, Austria) | — | Materials and Methods | FACT |
| Manufacturer | Dentek Austria GMBH | — | Materials and Methods | FACT |
| Wavelength | 810 | nm | Materials and Methods | FACT |
| Set/panel power | UNKNOWN — explicitly stated by the source NOT to correspond to the reported (measured) output values; the panel display value itself is never given | — | Materials and Methods | UNKNOWN (by the source's own design) |
| Measured output power | 0.5–4.5 (400 μm tip, all three modes); 0.5–2 (200 μm tip, all three modes) — measured directly at the fiber outflow with a wattmeter | W | Materials and Methods; Tables 1–2 | FACT |
| Average power | Same as measured output power above; the source's own table column header is "Average power," describing the measured wattmeter value used per condition | W | Tables 1–2 | FACT |
| Peak power | UNKNOWN — not reported separately from average power for the pulsed settings | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW), and two pulsed modes: 25 Hz/30 msec pulse width, and 50 Hz/10 msec pulse width | — | Materials and Methods | FACT |
| Pulse duration | 30 msec (25 Hz mode); 10 msec (50 Hz mode); device capability range 2–32 msec | msec | Materials and Methods | FACT |
| Frequency | 25 Hz or 50 Hz used in this study; device capability range 1.5–250 Hz | Hz | Materials and Methods | FACT |
| Duty cycle | 75% (25 Hz × 30 msec); 50% (50 Hz × 10 msec) | % | Computed in this vault from the source's own reported frequency and pulse width (25 Hz × 0.030 s = 0.75; 50 Hz × 0.010 s = 0.50) | INTERPRETATION (arithmetic derivation of two reported FACTs, not itself stated by the source) |
| Fiber diameter / tip | 200 μm and 400 μm (two tips tested; 200 μm tip limited to a 2 W maximum measured output) | μm | Materials and Methods | FACT |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact / non-contact mode | UNKNOWN — not explicitly stated | — | — | UNKNOWN |
| Incision speed | 10 | mm/second | Materials and Methods (handpiece attached to a motorized device, timed with a stopwatch) | FACT |
| Excision/incision protocol | Standardized 3 cm incisions in oral mucosa parallel to the mandible border; 6 incisions per parameter combination (3 at 5 mm below gingival margin, 3 at 5 mm from the lower mandible border); 198 total incisions across 33 parameter combinations | — | Materials and Methods | FACT |
| Tissue model | Ex vivo, 17 fresh pig mandibles (used ≤6 h post-mortem); average soft-tissue thickness 0.8–2 mm; no lesion present — healthy mucosa only | — | Materials and Methods | FACT |
| Specimen size | Not applicable — this is an incision-geometry study, not a diagnostic-biopsy specimen-size study | — | — | N/A |
| Measurement method | Histologic sections (6 μm, Serius red stain); incision depth/width and vertical/horizontal collateral damage measured per slide (15 slides per parameter/incision-site combination) | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN [[03 Concepts/Glossary/Calibration\|calibration]] for the wattmeter itself (brand/protocol not stated beyond "measured directly... with a wattmeter") | — | — | UNKNOWN |
| Incision depth, CW, 400 μm tip | Range 217.5–647.5 (across 0.5–4.5 W) | μm | Table 1 | FACT |
| Incision depth, CW, 200 μm tip | Range 405–605 (across 0.5–2 W) | μm | Table 2 | FACT |
| Vertical thermal damage (all modes/tips pooled) | Range 22.5–85.3 | μm | Results; Tables 1–2 | FACT |
| Horizontal thermal damage (all modes/tips pooled) | Range 28.3–98 | μm | Results; Tables 1–2 | FACT |
| Bone charring (underlying incisions) | None visible to the naked eye at any tested power (0.5–4.5 W), either mode, either soft-tissue thickness (0.8–2 mm) | — | Results | FACT |
| Diagnostic yield | Not applicable — no lesion excised, no diagnosis rendered | — | — | N/A |
| Coagulation zone | Not scored; described only qualitatively ("excellent coagulation ability") as a general property of the diode laser, not a measured finding of this study | — | Discussion | FACT (qualitative claim only) |
| Carbonization | Not scored on soft tissue; only bone charring (binary, visible/not visible to the naked eye) was assessed | — | Materials and Methods; Results | FACT |
| Sample | 198 incisions from 17 pig mandibles; 33 parameter combinations (7 average-power levels × up to 3 modes × 2 tips, with the 200 μm tip capped at 2 W); 15 histologic slides measured per parameter/site combination | — | Materials and Methods | FACT |

## Notes

- FACT: [[03 Concepts/Glossary/Incision Depth|Incision depth]] and width correlated strongly and positively with average (measured) power in both CW and pulsed modes, for both tips — a clean, source-confirmed dose-response for incision geometry.
- FACT, directly relevant to this vault's power-vs-thermal-damage question: **the source's own stated result is that vertical and horizontal collateral [[03 Concepts/Glossary/Thermal Damage|thermal-damage zone]] width depended on neither average power (0.5–4.5 W), nor operating mode ([[03 Concepts/Glossary/Continuous Wave|CW]] vs. either [[03 Concepts/Glossary/Pulsed Mode|pulsed]] setting), nor fiber tip diameter** — "The horizontal and vertical damage zone depends neither on the average power, nor on the mode used or fiber tip" (Discussion). This is a clean, single-source, multi-level (7 power levels × 3 modes × 2 tips) test finding **no dependence of thermal-damage-zone width on power or mode**, corroborating (in direction, not magnitude or tissue type) [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]]'s non-significant pooled power-level finding, and directly at odds with the "higher power → more damage" pattern suggested informally by [[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters|Gutiérrez-Corrales et al. 2020]] and [[07 Data/Azevedo et al 2016 - Diode Laser Thermal Damage and Carbonization Data|Azevedo et al. 2016]]'s within-device Boost-setting gradient.
- FACT, directly relevant to CW vs. PW: at every one of the 7 matched average-power levels tested with the 400 μm tip, the source reports vertical and horizontal damage values for CW and both pulsed settings side by side (Table 1); no consistent direction (CW higher, or pulsed higher) is apparent across the 7 power levels — this is a **third, independent, ex vivo pattern**: not "PW < CW" (as in [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]] and [[07 Data/Romanos et al 2022 - Initiated vs Non-Initiated Diode Laser Penetration Depth|Romanos et al. 2022]]), nor "PW > CW, non-significant" (as in Pergolini et al. 2025), but **no detectable mode-dependence at all**, at any power level from 0.5–4.5 W. This deepens rather than resolves the vault's existing CW-vs-PW conflict — it is a third distinct pattern, not a tiebreaker.
- FACT: This is the first source in this vault's biopsy-adjacent literature to report a numeric [[03 Concepts/Glossary/Incision Speed|incision speed]] (10 mm/second), and the first to report genuinely measured (wattmeter-verified) output power rather than a set/console value.
- INTERPRETATION (source's own): the lack of a clear power/mode effect on collateral damage, contrasted with a clear power effect on incision depth, is attributed by the authors to the diode laser's "chopped operating mode" behavior and to hemoglobin absorption giving strong coagulation without proportionally increasing lateral thermal spread — this is the source's own explanation, not independently re-derived here.
- HYPOTHESIS: UNKNOWN — no formal hypothesis beyond the study's own stated aim.
- Limitations (source-stated and vault-noted): ex vivo pig mandible tissue, not human oral mucosa and not a lesion; no diagnostic outcome is measured at all, so this source cannot contribute to the diagnostic-yield or margin-readability questions in [[04 Evidence/Biopsy Specimen Quality]]; tip-initiation status and contact/non-contact mode are not reported; wattmeter calibration protocol is not described beyond "measured directly... with a wattmeter."
- Classification for this vault: supporting, non-diagnostic ex vivo evidence for the power/mode → thermal-damage-width relationship, for incision speed, and for the distinction between set and measured power. Relevant to [[04 Evidence/Power Output and Tissue Effect]], [[04 Evidence/Thermal Artifact]], and [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]].
- METADATA CONVENTION: `speed_control: mechanized` — the source describes both a motorized generation mechanism (handpiece attached to a motorized device) and an independent verification detail (timed with a stopwatch). Per schema precedence, the field records how motion was generated; the stopwatch-verification detail is preserved here in prose rather than promoted to a separate value (see [[99 Templates/Study Metadata Schema]]).
