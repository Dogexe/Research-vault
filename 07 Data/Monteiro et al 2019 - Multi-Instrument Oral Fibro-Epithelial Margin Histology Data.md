---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 980
set_power_w: 3.5
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "PW"
fiber_diameter_um: 300
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: "quantified (Tissue Damage Extension, TDE, μm, epithelial and connective separately, by instrument); diode arm: epithelial 913.73±322.45 μm, connective 284.81±110.56 μm — highest epithelial TDE of the six instruments tested"
tissue_architecture: "ordinal (epithelial score 0–3 and connective score 0–3, summed from nuclear/cytoplasmic/attachment-loss and carbonization/desiccation/vascular sub-items; plus regularity-of-incision score 0–4); diode arm: epithelial score 2.95±0.22 (highest of six), connective score 2.76±0.54, incision-regularity score 1.86±0.73 (least regular of six)"
specimen_interpretability: null
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: CORE BIOPSY — a real, six-instrument human comparison** (CO2 laser, diode laser, Er:YAG laser, Nd:YAG laser, electrosurgical scalpel, cold scalpel), n=130 real excised benign fibro-epithelial hyperplasias, single blinded pathologist, explicit per-case diagnosis-limitation judgment. **This is the single most important non-diode multi-modality precedent found in the Phase 4 literature search** — see [[04 Evidence/Biopsy Specimen Quality]] and [[06 Synthesis/Diode Laser Biopsy Specimen Quality]].

**YAML scoping note (per schema convention, matching how [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]] and [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] treat their own comparator arms): the YAML frontmatter above records ONLY the diode-laser arm's parameters** (`wavelength_nm`, `set_power_w`, `margin_quality`, `tissue_architecture` are diode-specific), per [[99 Templates/Study Metadata Schema]]'s field definition that `wavelength_nm`/`set_power_w` capture "the diode arm only." **The other five instruments' full data are preserved below in the Extraction table and Notes — they are not discarded, only excluded from the diode-scoped YAML fields**, consistent with this study being a genuine six-way comparison, not a diode-only study.

## Source

