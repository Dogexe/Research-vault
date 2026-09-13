---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 980
set_power_w: 2
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 300
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: "quantified (5 mm safety margin protocol; thermal alteration from margin: epithelium 288.9 um, connective tissue 430.3 um; diagnosis unimpaired in all cases)"
tissue_architecture: "quantified (epithelium and lamina propria significantly thicker than healthy control, p=0.021/0.034, but did not impair diagnosis)"
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.3390/dj14030168]]
- Source link: https://doi.org/10.3390/dj14030168
- Source locator: Full text (Materials and Methods §2.1–2.7; Results §3.1–3.6; Discussion), retrieved from the attached PDF via the local Zotero library (zotero-key 8G8RTCNF).

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Raffaello Laser by DMT, Lissone, Italy | — | §2.2 (Laser Group Protocol) | FACT |
| Manufacturer | DMT, Lissone, Italy | — | §2.2 | FACT |
| Wavelength | 980 | nm | §2.2 | FACT |
| Set power | 2 | W | §2.2 | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; set/console value only | — | — | UNKNOWN |
| Average power | UNKNOWN (CW, no distinct average-power field) | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) | — | §2.2 | FACT |
| Pulse duration | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Frequency | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Duty cycle | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Fiber diameter | 300 | μm | §2.2 | FACT |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | Contact mode | — | §2.2 | FACT |
| Exposure duration | UNKNOWN as a fixed time value; single operator performed all procedures to minimize inter-operator variability | — | §2.2 | FACT (operator control) / UNKNOWN (exposure time) |
| Excision margin | Circumferential safety margin of 5 mm from clinically healthy tissue | mm | §2.2 | FACT |
| Measurement method — histology | Thermal alteration measured in microns from the surgical margin toward histologically readable tissue by a blinded pathologist using digital analysis software on H&E-stained sections (×100 magnification); defined as the mean maximum unreadable area in epithelial and connective-tissue compartments; connective-tissue alteration characterized by basophilic changes consistent with hemocoagulative phenomena | — | §2.5 | FACT |
| Measurement method — OCT | Ex vivo spectral-domain OCT (Telesto 220, Thorlabs Inc.), 1300 nm central wavelength, 5.5 μm axial / 13 μm lateral resolution, 10×10 mm scan area, ~3.5 mm max imaging depth; peripheral (surgical margin) and central (unaffected reference) scans per specimen, spatially co-registered to histology via India-ink marking | — | §2.4 | FACT |
| Calibration method | UNKNOWN — no laser power-meter calibration protocol reported (OCT system specifications are reported; laser output calibration is not) | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Diagnostic yield | Definitive histopathological diagnosis obtained in all 30/30 cases (100%); laser-induced thermal effects did not impair diagnosis in any specimen | — | §3.4 | FACT |
| Histologic thermal damage — epithelium | Mean 288.9 | μm | §3.4 | FACT |
| Histologic thermal damage — connective tissue | Mean 430.3 | μm | §3.4 | FACT |
| OCT-measured epithelial remodeling | 0.028 ± 0.05 | mm | §3.4 | FACT |
| OCT-measured connective-tissue remodeling | 0.040 ± 0.05 | mm | §3.4 | FACT |
| OCT–histology overall concordance | 88.5%; ICC 0.88 (95% CI 0.81–0.93); no significant difference by Wilcoxon signed-rank test for epithelium (p=0.42) or lamina propria (p=0.36) | — | §3.4–3.5 | FACT |
| Epithelium thickness — laser group vs. healthy control | Laser: 0.414 ± 0.163 mm (median 0.40, range 0.21–0.80); Control: 0.276 ± 0.050 mm (median 0.27, range 0.19–0.36); Mann-Whitney U p=0.021 (significant) | mm | Table 4 | FACT |
| Lamina propria thickness — laser group vs. healthy control | Laser: 0.507 ± 0.416 mm (median 0.40, range 0.18–1.50); Control: 0.443 ± 0.089 mm (median 0.44, range 0.28–0.55); Mann-Whitney U p=0.034 (significant) | mm | Table 4 | FACT |
| Sample | 30 patients with OL without epithelial dysplasia (17M/13F, mean age 49.35 y), max lesion diameter ≤1.5 cm; 15 lesions excised by diode laser (laser group), 15 removed by scalpel (control group, peri-lesional normal mucosa ~3 mm from lesion margin) | — | §2.1; §3.1 | FACT |

## Notes

- FACT: This is the vault's second source with a real pathologist-rendered [[03 Concepts/Glossary/Diagnostic Quality|diagnostic]]-yield outcome (after Romeo et al. 2014), and — unlike Romeo et al. and Angiero et al. — it directly quantifies histologic [[03 Concepts/Glossary/Thermal Damage|thermal-damage]] width (epithelium 288.9 μm, connective tissue 430.3 μm) *and* diagnostic outcome (100% success) in the same human specimen set, at a fixed, standardized 5 mm margin. This is the closest match in this vault to the kind of study design identified as a research gap (thermal-artifact measurement + diagnostic outcome, same specimens) — though it still does not vary power/operating parameters as an independent variable, and does not independently verify delivered power.
- FACT: Despite 100% diagnostic success, laser-treated tissue showed statistically significantly greater epithelium and lamina propria thickness than healthy control tissue (p=0.021, p=0.034) — i.e., a real, measurable, statistically significant [[03 Concepts/Glossary/Tissue Architecture Preservation|tissue-architecture]] alteration was present, but it did not rise to the level of impairing diagnosis. This nuance is preserved rather than collapsed into a simple "no effect" reading.
- FACT: The excision margin (5 mm) matches Angiero et al.'s recommended minimum in vivo specimen diameter (≥5 mm) — an independent, if indirect, cross-study consistency point, since this study was designed around (not testing) that margin.
- FACT: The source's own Discussion cites, as background (not as its own finding), that "studies indicate that when excision includes at least 3–5 mm of surrounding healthy tissue, carbonization does not impair diagnostic evaluation" (Introduction, citing refs 12–13) — consistent with, but not independent confirmation of, the Angiero et al. and Romeo et al. size/margin findings already in this vault.
- HYPOTHESIS: UNKNOWN.
- Limitations (source's own, stated in Discussion): modest sample size; ex vivo OCT imaging only (in vivo application not tested); single-center; power/operating parameters were fixed, not varied.
- Classification for this vault: direct dental-diode biopsy diagnostic-yield, thermal-damage, and specimen-margin evidence. Relevant to [[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Thermal Artifact]], and [[04 Evidence/Surgical Margins]].
