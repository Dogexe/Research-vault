---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 980
set_power_w: 3
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW+PW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.4103/jpbs.jpbs_861_21]]
- Source link: https://doi.org/10.4103/jpbs.jpbs_861_21
- Source locator: Full text retrieved from PubMed Central (PMC9469426), via the PubMed MCP tool (`get_full_text_article`). According to PubMed, this is Gundlapalle P, Nagappan N, Ramesh P, Ziauddhin S, Karthick BP, Paleti VSM, Kumar BV. "Comparison of Oral Mucosal Biopsies Done Using Scalpel and Diode Lasers: A Vivo Study." *J Pharm Bioallied Sci.* 2022;14(Suppl 1):S947-S954. [DOI](https://doi.org/10.4103/jpbs.jpbs_861_21). No PDF is cached in this vault's local Zotero library for this source (the literature note has no attached-file link); the full text was instead retrieved directly from PMC.

## Extraction

Scope note: this is a three-arm human clinical comparison (scalpel vs. diode laser continuous-wave [CW] vs. diode laser pulsed-wave [PW]). Only the diode-laser rows and the diode-vs-scalpel comparisons directly relevant to biopsy specimen quality are extracted here; procedure-time, local-anesthesia-volume, and pain-scale outcomes are noted only where the source ties them to laser mode.

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | 980 nm Zolar Plus diode laser | — | Methodology | FACT |
| Manufacturer | UNKNOWN (brand name "Zolar Plus" only; manufacturer/company not stated in the retrieved text) | — | — | UNKNOWN |
| Wavelength | 980 | nm | Methodology | FACT |
| Set power | 3 | W | Methodology | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; set/console value only | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) and pulsed wave (PW), compared as two arms at the same nominal 3 W set power | — | Methodology | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | UNKNOWN | — | — | UNKNOWN |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | UNKNOWN — not explicitly stated as contact or non-contact | — | — | UNKNOWN |
| Exposure duration | UNKNOWN as a per-incision value; total procedure time reported instead (see below) | — | — | UNKNOWN (per-incision) |
| Excision/incision protocol | Both incisional and excisional biopsies performed depending on clinical diagnosis; tissue taken large enough to include normal and suspicious tissue | — | Methodology | FACT |
| Specimen size | UNKNOWN — no specimen diameter/size value or distribution reported | — | — | UNKNOWN |
| Measurement method — thermal damage | Width of necrotic border at the specimen periphery, measured on laser-cut tissue sections using Quick Capture Pro 6.0 software | — | Methodology; Results | FACT |
| Measurement method — slide quality | Quality of slide at periphery and center [[03 Concepts/Glossary/Artifact Grading\|graded]] microscopically by a pathologist: 1 = good, 2 = average, 3 = poor, 5 = non-diagnostic (the source's own scale omits a "4" grade; preserved as reported) | — | Methodology | FACT |
| [[03 Concepts/Glossary/Calibration\|Calibration]] method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Thermal damage (necrotic border width) — CW | Mean 279.84 | μm | Results | FACT |
| Thermal damage (necrotic border width) — PW | Mean 208.766 | μm | Results | FACT |
| Recommended specimen margin | Minimum 5 mm of normal tissue margin, "if a diode laser with a power setting of 3W or lesser is used," due to thermal damage at margins potentially confounding lesion-extent/dysplasia assessment | mm | Discussion/Conclusion | FACT |
| Diagnostic yield (quantified) | UNKNOWN — no numeric diagnostic-accuracy or unreadable-specimen percentage is reported in the retrieved text; the source states qualitatively that laser-biopsy artifacts "were negligible, thus allowing adequate histological examination and correct diagnosis" | — | Conclusion | FACT (qualitative statement only) / UNKNOWN (quantified yield) |
| Slide quality, periphery/center — CW vs. PW | PW had better quality at both periphery and center than CW (source's own comparative statement; no numeric grade values given for either arm) | — | Results | FACT |
| Slide quality, laser vs. scalpel | Scalpel slide quality (periphery and center) was better than laser overall — no thermal damage in the scalpel arm | — | Results; Discussion | FACT |
| Coagulation zone | Not scored or measured as an isolated variable; the Discussion describes coagulation only as a general laser-tissue physics mechanism (collagen shrinkage sealing vessels), not a measured finding of this study's own specimens | — | Discussion | FACT (mechanism description, not a study finding) |
| Carbonization | Listed as an observed artifact (Figure 5 caption: "Carbonization"), not scored numerically or separated by CW/PW arm | — | Results (figure) | FACT (qualitative) |
| [[03 Concepts/Glossary/Histological Artifact\|Histologic artifacts]] reported | Tissue necrosis, fibrous degeneration, hyperchromatism, nuclear elongation, intercellular spacing, loss of cellular morphology, intercellular edema, hyalinization, shedding of keratin, vacuolation, epithelium separation from connective tissue | — | Results | FACT |
| Procedure time — CW vs. PW | CW: mean 15.467 ± 4.549 min; PW: mean 22.000 ± 3.927 min; PW took significantly longer (p=0.000). This is total procedure time (includes anesthesia/positioning), not a pure incision/exposure time. | min | Results | FACT |
| Sample | 60 patients total; 30 scalpel, 30 diode laser (15 CW at 3W, 15 PW at 3W); Department of Oral Medicine | — | Methodology | FACT |

## Notes

- FACT: This source directly compares [[03 Concepts/Glossary/Continuous Wave|CW]] and [[03 Concepts/Glossary/Pulsed Mode|PW]] diode-laser modes at the same nominal 3 W set power in a real human biopsy pathway, and found PW produced a smaller mean [[03 Concepts/Glossary/Thermal Damage|thermal-damage]] (necrotic border) width than CW (208.766 μm vs. 279.84 μm) and better pathologist-graded [[03 Concepts/Glossary/Margin Quality|slide quality]] at both periphery and center — the vault's first source to directly compare CW vs. PW mode, at matched set power, in real human oral biopsy specimens.
- FACT: The source's own recommendation (≥5 mm normal-tissue margin at 3 W or lower) is consistent in order of magnitude with, though independently derived from, Angiero et al.'s ≥5 mm in vivo recommendation and Gambino et al.'s standardized 5 mm protocol already in this vault — a third, independent convergence on the same figure. [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]] [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data]]
- FACT: No numeric diagnostic-yield or unreadable-specimen percentage is reported for either the scalpel or diode arms in the retrieved full text, despite the study's stated aim to note "co-relation of provisional and final diagnosis" — this aim's quantified result is not present in the Results section as retrieved. This is treated as UNKNOWN, not inferred.
- FACT: The source's own scale for slide-quality grading skips the value "4" (1-good, 2-average, 3-poor, 5-non-diagnostic) — preserved as reported, not corrected or assumed to be a typo.
- FACT (source's own citation, not independent vault verification): the Discussion cites "Capodiferro. noted that regressive tissue changes due to thermal cut of diode lasers are usually negligible, thus allowing adequate histological examination and correct diagnosis" and "Suter. evaluated histopathological characteristics and suitability of diode and CO2 lasers... concluded that both the lasers can be used successfully" — both are this source's own citations of Capodiferro et al. 2008 and Suter et al. 2010 (both still unprocessed in this vault, see [[01 Projects/Diode Laser Biopsy]]), not independent vault confirmation of either paper's findings.
- INTERPRETATION (source's own): the Discussion attributes varying slide quality within the laser group (despite identical 3 W set power) to tissue chromophore/wavelength absorption differences (hemoglobin, melanin, water) rather than to the power setting itself.
- HYPOTHESIS: UNKNOWN — no formal hypothesis beyond the source's own recommendations is proposed.
- Classification for this vault: direct dental-diode CW-vs-PW thermal-damage and specimen-margin evidence, in a real human biopsy pathway — set power only, no independent power-meter verification, no quantified diagnostic-yield percentage. Relevant to [[04 Evidence/Thermal Artifact]], [[04 Evidence/Surgical Margins]], and [[03 Concepts/Glossary/Carbonization]].