- Literature note: [[02 Literature/10.4317/medoral.22819]]
- Source link: https://doi.org/10.4317/medoral.22819
- Source locator: Full text (cached plain-text extraction, `.zotero-ft-cache`, cross-checked against the article's own tables) — Abstract; Material and Methods; Table 1 (patient characteristics); Table 2 (epithelial/connective alterations, scores); Table 3 (TDE by instrument and specimen size); Results; Discussion; Conclusions; References.

## Extraction — all six instrument groups (not diode-only)

| Parameter | CO2 laser | Diode laser | Er:YAG laser | Nd:YAG laser | Electrosurgical scalpel | Cold scalpel | Evidence status |
| --- | --- | --- | --- | --- | --- | --- | --- |
| n | 27 | 21 | 22 | 25 | 15 | 20 | FACT |
| Device | DEKA® Smart US 20D | LITEMEDICS® (Brendola, Italy) | FOTONA® LigthWalker | DEKA® Smart US 20D (Smarty-A10) | CARLO DI GIORGI® | KIATO® blade #15C | FACT |
| Wavelength | 10600 nm | 980 nm | 2940 nm | 1064 nm | N/A | N/A | FACT |
| Power | 4 W (80 Hz, 50 mJ, angulated mirror handpiece, 0.5 mm spot) | 3.5 W (300 μm fiber, contact, 50 Hz, 70 mJ) | 4 W (angulated mirror handpiece H02, 0.5 mm spot, 20 Hz, "Long pulse," 200 mJ) | 4 W (300 μm fiber, contact, 40 Hz, "short pulse," 100 mJ) | 5 W ("cut/coagulation" mode, 0.22 mm electrode) | N/A | FACT |
| Power density / fluence | 2040.8 W/cm², 40.8 J/cm² | 4957.5 W/cm², 99.2 J/cm² | 2040.8 W/cm², 102 J/cm² | 5665.7 W/cm², 141.6 J/cm² | UNKNOWN | N/A | FACT |
| Contact mode | UNKNOWN (angulated mirror handpiece, not fiber-contact) | Contact | UNKNOWN (angulated mirror handpiece) | Contact | Contact | N/A | FACT (diode, Nd:YAG, electrosurgical) |
| Independently measured power | NO — every instrument's power is the manufacturer-recommended device setting; no power meter or independent verification instrument is named anywhere in Methods | — | — | — | — | — | FACT (absence confirmed for all six groups) |
| Incision speed | NOT REPORTED for any instrument — no mm/s value or speed-control description anywhere in the text | — | — | — | — | — | FACT (absence) |
| Epithelial score (0–3, sum of nuclear/cytoplasmic/attachment-loss) | 2.59±0.5 | **2.95±0.22 (highest)** | 1.91±0.68 (lowest of the five active instruments) | 2.88±0.33 | 2.80±0.41 | 0.20±0.52 | FACT |
| Connective score (0–3, sum of carbonization/desiccation/vascular) | 2.81±0.39 | 2.76±0.54 | 2.45±0.59 (lowest of five) | 2.64±0.57 | **2.87±0.35 (highest)** | 0.05±0.22 | FACT |
| Regularity-of-incision score (0–4, 4=best/scalpel-like) | 2.64±0.79 (best of the five active instruments) | **1.86±0.73 (worst)** | 2.44±0.85 | 2.08±0.64 | 2.07±0.88 | 3.25±0.64 | FACT |
| Epithelial TDE (μm, mean±SD) | 538.37±170.50 | **913.73±322.45 (2nd highest)** | 166.47±123.85 (lowest of five) | 899.83±327.75 | 1002.19±434.92 (highest) | 2.36±7.27 | FACT |
| Connective TDE (μm, mean±SD) | 201.69±89.86 | 284.81±110.56 (3rd) | 48.54±26.09 (lowest of five) | 310.85±107.45 | 393.80±359.11 (highest) | 0±0 | FACT |
| Histological diagnosis affected? | No | No | No | No | No | No | FACT — "no case showed any limitation of diagnosis related with the use of any instrument evaluated" |

## Study design (per task's Section A)

- Human, in vivo, retrospective (Jan 2010–Jul 2018), single-center (University Institute of Health Sciences, CESPU, Portugal). NOT ex vivo.
- **True diagnostic/excisional biopsy pathway**: real benign fibro-epithelial hyperplasia lesions (fibro-epithelial hyperplasia, denture-related fibrous hyperplasia, fibroma, fibropapilloma), histological diagnosis rendered on every specimen.
- Comparator groups: 6 arms (CO2, diode, Er:YAG, Nd:YAG, electrosurgical scalpel, cold scalpel), instrument assigned "randomly" per patient (method of randomization not further described — FACT of the term used, not a described randomization protocol).
- n=130 total (originally 142, 12 excluded for incomplete data/no specimen).
- Tissue/site: buccal-vestibular-lip mucosa (n=70), gingiva (n=32), hard palate (n=7), soft palate (n=4), tongue (n=17); 91 non-keratinized, 39 keratinized.
- Mean specimen size 1.11±0.83 cm (range 0.4–6 cm); no significant between-group difference (P=0.502).

## Histopathology methodology (per task's Section C)

- Fixation: 10% buffered formalin. Serial sections 3 μm, H&E stain.
- Microscope: ZEISS AxioLab A1, ZEISS Axiocam 105 color, ZEISS Zen2 software.
- **Pathologist involvement: one experienced pathologist**, explicitly stated **blinded to the type of surgical instrument used**.
- Number of assessors: 1. **NOT a multi-pathologist consensus design** — contrast with [[07 Data/Seoane et al 2013 - Er,Cr YSGG Leukoplakia Pseudodysplastic Artifact Data|Seoane et al. 2013]]'s two-pathologist blinded consensus, below.
- Inter-rater reliability: NOT REPORTED (single assessor — not applicable).
- Magnification: 40× for the presence/absence histological alterations; TDE measured "from the greatest distance from the edge of the incision to the end of the laser thermal damage, perpendicular to the surgical margin."
- **Histologic evaluation criteria explicitly stated as borrowed, not invented in this paper**: "The presence of histological alterations adjacent to the surgical margins were evaluated... according the criteria established by Vescovi et al. (8)" — i.e., [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data|Vescovi et al. 2010]]. This is a direct, source-confirmed methodological lineage, not an inference.

