---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: [445, 810, 980, 1064, 1470]
set_power_w: [0.5, 2]
measured_power: true
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: "fiber tip"
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 300
tip_initiation: "non-initiated"
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

## Source

- Literature note: [[02 Literature/10.4317/medoral.23317|Gutiérrez-Corrales et al. 2020]]
- Source link: https://doi.org/10.4317/medoral.23317
- Source locator: Abstract; Material and Methods (Laser wavelengths and systems; Laser incisions); Table 1–3

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Six systems, all supplied by A.R.C. Laser GmbH (Nuremberg, Germany): FOX IV (445 nm), NuvoLas (532 nm, KTP), FOX (810 nm), FOX (980 nm), FOX (1064 nm), WOLF (1470 nm) | — | Material and Methods | FACT |
| Manufacturer | A.R.C. Laser GmbH, Nuremberg, Germany (all six systems) | — | Material and Methods | FACT |
| Wavelength | 445, 532 (KTP), 810, 980, 1064, 1470 | nm | Abstract; Material and Methods | FACT |
| Set power | 0.5, 1.0, 1.5, 2.0 (each wavelength tested across this range in 0.5 W increments) | W | Abstract; Material and Methods | FACT |
| Measured output power (independent, reported value) | UNKNOWN — the source states output power was measured at the [[03 Concepts/Glossary/Measurement Location\|fiber tip]] with a [[03 Concepts/Glossary/Power Meter\|power meter]] before each incision, but reports no numeric measured-output or deviation value; the measurement is described only as a quality-control step ("to ensure all the incisions were set with equal parameters") | — | Material and Methods (Laser incisions) | UNKNOWN (value) / FACT (that a fiber-tip measurement was performed) |
| Average power | Same as set power (CW mode; no distinct average-power field reported) | W | Material and Methods | FACT |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW), all six wavelengths | — | Material and Methods | FACT |
| Pulse duration | UNKNOWN (CW only) | — | — | UNKNOWN |
| Frequency | UNKNOWN (CW only) | — | — | UNKNOWN |
| Duty cycle | UNKNOWN (CW only) | — | — | UNKNOWN |
| Fiber diameter | 300 (bare fiber, 280 μm core diameter) | μm | Material and Methods | FACT |
| Tip type | Bare fiber, fixed in a surgical handpiece with a curved tip attachment; inclination angle fixed at 30°; fiber projection adjusted to 3 mm; fiber cleaned before each incision | — | Material and Methods | FACT |
| Tip initiation status | Non-initialized (non-initiated) bare fiber, explicitly chosen "to ensure a pure tissue interaction... without the hot effect of initialized fibres" | — | Material and Methods | FACT |
| Contact mode | UNKNOWN — not explicitly stated as contact or non-contact in the reported methods text | — | — | UNKNOWN |
| Exposure duration | UNKNOWN as a fixed time value (incisions were made as controlled cuts across the paramarginal/pocket sites; no exposure-duration figure in seconds is given in the extracted text) | — | — | UNKNOWN |
| Measurement method | Fiber cleaned and output power measured at the fiber tip with a power meter before each incision, to standardize parameters across incisions | — | Material and Methods (Laser incisions) | FACT |
| Calibration method | UNKNOWN — power meter brand/model and [[03 Concepts/Glossary/Calibration\|calibration]] protocol are not reported | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN — not quantified; the fiber-tip measurement is described only as a setup-equalization step, with no set-vs-measured numeric comparison published | — | — | UNKNOWN |
| Sample | 24 porcine mandible specimens (40×30 mm, first/second molar region); 4 images per laser×power combination; 16 images per laser wavelength (periodontal pocket and oral mucosa sites combined) | — | Material and Methods | FACT |

## Notes

- FACT: This study's primary outcome is histological tissue effect (area of tissue loss, thermal damage area, necrosis area) across six diode/KTP wavelengths and four CW power settings (0.5–2.0 W), not power-output accuracy.
- FACT: The source explicitly performed a direct fiber-tip power-meter measurement before each incision ("we measured output power at the fibre tip with a powermeter to ensure all the incisions were set with equal parameters"), but did not publish the resulting [[03 Concepts/Glossary/Measured Power|measured]] values or any set-vs-measured deviation — so this study cannot supply a quantified power-loss or deviation figure for this vault, despite performing the underlying measurement.
- FACT: The fiber was deliberately used [[03 Concepts/Glossary/Non-initiated Tip|non-initiated]] ("non-initialized bare fibre"), explicitly to isolate the laser-tissue interaction from the added thermal effect of an [[03 Concepts/Glossary/Initiated Tip|initiated]] tip — directly relevant to the vault's "initiated / non-initiated tip" parameter, and a useful contrast with Al-Ani et al. 2023's explicitly *initiated* protocol.
- INTERPRETATION: None drawn beyond the source's own reported tissue-effect findings (1470 nm showed the greatest thermal damage/necrosis in both periodontal pocket and oral mucosa; 810 nm and 1064 nm showed the least).
- HYPOTHESIS: UNKNOWN — no hypothesis regarding power-output accuracy is proposed.
- Classification for this vault: supporting/background evidence for operating parameters and tip-initiation protocol; **not** direct measured-output evidence (measurement performed but not reported numerically).
