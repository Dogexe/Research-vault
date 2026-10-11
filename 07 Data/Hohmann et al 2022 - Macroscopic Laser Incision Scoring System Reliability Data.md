---
classification: SUPPORTING TECHNICAL (methods precedent — immediate macroscopic incision scoring)
oral_tissue: false
ex_vivo: true
human_tissue: false
diode_laser: false
wavelength_nm: 10600
set_power_w: null
measured_power: null
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
speed_varied: null
cw_pw: null
fiber_diameter_um: null
tip_initiation: null
contact_mode: null
histology: false
thermal_damage: true
thermal_damage_measure: "Macroscopic 1–5 score from tissue colour (black/dark brown/light brown = carbonisation; white = coagulation; pink = undamaged) and darkened-area fraction (≥80%, ≥50%, 30–50%, <30%, none); 5 = best; scored on photographs"
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

- Literature note: [[02 Literature/10.1038/s41598-022-18969-0|Hohmann et al. 2022]]
- Citation: Hohmann M, Kühn D, Späth M, Rohde M, Stelzle F, Klämpfl F, Schmidt M. Development and evaluation of a scoring system for assessing incisions in laser surgery. *Sci Rep*. 2022;12(1):14741. PMID 36042339; PMCID PMC9427958.
- Source link: https://doi.org/10.1038/s41598-022-18969-0
- Source locator: Full text read from local Zotero PDF (storage 88YL5JW3) on 2026-10-11; Materials and methods, Fig. 1–3, Tables 1–4, Limitations, Conclusion.

## Parameters

| Parameter | Value | Unit | Locator | Label |
|---|---|---|---|---|
| Device | CO2 laser — model UNKNOWN | — | Materials and methods | FACT |
| Wavelength | UNKNOWN in this paper (CO2 only; 10,600 nm taken from the follow-up paper's device, same group) | nm | — | INTERPRETATION |
| Set power / mode / speed / spot | UNKNOWN — authors state laser parameters were varied but deliberately not reported, as not relevant to this reliability study | — | Materials and methods | FACT |
| Measured output power | UNKNOWN — not reported | — | — | UNKNOWN |
| Tissue | Muscle tissue from freshly slaughtered pigs (local butcher) | — | Materials and methods | FACT |
| Scored regions | Cutting area (CA) = new surface created by the cut; cutting edge (CE) = fine rim between cut and uncut surface | — | Scoring system; Fig. 1 | FACT |
| Score 1 | Dark brown to black; ≥80% darkened; strong carbonisation | — | Fig. 2; list 1–5 | FACT |
| Score 2 | Light brown to black; ≥50% darkened | — | Fig. 2 | FACT |
| Score 3 | Light brown and darker, normally no black; ~30–50% darkened | — | Fig. 2 | FACT |
| Score 4 | <30% darkened; large white (coagulation) areas, pink possible; shimmering possible ex vivo | — | Fig. 2 | FACT |
| Score 5 | No or nearly no darkening; pinkish and white dominate | — | Fig. 2 | FACT |
| Images scored | 115 cuts, one photograph per cut (not fresh tissue) | — | Scoring procedure; Limitations | FACT |
| Raters | 12 optics scientists, none with laser-surgery experience: 6 untrained (Fig. 2 only), 6 trained (25-image training with feedback, then 90 scored) | — | Scoring procedure; Fig. 3 | FACT |
| Statistic | ICC3, single fixed raters, absolute agreement (Python pingouin); Spearman; Wilcoxon signed-rank CA vs CE | — | Statistical evaluation | FACT |
| ICC untrained | CE 0.62 (95% CI 0.54–0.69); CA 0.71 (0.65–0.77) | — | Table 1 | FACT |
| ICC trained | CE 0.66 (0.58–0.74); CA 0.69 (0.61–0.76) | — | Table 3 | FACT |
| Learning effect, untrained | First third 0.56 (0.43–0.70) → last third 0.75 (0.64–0.84) | — | Table 2 | FACT (region label inconsistent — see Notes) |
| Learning effect, trained | First third 0.64 (0.50–0.78) → last third 0.72 (0.59–0.83) | — | Table 4 | FACT (region label inconsistent — see Notes) |
| Spearman | Mean CA 0.70; CE 0.62; CA vs CE 0.41; CA and CE distributions differ (p ≪ 1×10⁻³) | — | Results | FACT |

## Notes

- FACT: Authors recommend raters practise on ~100–200 samples before scoring a final data set, based on the ~0.2 ICC rise between first and last thirds.
- FACT: Authors state there is no gold standard for laser-incision evaluation; reliability (inter-rater agreement) is the validation used.
- FACT: Authors state scores cannot currently predict clinical outcomes (healing, scarring) and that scoring of fresh tissue directly after the cut still needs evaluation.
- FACT: Authors state the system should apply to other lasers and thermal cutting modalities, but this was not tested here.
- NEEDS VERIFICATION: Table 2 and Table 4 captions say "ICC for the CE", but their column headers say "CA 1 / CA 3", and the Results text describes Table 2 as CA and Table 4 as CE. Which region each learning-effect table describes cannot be settled from the paper.
- INTERPRETATION: Uses CO2 non-histologic macroscopic scoring on pig muscle. Transfer to 980 nm contact diode cutting on porcine tongue mucosa needs re-testing of reliability (adapted score + pilot ICC), as the 2026-10-11 advisor feedback requires.

## สรุปภาษาไทย

งานนี้พัฒนาระบบให้คะแนนรอยตัดเลเซอร์ด้วยตาเปล่า 1–5 คะแนน (5 = ดีที่สุด) โดยดูสีของเนื้อเยื่อ (ดำ/น้ำตาล = carbonisation, ขาว = coagulation, ชมพู = ปกติ) ร่วมกับสัดส่วนพื้นที่ที่คล้ำ แยกประเมินที่ cutting area (CA) และ cutting edge (CE) ผู้ประเมิน 12 คนให้คะแนน 115 รอยตัด (CO₂, กล้ามเนื้อหมู) จากภาพถ่าย ได้ ICC ของ CA = 0.71 และ CE = 0.62 ในกลุ่มที่ไม่ได้ฝึก ไม่มีการรายงานพารามิเตอร์ของเลเซอร์ ระบบนี้ไม่ใช่ gold standard และยังไม่ได้ทดสอบกับเนื้อเยื่อสด