## Outcome terminology (author's exact wording, per task's Section D)

- **"Tissue damage extension (TDE)"** — the paper's own named, defined metric (its own abbreviation).
- **"Epithelial score"** and **"Connective score"** — the paper's own constructed sum-scores (0–3 each), built from the individual binary sub-items (nuclear changes, cytoplasm changes, loss of attachment; carbonization, desiccation, vascular changes).
- **"Regularity of the incision"**, scored 0–4 ("morphology and regularity of the incision on a scale of 0 to 4 where level 4 represents the highest quality and 0 the worst").
- **"No... limitation of diagnosis"** — the paper's own binary diagnostic-interference judgment, stated once for the whole cohort, not scored per case in the tables.

## Outcome type (per task's Section E)

| Outcome | Type | Unit/range | Epithelial component? | CT component? | Margin-specific? | Architecture-specific? | Diagnosis affected? | Adequacy/readability judgment? |
|---|---|---|---|---|---|---|---|---|
| TDE | Quantitative continuous | μm, mean±SD, by group and by <1.1cm/≥1.1cm | Yes (separate) | Yes (separate) | Yes (distance from margin) | No | No | No |
| Epithelial score | Ordinal (sum of binary sub-items) | 0–3 | Yes | No | No | Yes | No | No |
| Connective score | Ordinal (sum of binary sub-items) | 0–3 | No | Yes | No | Yes | No | No |
| Regularity-of-incision score | Ordinal | 0–4 (4=best) | No | No | Yes (edge quality) | No | No | Yes (incision-quality proxy, not diagnostic-readability) |
| "No limitation of diagnosis" | Binary, whole-cohort statement | Yes/No | — | — | — | — | Yes | Yes (explicit diagnostic-adequacy judgment) |

## Score/grading details (per task's Section F)

- **TDE**: NOT a score — a direct linear measurement (ocular/software-based, instrument not further specified beyond the named microscope/camera system). Not reused from prior literature under this exact name (contrast: the epithelial/connective *evaluation criteria* were reused from Vescovi et al. 2010, but "TDE" as a named abbreviation appears original to this paper).
- **Epithelial/Connective scores (0–3)**: created for this paper as a sum of the individual sub-item binary variables (each present/absent), built on top of Vescovi et al. 2010's underlying criteria set. Not stated as validated. Single blinded scorer. No inter-rater reliability statistic (single assessor).
- **Regularity-of-incision score (0–4, 4=best)**: same construction — reused conceptually from Vescovi et al. 2010, which used an equivalent 0–4 "overall quality score." Not stated as validated. Single blinded scorer.
- Diagnosis-affected judgment: binary, per-case (implied from "no case showed any limitation"), not itself an ordinal score.

## Diode subgroup vs. other lasers — explicit differences

- FACT: Diode had the **highest epithelial score (2.95±0.22)** and the **worst (least regular) incision score (1.86±0.73)** of all six instruments — i.e., diode was the *least favorable* instrument on two of the three ordinal constructs.
- FACT: Diode's epithelial TDE (913.73 μm) was the second-highest after electrosurgical scalpel; its connective TDE (284.81 μm) was mid-range (3rd of six).
- FACT: A correlation was found between incision score and TDE (epithelial r=−0.438, connective r=−0.467, both P<0.001) — lower-quality (less regular) incisions were associated with greater TDE. The diode arm's own combination (worst incision score + high TDE) is internally consistent with this correlation.
- FACT: The paper's own Discussion cites Cercadillo-Ibarguren et al. 2010 as independently observing that "diode group presented the most significant thermal cell damage" — an external cross-study confirmation of the diode arm's relatively poor performance in this paper, not this vault's own interpretation.

