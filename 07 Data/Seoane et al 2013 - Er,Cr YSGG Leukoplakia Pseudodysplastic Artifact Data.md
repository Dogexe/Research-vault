---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: false
wavelength_nm: 2780
set_power_w: 2
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "PW"
fiber_diameter_um: 600
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
thermal_damage_measure: "width of thermal damage at incision edge (μm): mean 26.60±25.3 across n=4, per-patient range 3.32–56.86 μm"
margin_quality: null
tissue_architecture: "qualitative/count (pseudodysplastic epithelial artefacts: cellular/nuclear polymorphism, nuclear hyperchromatism, loss of intercellular adherence — presence/absence per patient, all described as low-intensity, basal/suprabasal layer only)"
specimen_interpretability: "Paper's central interpretive conclusion: the thermal-artifact profile 'avoids diagnostic interferences with real dysplastic borders' — i.e., the pseudodysplastic artifact did not interfere with distinguishing artifact from a genuine dysplasia diagnosis at the margin (stated as an overall interpretive conclusion, not a per-case scored variable)."
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: CORE BIOPSY — NOT a diode laser.** Er,Cr:YSGG is a solid-state garnet laser, distinct from the diode devices covered elsewhere in this vault; `diode_laser: false` is deliberate and confirmed, not an oversight. Included as a **non-diode methodological precedent** specifically for its blinded, two-pathologist consensus scoring of thermal artifacts that could be mistaken for real dysplasia — the "pseudodysplastic artifact" construct is genuinely new to this vault (see [[03 Concepts/Glossary/Glossary Index]] discovery candidates below).

## Source

- Literature note: [[02 Literature/10.1007/s10103-013-1266-9]]
- Source link: https://doi.org/10.1007/s10103-013-1266-9
- Source locator: Full text (cached plain-text extraction, `.zotero-ft-cache`) — Abstract; Methods and materials; Results; Table 1 (case series); Table 2 (heat damage/artifact distribution); Discussion; References.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Waterlase MD (Biolase Technology, Inc., San Clemente, CA, USA) | — | Methods | FACT |
| Wavelength | 2780 | nm | Methods | FACT |
| Device output range (spec, not the value used) | 0.1–8 | W | Methods | FACT (device spec, not the operating value) |
| Set power (excision) | 2 | W | Methods | FACT — "operated at the 3C preset (recommended for soft tissue incisions), at 2-W power" |
| Set power (hemostasis only, 2 of 4 patients, secondary use) | 0.75 | W | Results | FACT — separate, non-excision use; "off-water/off-air" with tip in motion, for bleeding control only |
| Pulse repetition rate (excision) | 20 (stated range: 10–50) | Hz | Methods | FACT |
| Pulse duration | 140 | μs | Methods | FACT |
| Energy per pulse | 100 | mJ | Methods | FACT |
| Fluence | 35.7 | J/cm² | Methods | FACT |
| Operating mode | Pulsed (device spec states "pulse repetition rate... at pulsed mode") | — | Methods | FACT |
| Fiber/tip | Sapphire tip, 600 μm diameter optic fiber | μm | Methods | FACT |
| Tip initiation status | UNKNOWN — not addressed anywhere in the text | — | — | UNKNOWN |
| Contact mode | Contact — "directing the laser beam (contact mode: slightly touching the mucosa)" | — | Methods | FACT |
| Water/air cooling spray | 30/10% (water/air), 6 mL water/min, for the excision protocol; "off-water/off-air" for the hemostasis-only application | % | Methods | FACT |
| Independently measured power | NO — the device's output range is a manufacturer specification; no power meter or independent verification step is described anywhere in the text | — | — | FACT (absence confirmed by full-text read) |
| Incision speed | NOT REPORTED — no mm/s value anywhere; the hemostasis-only use describes "the tip in motion" with no speed value | — | — | UNKNOWN |
| Sample | 4 oral leukoplakia patients (3 female), mean age 59, 2 homogeneous + 2 nonhomogeneous leukoplakias; complete surgical excision | — | Results | FACT |
| Tissue processing | 10% formalin-buffered saline, 24 h fixation; 4 μm sections; H&E stain; same technician for all specimens | — | Methods | FACT |
| Pathologist involvement | **Two pathologists**, **double-blinded**, studied specimens **until a consensus was reached for each case** | — | Methods | FACT |
| Magnification / measurement instrument | Optiphot-2 microscope (Nikon) with a millimeter-calibrated eyepiece graticle (Graticules, Town Bridge, Kent, UK) | — | Methods | FACT |
| Width of thermal damage at incision edge | Mean 26.60±25.3 μm across the series; per-patient: P1 5.62±2.07, P2 56.86±17.79, P3 3.32±1.02, P4 40.62±10.36 μm | μm | Results; Table 2 | FACT |
| Pseudodysplastic epithelial artefacts | Present in 2 of 4 patients (P2, P4); described as low-intensity, located at basal/suprabasal epithelial layers only | Presence/absence, per patient | Results; Table 2 | FACT |
| Cellular/nuclear polymorphism | Present in 2 of 4 patients (P2, P4) | Presence/absence | Table 2 | FACT |
| Nuclear hyperchromatism | Present in 2 of 4 patients (P2, P4) | Presence/absence | Table 2 | FACT |
| Loss of intercellular adherence | Present in 3 of 4 patients (P2, P3, P4) — "the most frequent thermal artifact in this series" | Presence/absence | Table 2 | FACT |
| Autolysis, fixation/handling artifacts | NONE observed in any sample ("no autolysis, and no fixation- or handling-related artifacts (pseudocysts, crushing, fragmentation, hemorrhage, or fissures)") | Absent | Results | FACT |
| Histological diagnosis rendered | Yes — squamous hyperplasia (P1, P2, P4), moderate dysplasia (P3) | — | Table 1 | FACT |
| Diagnosis affected/interfered by artifact | NOT reported as a formal per-case judgment; the paper's own conclusion states the protocol "avoids diagnostic interferences with real dysplastic borders" as an overall interpretive conclusion, not a per-case adjudicated variable | — | Discussion; Conclusion | FACT (stated as a conclusion, not a scored outcome) |

