---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: [810, 980]
set_power_w: [1.5, 2.5]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: "PINTUDY"
measurement_location: null
incision_speed_reported: true
speed_mm_s: 0.75
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 400
tip_initiation: "initiated"
contact_mode: "contact"
histology: false
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

- Literature note: [[02 Literature/10.34172/jlms.2023.37|Al-Ani et al. 2023]]
- Source link: https://doi.org/10.34172/jlms.2023.37
- Source locator: Abstract; Materials and Methods (Laser Parameters); Table 1

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Dual-wavelength diode laser: Quicklase 12W dual 4 (Quicklase, England, UK). Comparator (non-diode): Er,Cr:YSGG Waterlase iPlus (Biolase, California, USA) | — | Materials and Methods | FACT |
| Manufacturer | Quicklase (diode); Biolase (Er,Cr:YSGG comparator) | — | Materials and Methods | FACT |
| Wavelength | Diode: dual 810 nm (50%) + 980 nm (50%) simultaneously. Er,Cr:YSGG comparator: 2780 nm | nm | Abstract; Table 1 | FACT |
| Set power | Diode: 1.5 W and 2.5 W, CW. Er,Cr:YSGG comparator: 2.5 W and 3.5 W, PW (50 mJ/pulse and 70 mJ/pulse respectively) | W | Abstract; Table 1 | FACT |
| Measured output power (independent, post-set verification) | UNKNOWN — the power meter (PINTUDY) was used only to adjust the power while cutting the fiber to the target set value, not to independently verify/report a separate measured value after setup | — | Materials and Methods | UNKNOWN |
| Average power | Diode: 1.5 W and 2.5 W (CW, so average = set). Er,Cr:YSGG: 2.5 W and 3.5 W average (PW) | W | Table 1 | FACT |
| Peak power | Diode: UNKNOWN (CW mode, not reported). Er,Cr:YSGG: 71.43 W (2.5 W group), 100 W (3.5 W group) | W | Table 1 | FACT (Er,Cr:YSGG only) / UNKNOWN (diode) |
| Operating mode | Diode: continuous wave (CW). Er,Cr:YSGG comparator: pulsed wave (PW) | — | Table 1 | FACT |
| Pulse duration | Diode: UNKNOWN (CW, not applicable). Er,Cr:YSGG: 700 | μs | Table 1 | FACT (Er,Cr:YSGG) / UNKNOWN (diode) |
| Frequency | Diode: UNKNOWN (CW, not applicable). Er,Cr:YSGG: 50 | Hz | Table 1 | FACT (Er,Cr:YSGG) / UNKNOWN (diode) |
| Duty cycle | UNKNOWN for both lasers (not reported as duty cycle) | — | — | UNKNOWN |
| Fiber diameter | Diode: 400 (FC single file multimode). Er,Cr:YSGG: 600 (tip MZ6, length 6 mm) | μm | Materials and Methods; Table 1 | FACT |
| Tip type | Diode: fiber optic, initiated before each power output. Er,Cr:YSGG: tip MZ6 (diameter 600 μm, length 6 mm) | — | Materials and Methods | FACT |
| Tip initiation status | Diode: initiated — explicit protocol described: laser set to 0.5 W, fiber applied to articulating paper, activated until perforation seen and a flame/char formed, before each power output was used for incisions | — | Materials and Methods | FACT |
| Contact mode | Diode: contact mode. Er,Cr:YSGG: contact mode | — | Materials and Methods | FACT |
| Exposure duration | 20 sec per incision (15 mm incision length, 0.75 mm/s speed of movement), fixed across all groups in the main study | sec | Materials and Methods | FACT |
| Measurement method | Power meter (PINTUDY, Guangzhou, China) used to adjust/set the diode power via the fiber cut; not described as independently re-verifying output after setup | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN — power meter brand is named (PINTUDY) but no calibration protocol, certificate, or traceability is described | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN — not reported; this study measures temperature rise as its outcome, not power-output accuracy | — | — | UNKNOWN |
| Power density (calculated) | Diode: 1153.8 W/cm² (1.5 W), 1923 W/cm² (2.5 W). Er,Cr:YSGG: 892.8 W/cm² (2.5 W), 1250 W/cm² (3.5 W) | W/cm² | Table 1 | FACT |
| Water/air spray | Diode: UNKNOWN (not reported, "--" in Table 1). Er,Cr:YSGG: 10%/10% | % | Table 1 | FACT (Er,Cr:YSGG) / UNKNOWN (diode) |
| Sample | 6 freshly dissected sheep tongues; 50 total incisions (10 pilot + 40 main study); main study: 20 diode incisions (10 per power level) + 20 Er,Cr:YSGG incisions (10 per power level) | — | Materials and Methods | FACT |

## Notes

- FACT: This study's primary outcome is peri-incisional temperature rise (thermocouple measurement), not power-output accuracy. The diode laser showed a significantly greater mean temperature rise (8.06 ± 2.58 °C) than the Er,Cr:YSGG comparator (3.87 ± 1.16 °C, P < 0.001); the 2.5 W diode group had the highest rise of all four groups (10.06 ± 2.02 °C) and the 2.5 W Er,Cr:YSGG group the lowest (3.02 ± 0.57 °C).
- FACT: The diode fiber tip was explicitly *[[03 Concepts/Glossary/Initiated Tip|initiated]]* (pre-charred) before each power setting was used — a directly stated tip-initiation protocol, useful for the vault's "initiated / non-initiated tip" parameter even though this study does not measure power loss.
- FACT: The power meter (PINTUDY) served only to standardize the *[[03 Concepts/Glossary/Set Power|set]]* power via the fiber-optic cut; the study provides no independent [[03 Concepts/Glossary/Measured Power|measured-output]] value distinct from the set value, and therefore contributes no power-loss or set-vs-measured deviation data.
- HYPOTHESIS: UNKNOWN — no hypothesis regarding power accuracy is proposed; the study's hypothesis concerns comparative thermal safety between the two laser types.
- Classification for this vault: supporting/background evidence for operating parameters and tip-initiation protocol; **not** direct measured-output evidence (no power loss/deviation reported).
- METADATA CONVENTION: this vault's structured schema records `speed_control: unknown` for this study. A numeric incision speed (0.75 mm/s) is explicitly reported, but the mechanism used to control or verify that speed is not described — the source does not state whether it was mechanized, clinician-executed, or otherwise. Per schema convention, `speed_control` is not upgraded to `clinician-controlled` or `mechanized` without explicit source support (see [[99 Templates/Study Metadata Schema]]).
