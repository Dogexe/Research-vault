---
classification: SUPPORTING TECHNICAL
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 810
set_power_w: [1.0, 1.7]
measured_power: true
measured_power_value_reported: true
measured_power_w: [0.54, 0.91]
power_meter: Molectron (Coherent Inc.)
measurement_location: tip of the optical fiber
incision_speed_reported: false
speed_mm_s: null
speed_control: descriptive
speed_varied: null
cw_pw: CW
fiber_diameter_um: 400
tip_initiation: null
contact_mode: both
histology: false
thermal_damage: false
thermal_damage_measure: null
margin_quality: null
tissue_architecture: null
specimen_interpretability: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/Others/Phenomenon of laser power loss during curettage of infected periodontal pockets]]
- Zotero item: [X5DXV8RX](zotero://select/library/items/X5DXV8RX)
- Source link: https://doi.org/10.1089/pho.2010.2911
- Source locator: Full text (Abstract; Materials and Methods; Results; Tables 1–3; Discussion; Conclusions), retrieved from the Zotero attachment.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | 810 nm diode laser, Biolase (Irvine, CA) | — | Materials and Methods | FACT |
| Manufacturer | Biolase | — | Materials and Methods | FACT |
| Wavelength | 810 | nm | Abstract; Materials and Methods | FACT |
| Set power | Treatment: 1.7 W CW. Measurement standardization: 1.0 W CW at the control panel before each power-output measurement; after measurement, power was increased to 1.7 W for the next treatment application. | W | Abstract; Materials and Methods | FACT |
| Independently measured power | Power output was measured at the tip of the optical fiber with a Molectron (Coherent Inc.) power meter before each treatment application. Table 1 reports study-group means of 0.91, 0.72, 0.63, and 0.54 W for the first through fourth applications, respectively, at the 1.0 W measurement setting. These are not measured-output values at the 1.7 W treatment setting. | W | Materials and Methods; Table 1 | FACT |
| Operating mode | Continuous wave (CW) | — | Abstract; Materials and Methods | FACT |
| Fiber diameter | 400 | μm | Materials and Methods | FACT |
| Tip condition | Fiber tip freshly cleaved after every four applications; initiation status not reported. | — | Materials and Methods | FACT / UNKNOWN (initiation status) |
| Contact mode | Study group: contact. Control measurements: non-contact. | — | Materials and Methods | FACT |
| Incision speed | No numeric speed reported. The study describes rapid perpendicular and zigzag fiber movements; duration was 10–15 s per application site and is not converted here to speed. | — | Materials and Methods | FACT / UNKNOWN (numeric speed) |
| Exposure duration | 10–15 s per treatment application; four applications per tooth (40–60 s total). Controls: four measurements at 15-s intervals. | s | Abstract; Materials and Methods | FACT |
| Measurement method | Four power-output measurements per tooth (110 total; one tooth had two measurements only); control group: 28 non-contact irradiations with four measurements each (112 total). Fiber tip was cleaned before each measurement. | — | Materials and Methods | FACT |
| Power loss | Study group: 20.89%, 30.39%, and 40.26% mean loss between first and second, first and third, and first and fourth applications. Control: 0.14%, 0.54%, and 1.58% over the same comparisons. | % | Abstract; Table 2; Discussion | FACT |
| Calibration method | Laser power was standardized at 1.0 W before each measurement. Power-meter calibration details were not reported. | — | Materials and Methods | FACT / UNKNOWN (meter calibration details) |

## Notes

- FACT: This is clinical periodontal curettage, not a biopsy-specimen or histology study; it is supporting technical evidence for delivered-power change at the fiber tip.
- FACT: The source reports a 9% mean fiber-transmission loss before tissue contact and a progressive contact-associated reduction in output across applications.
- NEEDS VERIFICATION: The source also calls the fourth-application output a 54% loss from the 1.0 W panel setting, whereas Table 1 reports a mean 0.54 W remaining, which corresponds arithmetically to approximately 46% loss. Both source statements are retained without reconciliation.
- INTERPRETATION: The qualitative movement description is not a controlled or measured incision-speed value and does not establish a speed effect.
- HYPOTHESIS: UNKNOWN.

## Related notes

- Evidence: [[04 Evidence/Set Power vs Measured Output]], [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]]
- Concepts: [[03 Concepts/Glossary/Measured Power]], [[03 Concepts/Glossary/Power Loss]], [[03 Concepts/Glossary/Incision Speed]]