## Study design (per task's Section A)

- Human, in vivo. NOT ex vivo.
- **True diagnostic/excisional biopsy pathway**: real oral leukoplakia lesions, complete surgical excision, histological diagnosis rendered per case (including one case of moderate dysplasia — i.e., this is not a purely benign/non-dysplastic sample set).
- No comparator group in this paper itself — single-arm case series. (CO2 laser is discussed extensively as a comparator in the Introduction/Discussion by citation to other studies, not as a study arm here.)
- Sample size: n=4 patients (very small — explicitly a "pilot study").
- Tissue/site: soft palate, lateral lingual margin/floor of mouth, angle of mouth, gingiva.

## Histopathology methodology (per task's Section C)

- Fixation: 10% formalin-buffered saline, 24 h. Sections 4 μm, H&E.
- **Pathologist involvement: two pathologists.**
- **Blinded: YES, explicitly stated** ("double-blindedly studied by two pathologists").
- **Consensus process: YES, explicitly stated** ("until a consensus was reached for each case").
- **Inter-rater reliability statistic: NOT REPORTED** — the paper describes a consensus process but does not report a kappa or other quantified agreement statistic. Per task instruction, this is stated as NOT REPORTED, not inferred as "high agreement."
- Magnification: not given as a numeric power; described via the graticle-equipped microscope used for epithelial thermal-damage measurement.

## Outcome terminology (author's exact wording, per task's Section D)

- **"Pseudodysplastic artifacts"** / **"pseudodysplastic epithelial artifacts"** — the paper's own term, used repeatedly and centrally.
- **"Width of the thermal damage at the edge of the incision"** — the paper's own phrase for the μm measurement (not given a named abbreviation, unlike Monteiro's "TDE" or Prado's "TDD/TDA").
- **"Cellular and nuclear polymorphism"**, **"nuclear hyperchromatism"**, **"loss of intercellular adherence"** — the paper's own named sub-components of the pseudodysplastic-artifact construct.
- **"Avoids diagnostic interferences with real dysplastic borders"** — the paper's own concluding language; NOT the same construct as "diagnosis affected: Yes/No" used in Monteiro 2019 or the Lopes-Santos review (already in vault) — this paper frames the finding as a qualitative interpretive conclusion about margin trustworthiness, not a scored per-case diagnostic-outcome variable.

## Outcome type (per task's Section E)

| Outcome | Type | Unit/range | Epithelial component? | CT component? | Margin-specific? | Architecture-specific? | Diagnosis affected? | Adequacy/readability judgment? |
|---|---|---|---|---|---|---|---|---|
| Width of thermal damage | Quantitative continuous | μm, per-patient mean±SD | Yes (epithelial, explicitly) | No (not separately reported for connective tissue) | Yes | No | No | No |
| Pseudodysplastic artifact presence | Binary/count, per patient | Present/absent, 3 named sub-types | Yes | No | No | Yes (architecture: polymorphism, adherence) | No | Indirectly — low-intensity artifact framed as non-diagnosis-threatening |
| "Avoids diagnostic interferences with real dysplastic borders" | Qualitative descriptive conclusion, not a scored variable | N/A | — | — | — | — | Interpretive, not scored | Yes — the paper's central adequacy/readability claim |

## Score/grading details (per task's Section F)

- **No named numeric score is used in this paper** — thermal-damage width is a direct linear measurement (not an ordinal scale); pseudodysplastic-artifact presence is recorded as present/absent per sub-type per patient, not summed into an ordinal score (contrast with Monteiro 2019's and Vescovi 2010's 0–3/0–4 sum-scores).
- Score name: N/A (no formal score).
- Validation status: N/A (no score created or reused as a numeric instrument).
- **Blinded scoring: YES.**
- **Number of scorers: 2, with consensus.**
- **Reliability statistic: NOT REPORTED.**

