---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: [450, 808]
set_power_w: [2, 4]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW+PW"
fiber_diameter_um: 300
tip_initiation: "initiated"
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.3390/dj13060265]]
- Source link: https://doi.org/10.3390/dj13060265
- Source locator: Full text (Introduction; Materials and Methods; Results §3; Discussion §4; Conclusions §5; Tables 1–7), retrieved from the attached PDF's cached plaintext via the local Zotero library (zotero-key CEUD69R9).

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Wiser 3 (Doctor Smile, Brendola (VI), Italy) — dual-wavelength diode laser | — | Materials and Methods | FACT |
| Manufacturer | Doctor Smile, Brendola (VI), Italy | — | Materials and Methods | FACT |
| Wavelength | Dual-wavelength: 450 and 808 (combined in one handpiece/emission) | nm | Materials and Methods | FACT |
| Set power | 2, 3, 4 (three levels, each tested in both CW and PW) | W | Materials and Methods | FACT |
| Measured output power | UNKNOWN — described as "adjusted output power of the laser device," a console/set value; no independent power-meter verification reported | — | — | UNKNOWN |
| Average power | UNKNOWN (the 2/3/4 W values are themselves described as "average powers" per the Abstract, but no independently measured average distinct from the set value is reported) | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) and pulsed wave (PW), each tested at all three power levels (six groups total) | — | Materials and Methods | FACT |
| Pulse duration | UNKNOWN (Introduction states the device class supports "pulse duration ranging from 0.1 ms to infinity," as general background, not this study's specific PW setting) | — | Introduction (background only) | UNKNOWN (study-specific value) |
| Frequency | 10 | kHz | Materials and Methods | FACT |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | 300 | μm | Materials and Methods | FACT |
| Tip type | Initiated surgical tip; tip length 5 mm; checked during excision for carbonized build-up to prevent additional collateral thermal damage | — | Materials and Methods | FACT |
| Tip initiation status | Initiated | — | Materials and Methods | FACT |
| Contact mode | Contact mode | — | Materials and Methods | FACT |
| Exposure duration | UNKNOWN as a per-incision time value; total energy of 579.8 J stated for the protocol (ambiguous in the retrieved text whether this is per-sample or per-group total; preserved as reported, not resolved) | J | Materials and Methods | FACT (energy value) / UNKNOWN (per-incision exposure time; energy-value scope) |
| Excision protocol | Ex vivo excisions on porcine lingual mucosa; six groups of six samples each (2/3/4 W × CW/PW); single-pass excisions | — | Materials and Methods | FACT |
| Specimen size | UNKNOWN — no specimen diameter/size value reported; this is an ex vivo tissue-damage study, not a diagnostic-biopsy specimen-size study | — | — | UNKNOWN |
| Measurement method | Epithelial and connective-tissue thermal damage measured in mm on H&E-stained sections at 2.5× magnification using LAS 4.8 software; pathologist blinded to laser parameters | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN — no laser power-meter calibration protocol reported | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Diagnostic yield | Not applicable — ex vivo tissue-damage study; no diagnosis rendered. In 2/36 samples, epithelial damage could not be quantified due to severe epithelial destruction. | — | Results | FACT |
| Epithelial damage, minimum | 0.62 (2 W CW) | mm | Results | FACT |
| Epithelial damage, maximum | 3.12 (4 W PW) | mm | Results | FACT |
| Connective tissue damage, minimum | 0.53 (4 W CW) | mm | Results | FACT |
| Connective tissue damage, maximum | 3.19 (4 W PW) | mm | Results | FACT |
| Total epithelial damage (all groups) | Mean 1.33 ± 0.56 | mm | Table 1 | FACT |
| Total connective tissue damage (all groups) | Mean 1.57 ± 0.61 | mm | Table 1 | FACT |
| Epithelial damage — CW vs. PW (pooled across power) | CW: 1.22 ± 0.45; PW: 1.45 ± 0.64; t=−1.21, p=0.234 (not statistically significant) | mm | Table 1; Table 6 | FACT |
| Connective tissue damage — CW vs. PW (pooled across power) | CW: 1.49 ± 0.46; PW: 1.65 ± 0.73; t=0.77, p=0.444 (not statistically significant) | mm | Table 1; Table 6 | FACT |
| Epithelial damage by power (pooled across mode) | 2W: 1.35 ± 0.48; 3W: 1.41 ± 0.45; 4W: 1.21 ± 0.74; F(2,33)=0.271, p=0.765 (not statistically significant) | mm | Table 7 | FACT |
| Connective tissue damage by power (pooled across mode) | 2W: 1.55 ± 0.44; 3W: 1.46 ± 0.42; 4W: 1.70 ± 0.88; F(2,33)=0.434, p=0.652 (not statistically significant) | mm | Table 7 | FACT |
| Group B (2W PW) vs. Group A (2W CW), epithelial damage | Reported as "statistically significant correlation" in text with stated value "t = 1.94, p < 0.01"; however, Table 2's own reported p-value for this exact comparison is p = 0.084, not p < 0.01. Both figures are preserved verbatim from the source; the discrepancy is NOT resolved by this vault. NEEDS VERIFICATION. | — | Results; Table 2 | FACT (as reported) — internal inconsistency flagged |
| Significance threshold used by source | p ≤ 0.10 (explicitly stated in Methods, non-standard/looser than the conventional 0.05) | — | Materials and Methods | FACT |
| Recommended perilesional margin | At least 2 mm in both CW and PW, "especially in excisional biopsies of lesions suspected of malignancy"; 2 W CW identified as showing the least thermal damage | mm | Conclusions | FACT |
| Carbonization | Listed among observed histologic artifacts; not scored numerically or isolated as its own measured variable | — | Results | FACT (qualitative) |
| Coagulation zone | Not scored or measured as an isolated variable in this source | — | — | UNKNOWN |
| Histologic artifacts reported | Epithelial detachment, loss of epithelial/subepithelial cellular adhesion, epithelial erosion, epithelial spongiosis, carbonization, vacuolization | — | Results | FACT |
| Sample | 36 porcine lingual mucosa samples from 6 tongues (deceased <24 h); 6 groups of 6 (2/3/4 W × CW/PW) | — | Materials and Methods | FACT |

## Notes

- FACT: This is the vault's first source to vary power (2/3/4 W) and mode ([[03 Concepts/Glossary/Continuous Wave|CW]]/[[03 Concepts/Glossary/Pulsed Mode|PW]]) as two independent variables in a single fully crossed design (six groups) for a dual-wavelength dental diode laser, measuring both epithelial and connective-tissue [[03 Concepts/Glossary/Thermal Damage|thermal damage]] separately. None of the pooled comparisons (mode alone, power alone) reached statistical significance at the source's own stated threshold (p ≤ 0.10) except the single Group A vs. Group B comparison noted below.
- FACT — preserved internal source inconsistency: the source's own narrative text states the comparison between Group A (2W CW) and Group B (2W PW) for epithelial damage was significant with "t = 1.94, p < 0.01," but the source's own Table 2 lists p = 0.084 for that identical comparison — 0.084 is not < 0.01, though it does fall within the source's stated significance threshold of p ≤ 0.10. This vault does not resolve or correct this discrepancy; both figures are recorded as the source reports them. NEEDS VERIFICATION.
- FACT: Despite testing three power levels (2/3/4 W) with a fully crossed design, the pooled by-power comparison (disregarding mode) found no statistically significant difference in either epithelial (p=0.765) or connective-tissue (p=0.652) damage — i.e., within this source's own data, power level alone did not have a demonstrated (statistically significant) effect on thermal-damage extent, even though the raw minimum/maximum values do increase with power (0.62 mm at 2W CW up to 3.12–3.19 mm at 4W PW).
- FACT: The source's own Conclusions nonetheless recommend the lowest tested power (2 W CW) based on it showing the least average thermal damage, and recommend a ≥2 mm perilesional margin for excisional biopsies of lesions suspected of malignancy — a smaller recommended margin than the ≥5 mm figures reported by Angiero et al., Gambino et al., and Gundlapalle et al. already in this vault. This is a genuine cross-source difference in recommended margin, not resolved here (see Conflicting findings in the synthesis). [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]] [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data]] [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data]]
- FACT: The source's own Discussion cites a different in vivo study (Palaia et al., ref. 14, 445 nm diode, 12 patients) as showing *greater* thermal effects than this ex vivo study, attributed to reduced tissue vascularization in the deceased-porcine ex vivo model — this is the source's own cited comparison, not independent vault verification of Palaia et al., which is not itself a processed source in this vault.
- FACT: The source's own Discussion also cites Gundlapalle et al. 2022 (ref. 1, this vault's other newly processed source), Al-Ani et al. 2024 (ref. 13, a different Al-Ani study than the 2023 dual-wavelength source already in this vault — not to be conflated), and cites recommended margin additions of "1 mm in CW and 0.7 mm in PW" from Monteiro et al. (ref. 22) as background, not as this study's own finding.
- INTERPRETATION (source's own): greater connective-tissue than epithelial damage at higher power (notably 4 W) is attributed to the two wavelengths' (445/808 nm) affinity for hemoglobin/melanin, chromophores concentrated in connective tissue, allowing deeper laser penetration.
- HYPOTHESIS (source's own, explicitly labeled tentative given non-significant results): PW mode may cause greater thermal damage than CW because achieving full excision in PW requires repeated tip application at the same site, though the source states this cannot be asserted with certainty given the lack of significant results at 3 W and 4 W.
- Classification for this vault: direct dual-wavelength dental-diode power×mode thermal-damage evidence — ex vivo, not a diagnostic-biopsy outcome (no diagnosis rendered), set/console power only, no calibration protocol reported. Relevant to [[04 Evidence/Thermal Artifact]], [[04 Evidence/Surgical Margins]], [[03 Concepts/Glossary/Carbonization]], and [[03 Concepts/Glossary/Coagulation Zone]] (coagulation zone not scored).