## Specimen size

- FACT: No correlation was found between specimen size and epithelial TDE (P=0.661) or connective TDE (P=0.288), or between size and any of the categorical alteration variables, **in this study specifically** — a direct contrast with [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data|Vescovi et al. 2010]] (below) and with the vault's existing Angiero et al. 2011 finding, both of which found strong size-dependent effects. The paper's own Discussion explicitly notes this contrast, attributing it partly to the fact that "all our samples size were superior to 4mm" (i.e., their sample did not include the very small specimens where Angiero and Vescovi found the strongest effects).

## Notes

- FACT: This is the vault's first source with a genuine 6-arm real-human multi-instrument comparison including a diode arm, a true diagnostic-biopsy pathway, a blinded (single) pathologist, and both a linear (TDE) and ordinal (epithelial/connective/incision-regularity) outcome set — but it independently measures no power for any instrument and reports no incision speed for any instrument, so it does not close this project's core measured-power + speed gap.
- FACT: This paper's own histologic evaluation criteria are explicitly stated as adopted from Vescovi et al. 2010 — a direct, confirmed methodological lineage between two of this phase's four primary extractions.
- NEEDS VERIFICATION flagged in YAML for three judgment calls made during this extraction: (1) `cw_pw: PW` for the diode arm is inferred from the reported frequency (50 Hz) and energy-per-pulse (70 mJ) parameters, since the paper never uses the word "pulsed" or "continuous wave" explicitly for any instrument — this is a physics-based reading of the stated parameters, not an invented value, but should be re-checked against the original PDF tables if a human reviewer wants full confidence; (2) the split of the diode arm's quantitative TDE data into `margin_quality` and its ordinal score data into `tissue_architecture` is a vault convention judgment (matching how [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data|Gambino et al. 2026]] was tagged), not a distinction the source paper itself makes; (3) `tip_initiation: null` reflects that the paper never addresses initiated/non-initiated status for any laser — confirmed absence, not oversight.
- Classification for this vault: CORE BIOPSY — real diagnostic pathway, diode-inclusive, strengthens the multi-modality specimen-quality precedent base materially (see [[06 Synthesis/Diode Laser Biopsy Specimen Quality]]).

## สรุปภาษาไทย

- การศึกษานี้เปรียบเทียบเครื่องมือตัดชิ้นเนื้อ 6 ชนิดในมนุษย์จริง (เลเซอร์ CO2, ไดโอด, Er:YAG, Nd:YAG, electrosurgical scalpel, ใบมีดเย็น) จากรอยโรค fibro-epithelial hyperplasia จริง 130 ราย มีพยาธิแพทย์ 1 คนที่ไม่ทราบว่าใช้เครื่องมือใด (blinded) ประเมินผล
- กลุ่มไดโอดมีคะแนนเยื่อบุผิว (epithelial score) สูงที่สุด และคะแนนความสม่ำเสมอของแนวตัด (regularity score) แย่ที่สุดในบรรดาเครื่องมือทั้ง 6 ชนิด
- **ไม่พบข้อจำกัดในการวินิจฉัยทางพยาธิวิทยาในทุกกรณี ไม่ว่าจะใช้เครื่องมือใด**
- ไม่มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์ และไม่มีการรายงานความเร็วตัดสำหรับเครื่องมือใดเลย
- เกณฑ์การประเมินทางจุลพยาธิวิทยาที่ใช้ในบทความนี้ระบุไว้ชัดเจนว่ายืมมาจาก Vescovi et al. 2010

## Related notes

- Literature: [[02 Literature/10.4317/medoral.22819]]
- Data: [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data]] (source of this paper's evaluation criteria), [[07 Data/Azevedo et al 2016 - Diode Laser Thermal Damage and Carbonization Data]] (same LITEMEDICS device manufacturer)
- Evidence: [[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Power Output and Tissue Effect]]
- Synthesis: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
- Project: [[01 Projects/Diode Laser Biopsy]]