## Diagnostic-interpretability findings (task's specific focus for this source)

- FACT: The paper's central claim is that Er,Cr:YSGG-induced thermal artifacts are distinguishable from — and did not obscure — real dysplastic changes: one of the four patients (P3) had a genuine histological diagnosis of moderate dysplasia rendered, alongside (not confused with) the pseudodysplastic-artifact assessment applied uniformly across the series.
- FACT: The paper explicitly frames the risk this addresses: "margins of lesions treated with lasers may simulate cytological atypia (hyperchromatism, pleomorphism and nuclear elongation, and vacuolar degeneration)," citing this as a recognized problem for CO2-laser-excised specimens specifically (via cited prior work, e.g. its own reference to Seoane et al. 2010 and González-Mosquera et al. 2012 — the latter already identified in this vault's Phase 4 search).
- FACT: The paper's own stated safety-margin implication: CO2/diode/Nd:YAG lasers "demand an additional amount of healthy tissue (1 to 3 mm)," whereas Er,Cr:YSGG's measured thermal-damage width "would make such wide safety margins unnecessary" — an explicit, source-stated margin-width recommendation tied to the measured value, comparable in structure to [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]]'s ≥1 mm recommendation, but for a non-diode laser.

## Notes

- FACT: This is the vault's first source with an explicitly **blinded, two-pathologist consensus** histologic assessment — a stronger pathologist-involvement design than any diode-specific source currently in the vault (all of which use one pathologist, blinded or unspecified).
- FACT: Sample size is very small (n=4) and is explicitly self-described as a "pilot study" and "descriptive... cross-sectional analysis" — this limits how far the "avoids diagnostic interferences" conclusion can be generalized.
- FACT: No comparator arm (single-technique case series) — this paper alone cannot support a cross-laser comparison; its value is methodological (blinding + consensus + the pseudodysplastic-artifact construct itself), not comparative.
- NEEDS VERIFICATION flagged in YAML: (1) `set_power_w: 2` records the excision-protocol power only; the paper also reports a distinct 0.75 W hemostasis-only setting used in 2 of 4 patients for bleeding control, which is NOT the excision power and is preserved separately in the Extraction table above — a human should confirm this scoping choice is the intended one; (2) whether "avoids diagnostic interferences with real dysplastic borders" should populate `diagnostic_outcome: true` is a judgment call, since the paper frames this as an interpretive conclusion rather than a per-case scored variable — recorded as `true` here because a real histological diagnosis (including one dysplasia case) was in fact rendered on every specimen, consistent with the schema's definition ("whether a clinical/histopathologic diagnosis was rendered from the specimen").
- Classification for this vault: CORE BIOPSY, non-diode. Strengthens the diagnostic-artifact-methodology precedent base materially; does not touch the diode-specific or measured-power axes.

## สรุปภาษาไทย

- การศึกษานี้เป็น pilot study ในผู้ป่วย leukoplakia 4 รายที่ตัดออกด้วยเลเซอร์ Er,Cr:YSGG (ไม่ใช่เลเซอร์ไดโอด) โดยมี**พยาธิแพทย์ 2 คน อ่านผลแบบปกปิดข้อมูล (double-blinded) จนกว่าจะได้ข้อสรุปร่วมกัน (consensus)** — เป็นระเบียบวิธีที่เข้มงวดกว่าแหล่งข้อมูลไดโอดทุกฉบับในคลังนี้
- คำศัพท์สำคัญที่บทความนี้ใช้เองคือ "pseudodysplastic artifacts" (สิ่งแปลกปลอมจากความร้อนที่มีลักษณะคล้าย dysplasia) — พบใน 2 ใน 4 ราย ความรุนแรงต่ำ อยู่เฉพาะชั้น basal/suprabasal ของเยื่อบุผิว
- ความกว้างของความเสียหายจากความร้อนที่ขอบแผลเฉลี่ย 26.60±25.3 ไมโครเมตร
- บทความสรุปว่าเลเซอร์นี้ "หลีกเลี่ยงการรบกวนการวินิจฉัยกับขอบเขตของ dysplasia จริง" แต่เป็นกลุ่มตัวอย่างเล็กมาก (n=4) ไม่มีกลุ่มเปรียบเทียบ
- ไม่มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์ และไม่มีการรายงานความเร็วตัด

## Related notes

- Literature: [[02 Literature/10.1007/s10103-013-1266-9]]
- Data: [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data]] (cites the same "pseudodysplastic" artifact family)
- Evidence: [[04 Evidence/Biopsy Specimen Quality]]
- Concepts: [[03 Concepts/Glossary/Histological Artifact]], [[03 Concepts/Glossary/Diagnostic Quality]]
- Synthesis: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
- Project: [[01 Projects/Diode Laser Biopsy]]
