---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: false
wavelength_nm: [10600, 2940]
set_power_w: [4.62, 7]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: "unknown"
cw_pw: "PW"
fiber_diameter_um: 400
tip_initiation: null
contact_mode: "non-contact"
histology: true
thermal_damage: true
margin_quality: "quantified (thermal damage zone width, μm, minima/maxima measured per specimen by a blinded pathologist); CO2 (140 Hz, 400 μs, 33 mJ, 4.62 W): median of all maxima 74.9 μm (49.9–122.6), median of all minima 27.2 μm (18.2–49.9); Er:YAG (35 Hz, 297 μs, 200 mJ, 7 W): median of all maxima 34.0 μm (18.2–59.0), median of all minima 4.5 μm (12.5–22.7 IQR as reported); pooled median all values 54.5 μm overall; Er:YAG significantly thinner than CO2 in both maxima and minima (p<0.0001)"
tissue_architecture: "qualitative (not scored numerically); CO2 specimens showed 'groups of blisters' in the thermally damaged tissue with a more precise linear cut; Er:YAG specimens showed a 'cratered surface' from microexplosions (thermomechanical/photomechanical effect) but more compact, unaltered adjacent tissue and less regular cut geometry"
specimen_interpretability: "1 of 32 specimens (CO2 group) excluded from the thermal-damage-zone measurement because the zone 'could not be identified adequately' — this exclusion is scoped by the source to the thermal-damage-zone submeasurement specifically; the source does not separately state whether the underlying histologic diagnosis (fibrous hyperplasia) was still confirmable for that excluded specimen, so a diagnostic-failure claim for this case is NOT ESTABLISHED, only a measurement/readability limitation for one specific outcome variable"
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: CORE BIOPSY — NOT a diode laser.** CO2 and Er:YAG are both non-diode systems; `diode_laser: false` is deliberate and confirmed. This is a **randomized controlled trial** (genuine computer-generated block randomization, `www.randomization.com`) directly and exclusively comparing CO2 vs. Er:YAG for excisional biopsy of a single, controlled lesion type (fibrous hyperplasia, buccal mucosa only) — a cleaner two-arm design than [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data|Monteiro et al. 2019]]'s six-arm retrospective comparison, which includes both CO2 and Er:YAG among its arms but was not purpose-built or randomized for a CO2-vs-Er:YAG comparison specifically.

**Disambiguation note:** this is a **different paper** from [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)|Suter et al. 2010]] (same senior-author group — Suter, Altermatt, Bornstein — publishing a continuing research program on excisional-biopsy laser comparisons). The 2010 paper compares CO2 vs. **diode**; this 2017 paper compares CO2 vs. **Er:YAG**. Do not conflate the two.

**Manufacturer-preset provenance note (relevant to [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]], though that synthesis note's update scope in this task is restricted to Parker et al. 2024 — this finding is preserved here as a citable data point for a future preset-reliability update):** the paper's own Discussion states explicitly, "The settings used in the present study were chosen according to the **manufacturer's recommendation for soft tissue biopsy**" (referring to the Er:YAG LiteTouch™ device's biopsy-mode preset: 35 Hz, 297 μs, 200 mJ → 7 W). This is the clearest explicit author-stated instance found anywhere in this vault of a primary study following a **named manufacturer soft-tissue-biopsy preset**, with the resulting histologic outcome (thermal damage zone) independently measured by a blinded pathologist.

## Source

- Literature note: [[02 Literature/10.1007/s10103-017-2151-8]]
- Source link: https://doi.org/10.1007/s10103-017-2151-8
- Source locator: Full text (`pdftotext` extraction of the Zotero-attached PDF) — Abstract; Introduction; Materials and methods; Results; Tables 1–4; Discussion; Conclusions.

## Extraction

| Parameter | Group 1: CO2 laser | Group 2: Er:YAG laser | Evidence status |
| --- | --- | --- | --- |
| Device | Spectra DENTA Surgical Carbon Dioxide Laser, MAX Engineering Ltd., Gyeonggi-Do, South Korea | LiteTouch™, Synergon Dental Lasers, Light Instruments Ltd., Yokneam Elite, Israel | FACT |
| Wavelength | 10,600 nm (10.6 μm) | 2940 nm | FACT |
| Mode | Char-free (pulsed) mode | Soft tissue biopsy mode, air-water cooling (22.5 mL/min) | FACT |
| Frequency | 140 Hz | 35 Hz | FACT |
| Pulse duration | 400 μs | 297 μs | FACT |
| Pulse energy | 33 mJ | 200 mJ | FACT |
| Resulting power | 4.62 W (calculated from pulse energy × frequency, not independently power-meter-verified) | 7 W (calculated from pulse energy × frequency, not independently power-meter-verified) | FACT |
| Setting provenance | Not stated as manufacturer-recommended in the text | **Explicitly stated: "chosen according to the manufacturer's recommendation for soft tissue biopsy"** | FACT |
| Delivery system | Articulated mirror arm, straight handpiece; spot size 0.2 mm | 400 μm diameter cylindrical sapphire tip | FACT |
| Contact mode | Non-contact (1–2 mm distance to mucosa) | Non-contact (no contact to tissue stated) | FACT |
| Independently measured power | NO — no power meter or independent verification step described anywhere in Methods | NO | FACT (absence confirmed) |
| Incision speed | NOT REPORTED — no mm/s value or speed-control description; only total excision duration (stopwatch) is timed | NOT REPORTED | FACT (absence) |
| n (surgical, all patients) | 16 | 16 | FACT |
| n (histopathological evaluation) | 15 (1 excluded — thermal damage zone unmeasurable) | 16 | FACT |
| Sample / lesion | Fibrous hyperplasia, buccal mucosa, minimal dimension 5 mm, max 20 mm | (same criteria, same lesion type/site) | FACT |
| Surgeon | Single experienced oral surgeon (V.S.) for all cases, both arms | (same) | FACT |
| Duration of excision (median, s) | 158.5 (IQR 103.5–243.8) | 201.0 (IQR 165.8–259.5); overall median all cases 209 s; no significant between-group difference (p=0.1188) | FACT |
| Intraoperative bleeding | 9/16 (56%) | 16/16 (100%); significantly more than CO2 (p=0.0068/p=0.0155 as separately reported for bleeding vs. electrocauter need) | FACT |
| Need for electrocauterization | 8/16 (50%) | 15/16 (94%) | FACT |
| Need for sutures | 0/16 | 1/16 | FACT |
| Postoperative pain, day 1 (median VAS 0–100) | 5.0 (IQR 0.0–19.2) | 3.0 (IQR 0.0–11.8) | FACT |
| Analgesic use | Low overall (<10% of all patients); no significant between-group difference reported | (same) | FACT |
| Pathologist | One experienced pathologist (H.J.A.), blinded to laser type used, not involved in primary diagnosis | (same, shared assessor across both groups) | FACT |
| Thermal damage zone — median of all maxima (μm) | 74.9 (IQR 49.9–122.6) | 34.0 (IQR 18.2–59.0); significantly lower than CO2 (p<0.0001) | FACT |
| Thermal damage zone — median of all minima (μm) | 27.2 (49.9 IQR upper as tabulated; see source Table 3 for exact IQR pairing) | 4.5 (18.2–22.7 IQR as tabulated) | FACT |
| Specimens excluded from thermal-damage measurement | 1 of 16 ("thermal damage zone could not be identified adequately") | 0 of 16 | FACT |
| Histologic diagnosis confirmed (fibrous hyperplasia) | Purpose of evaluation for all submitted specimens; explicit per-specimen confirmation count not separately tabulated | (same) | FACT (purpose stated); NOT ESTABLISHED (explicit per-specimen count) |

## Study design (per task's Section A)

- Human, in vivo, prospective RCT (Department of Oral Surgery and Stomatology, University of Bern, Switzerland; June 2013–December 2015; ethics-approved, KEK-BE: 203/12).
- **True diagnostic/excisional biopsy pathway**: real fibrous hyperplasia lesions, buccal mucosa only, histological evaluation performed to confirm diagnosis and measure thermal damage zone.
- Comparator groups: 2 arms only, CO2 vs. Er:YAG — no scalpel/cold-knife arm (explicitly noted by the authors as a limitation: "a control group including scalpel [is] necessary to confirm these findings").
- Sample size: n=32 patients enrolled and randomized (16/16); n=31 specimens available for the thermal-damage-zone histopathological outcome (15 CO2/16 Er:YAG).
- Tissue/site: buccal mucosa only (17 left, 15 right) — single anatomic subsite, a deliberate control for site variability.

## Histopathology methodology (per task's Section C)

- Fixation: 4% buffered formalin; paraffin-embedded; 5 μm sections; H&E stain.
- **Pathologist involvement: one experienced pathologist (H.J.A.)**, explicitly stated **not involved in the primary diagnosis of the specimens** and **blinded to the type of laser used**.
- Number of assessors: 1. NOT a multi-pathologist consensus design (contrast with Seoane et al. 2013's two-pathologist consensus).
- Inter-rater reliability: NOT REPORTED (single assessor, not applicable).
- Measurement: maximal and minimal thermal damage measured in micrometres on a representative section on both lateral edges of the fibrous hyperplasia, adjacent to the epithelium.

## Outcome terminology (author's exact wording, per task's Section D)

- **"Thermal damage zone"** / **"width of the thermal damage zone"** — the paper's own primary-outcome phrase (μm), reported as maxima and minima per specimen, then pooled medians by group.
- **"Not included in the histopathological evaluation"** — the source's own phrase for the one excluded CO2-group specimen, scoped explicitly to the thermal-damage-zone measurement ("because the thermal damage zone could not be identified adequately"), not phrased by the source as a diagnostic failure.
- No "pseudodysplastic" or artifact-specific vocabulary is used in this paper (contrast with Seoane 2013) — findings are framed purely as thermal damage zone width and qualitative morphology (blisters vs. cratered surface).

## Outcome type (per task's Section E)

| Outcome | Type | Unit/range | Epithelial component? | CT component? | Margin-specific? | Architecture-specific? | Diagnosis affected? | Adequacy/readability judgment? |
|---|---|---|---|---|---|---|---|---|
| Thermal damage zone (μm) | Quantitative continuous | μm, median/IQR, maxima and minima, by group | No — not separated into epithelial vs. connective-tissue compartments; a single measurement per specimen edge | No (same) | Yes (adjacent to epithelium, at the specimen edge) | No | No | No |
| Qualitative morphology (blisters vs. cratered surface) | Descriptive, not scored | N/A | Implied (blisters described at epithelium) | Not separately addressed | Yes (cut-interface description) | Yes | No | No |
| Excluded specimen (n=1, CO2) | Count/categorical, whole-cohort | 1/16 CO2, 0/16 Er:YAG | — | — | Indirect (a margin-measurement limitation) | — | NOT ESTABLISHED (not stated either way for this case) | Partial — a measurement-adequacy limitation for the thermal-damage-zone outcome specifically, distinct from a diagnostic-adequacy limitation |
| Clinical secondary outcomes (bleeding, electrocauter/sutures, pain, duration) | Quantitative/categorical, by group | See Extraction table | — | — | — | — | — | — |

**Per the task's explicit instruction not to collapse outcomes into one category:** this study evaluates **tissue damage** (thermal damage zone, quantitative) and, separately and more weakly, **specimen readability for that one outcome measure** (the single excluded specimen). It does **not** report a formal, scored **biopsy-margin-quality** construct (no ordinal margin score, unlike Monteiro 2019/Vescovi 2010's 0–4 incision-regularity scores), does **not** report a distinct **diagnostic-interpretability** judgment beyond stating the purpose of evaluation, and does **not** report a **diagnostic failure** for any specimen (the one exclusion is scoped to the thermal-damage submeasure only, with the underlying diagnostic status of that specimen left unstated).

## Score/grading details (per task's Section F)

- **No formal ordinal score is used** in this paper — thermal damage zone is a direct μm measurement (maxima/minima), and the CO2-vs-Er:YAG morphological difference (blisters vs. cratered surface) is described qualitatively in the Discussion, not scored numerically.
- Score name: N/A.
- Validation status: N/A.
- Blinded: YES (single pathologist).
- Number of scorers: 1.
- Reliability statistic: NOT REPORTED.

## Comparison against existing vault CORE BIOPSY sources (Gobbo 2017, Monteiro 2019, Seoane 2013, Vescovi 2010, Gundlapalle 2022)

- **Laser comparison uniqueness**: none of the five studies performs a purpose-built, randomized, two-arm-only **CO2-vs-Er:YAG** comparison for excisional biopsy. Monteiro 2019 includes both lasers among six retrospective (non-randomized) arms; the others do not include both lasers at all (Gobbo: diode vs. electrosurgery; Seoane: Er,Cr:YSGG single-arm; Vescovi: Nd:YAG vs. scalpel; Gundlapalle: diode CW vs. PW vs. scalpel).
- **Manufacturer-preset provenance**: this is the only one of the six studies (five existing + this one) where the paper's own text explicitly states its laser settings were drawn from **the manufacturer's stated recommendation for soft tissue biopsy** — a directly relevant, author-attributed preset-to-histologic-outcome data point not present in the other five extraction notes as read.
- **Secondary clinical outcomes**: this paper is the richest of the six for non-histologic clinical tradeoffs specific to a laser-vs-laser (not laser-vs-scalpel) comparison — quantified intraoperative bleeding, electrocauter/suture need, and 15-day VAS pain trajectory, isolated cleanly to the CO2-vs-Er:YAG contrast because of the two-arm randomized design.
- **Specimen-exclusion framing**: similar in kind to Gobbo 2017's "not measurable but diagnosis unaffected" finding, but weaker in documentation — Gobbo, Monteiro, and Vescovi all explicitly state diagnosis was unaffected in every case (including unmeasurable ones); this paper does not make that same explicit statement for its one excluded specimen, leaving that specimen's diagnostic status genuinely unreported rather than confirmed-adequate.
- **Wavelength-specific trend reinforcement**: Er:YAG's lower thermal damage relative to CO2 here is directionally consistent with Monteiro 2019 (Er:YAG lowest epithelial/connective TDE of five active instruments) and the existing vault's older Suter et al. 2010 finding — three independent datasets now converge on Er:YAG (or the lowest-thermal-effect modality tested) producing less thermal margin alteration than CO2, though via different study designs and without a shared statistical pooling.

## Notes

- FACT: This is the vault's first RCT-level, two-arm-only CO2-vs-Er:YAG excisional-biopsy comparison, with genuine computer-generated randomization, a single controlled lesion type/site, and a blinded pathologist.
- FACT: The paper explicitly attributes its Er:YAG settings to "the manufacturer's recommendation for soft tissue biopsy" — see the provenance note above. This is flagged here as a citable data point for the vault's ongoing preset-reliability thread, but per this task's explicit update-scope instruction, it does **not** itself trigger an update to [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] in this pass (that update was scoped to Parker et al. 2024 only).
- FACT: Independently measures no power (both values are calculated from pulse energy × frequency, not power-meter-verified) and reports no incision speed for either arm — does not close this project's core measured-power + speed gap.
- NEEDS VERIFICATION flagged in YAML: (1) `fiber_diameter_um: 400` records only the Er:YAG sapphire tip diameter — the CO2 arm is mirror-delivered (articulated arm, 0.2 mm spot size), not fiber-delivered, so this field is scoped to the one arm where a fiber/tip diameter concept applies; a human should confirm this scoping choice is the intended reading given neither arm is a diode laser; (2) `diagnostic_outcome: true` records that histopathological evaluation was performed with diagnosis-confirmation as its stated purpose for all specimens, but the source does not explicitly confirm diagnosis was rendered for the one excluded (thermal-damage-unmeasurable) CO2 specimen — this is a genuine gap in the source, not an oversight in this extraction; (3) `wavelength_nm`/`set_power_w` list ordering follows this vault's [CO2, Er:YAG] convention matching the Extraction table's Group 1/Group 2 order.
- Classification for this vault: CORE BIOPSY, non-diode. Strengthens the RCT-level CO2-vs-Er:YAG comparison precedent and the manufacturer-preset-provenance evidence base; does not touch the diode-specific, measured-power, or incision-speed axes.

## สรุปภาษาไทย

- การศึกษานี้เป็น RCT สุ่มจริงในผู้ป่วย 32 ราย เปรียบเทียบเลเซอร์ CO2 กับ Er:YAG สำหรับการตัดชิ้นเนื้อ fibrous hyperplasia บริเวณกระพุ้งแก้ม โดยมีพยาธิแพทย์ 1 คนที่ปกปิดข้อมูลชนิดเลเซอร์ (blinded) วัดความเสียหายจากความร้อน
- Er:YAG มีความเสียหายจากความร้อนน้อยกว่า CO2 อย่างมีนัยสำคัญ (มัธยฐาน 34.0 เทียบกับ 74.9 ไมโครเมตร) แต่มีเลือดออกระหว่างผ่าตัดมากกว่า (100% เทียบกับ 56%)
- **บทความระบุตรงๆ ว่าค่าที่ตั้งของ Er:YAG (35Hz, 297μs, 200mJ) เลือกตาม "คำแนะนำของผู้ผลิตสำหรับการตัดชิ้นเนื้อเนื้อเยื่ออ่อน"** — เป็นตัวอย่างที่ชัดเจนที่สุดในคลังนี้ของการใช้ค่าพรีเซ็ตจากผู้ผลิตโดยตรงแล้ววัดผลทางจุลพยาธิวิทยาอย่างเป็นอิสระ
- มี 1 ใน 32 ตัวอย่าง (กลุ่ม CO2) ที่ไม่สามารถวัดโซนความเสียหายจากความร้อนได้ แต่บทความไม่ได้ระบุชัดว่าการวินิจฉัยของตัวอย่างนี้ยังทำได้หรือไม่ — จึงไม่ควรสรุปว่าเป็น "ความล้มเหลวในการวินิจฉัย"
- ไม่มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์ และไม่มีการรายงานความเร็วตัดสำหรับกลุ่มใดเลย

## Related notes

- Literature: [[02 Literature/10.1007/s10103-017-2151-8]]
- Data: [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)]] (same author group, different comparator laser), [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data]] (includes both CO2 and Er:YAG among six retrospective arms), [[07 Data/Gobbo et al 2017 - Blue vs Infrared Diode Laser Biopsy Thermal Damage Data]] (comparable specimen-exclusion-vs-diagnosis-unaffected pattern), [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data]], [[07 Data/Seoane et al 2013 - Er,Cr YSGG Leukoplakia Pseudodysplastic Artifact Data]], [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data]]
- Evidence: [[04 Evidence/Biopsy Specimen Quality]]
- Synthesis: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] (manufacturer-preset-provenance data point, not yet incorporated into that note's update scope)
- Project: [[01 Projects/Diode Laser Biopsy]]
