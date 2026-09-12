# Diode Laser Biopsy

Companion project to [[01 Projects/Diode Laser Master]]. Extends this vault's existing power-output/power-loss research toward a biopsy specimen-quality outcome; it does not replace or duplicate that research, and no existing output/power-loss notes were altered to create this project.

## Scope

Dental/oral soft-tissue biopsy performed with diode lasers, focusing on how the device's preset power, actual delivered output, and operating parameters propagate through to tissue interaction and, ultimately, to the histopathologic/diagnostic quality of the excised specimen.

## Main research question

How do diode laser operating parameters and actual delivered power affect histopathologic quality of oral soft-tissue biopsy specimens?

## Subquestions

- Does the gap between set/preset power and measured/delivered output — already established in [[04 Evidence/Set Power vs Measured Output]] and [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]] — translate into a measurable difference in tissue thermal effect?
- Which operating parameters (power/power density, CW vs. pulsed mode, contact vs. non-contact, incision speed, fiber-tip initiation status) are reported to affect thermal damage zone width, coagulation, or carbonization at the specimen margin?
- At what specimen size and/or thermal-damage extent does histopathologic diagnosis become unreliable or unachievable?
- Does any dental-diode source measure delivered power (via calibrated power meter) and biopsy specimen histologic outcome in the same study? Current answer per vault evidence to date: no — see [[04 Evidence/Power Output and Tissue Effect]].

## Logic chain

Device preset → actual delivered output → operating parameters → tissue interaction → biopsy specimen quality

The first two links are covered by this vault's existing core evidence ([[04 Evidence/Set Power vs Measured Output]], [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]]); this project tracks the remaining links.

## Relevant concepts

- Reused, evidence-grounded: [[03 Concepts/Power Output]], [[03 Concepts/Power Loss]], [[03 Concepts/Operating Parameters]], [[03 Concepts/Laser Presetting]]
- New (this project): [[03 Concepts/Glossary/Histological Artifact]], [[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Coagulation Zone]], [[03 Concepts/Glossary/Carbonization]], [[03 Concepts/Glossary/Incision Speed]], [[03 Concepts/Glossary/Specimen Margin]], [[03 Concepts/Glossary/Diagnostic Quality]]

## Current evidence

- [[04 Evidence/Biopsy Specimen Quality]] — PARTIAL EVIDENCE (Angiero et al. 2011, Romeo et al. 2014, Gambino et al. 2026 processed: three real diagnostic-yield outcomes now in vault, all mutually consistent)
- [[04 Evidence/Thermal Artifact]] — PARTIAL EVIDENCE (Angiero et al. 2011, Azevedo et al. 2016, Gambino et al. 2026 processed: direct dental-diode thermal-damage/carbonization measurements)
- [[04 Evidence/Surgical Margins]] — PARTIAL EVIDENCE (Angiero et al. 2011, Romeo et al. 2014, Azevedo et al. 2016, Gambino et al. 2026 all processed)
- [[04 Evidence/Power Output and Tissue Effect]] — still NEEDS EVIDENCE (the central bridge node); all four processed papers report set power only, reinforcing rather than closing this gap
- [[06 Synthesis/Diode Laser Biopsy Specimen Quality]] — PROVISIONAL synthesis of the four processed biopsy sources; confirmed Capodiferro et al. 2008 still has no full-text literature note in `02 Literature/` and was not processed in this pass
- Reused background (already in vault, not created by this task): [[04 Evidence/Tip Initiation and Fiber Condition - Supporting Evidence]] — contains Gutiérrez-Corrales et al. 2020's explicit conclusion that an 810 nm diode laser at 0.5–2 W was the wavelength/power combination least likely to cause thermal damage to peri-incisional margins "for oral soft-tissue biopsy."

## Processed papers

All four papers below were added to `02 Literature/` via Zotero/ZotLit on 2026-09-12, which also provided full-text PDF/HTML access (via local Zotero cache) superseding this vault's earlier abstract-only or PMC-API-only extractions for Angiero, Romeo, and Azevedo. The Zotero-managed notes (title/DOI-keyed, `%%zt-managed%%` blocks preserved) are now the canonical literature notes; each carries an appended "## Vault processing" section linking to its Data extraction.

- Angiero F, et al. 2011 (*Lasers Med Sci* 2012;27:383-8; PubMed-indexed year 2011) — [[02 Literature/10.1007/s10103-011-0900-7]] / [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]] — full text (upgraded from abstract-only)
- Romeo U, et al. 2014 — [[02 Literature/Biopsy of Different Oral Soft Tissues Lesions by KTP and Diode Laser_ Histological Evaluation - Romeo - 2014 - The Scientific World Journal - Wiley Online Library]] / [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data]] — full text, now with per-patient tables (upgraded from PMC-API extraction)
- Azevedo AS, et al. 2016 — [[02 Literature/10.4317/jced.52830]] / [[07 Data/Azevedo et al 2016 - Diode Laser Thermal Damage and Carbonization Data]] — full text, now with actual table cell values (upgraded from PMC-API extraction)
- Gambino A, et al. 2026 — [[02 Literature/10.3390/dj14030168]] / [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data]] — full text, newly processed (previously an unprocessed candidate below)

This vault's earlier manually-created literature notes for Angiero, Romeo, and Azevedo (created before the Zotero import) are marked superseded in-place, not deleted; see each note's banner.

## Research gaps

- CONFIRMED (inherited from [[06 Synthesis/Research Gaps in Dental Diode Laser Output]]): no source pairs controlled tip-initiation status with an independently measured, calibrated power-meter output value.
- CONFIRMED (updated after processing): no source in this vault pairs a calibrated, independently measured dental-diode power value with a histologically assessed biopsy specimen outcome (thermal damage zone, coagulation, carbonization, diagnostic yield) in the same study — now confirmed across all four processed full-data sources (Angiero et al. 2011, Romeo et al. 2014, Azevedo et al. 2016, Gambino et al. 2026), which all report set/console power only.
- CONFIRMED: no source in this vault reports incision speed as an independently varied variable against specimen histologic quality; none of the four processed papers reports incision speed at all.
- CONFIRMED (updated after processing): specimen size/margin, not power, is the variable consistently associated with diagnostic yield across three independent sources — Angiero et al. 2011 (size-graded: 2mm 63.63% failure, 3mm 37.71%, ≥4mm 0%), Romeo et al. 2014 (5–10mm lesions, 0% failure), and Gambino et al. 2026 (standardized 5mm margin, 0% failure) all converge on a ≥4–5mm threshold, independently arrived at. No source varies power while holding specimen size constant, or vice versa, to isolate the two variables — this remains open.
- PARTIALLY NARROWED: coagulation-zone evidence — Capodiferro et al. 2008 remains the only identified candidate that *scores* a coagulation zone for a dental diode laser, and remains unprocessed. However, Angiero et al. 2011 and Gambino et al. 2026 (both now processed) each describe coagulation-related histologic findings qualitatively (clotted/thrombosed vessels; basophilic hemocoagulative changes) without isolating them as a scored variable — see [[03 Concepts/Glossary/Coagulation Zone]].
- RESOLVED: whether dental-diode-specific thermal-artifact and specimen-margin measurements exist at all — yes, now confirmed by four independent processed sources. What remains unresolved is linking any of these to a *measured* (as opposed to set) power value.
- NEW (from Gambino et al. 2026): a real untreated-control-group comparison now exists for the first time in this vault's biopsy evidence, showing laser-treated tissue is statistically significantly thicker than healthy tissue even when diagnosis is unimpaired — this sharpens "thermal artifact does not equal diagnostic failure" from an assumption into a directly tested finding, but only at one fixed power/margin combination.

## Papers to search next

Status: unprocessed. The candidates below are abstract-level review only; no literature or data-extraction notes have been created for these yet — they follow the same "identified, not yet processed" convention already used in [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]. According to PubMed, the following remain the next-highest-priority candidates:

1. Capodiferro S, Maiorano E, Loiudice AM, Scarpelli F, Favia G. "Oral laser surgical pathology: a preliminary study on the clinical advantages of diode laser and on the histopathological features of specimens evaluated by conventional and confocal laser scanning microscopy." *Minerva Stomatol.* 2008;57(1-2):1-6. PMID: 18427366. (No DOI in source record.) Why flagged: n=25, diode 2–7 W; states coagulation of proteins present "only with high power density output" — directly on the power→tissue-effect link and the only identified candidate specific to [[03 Concepts/Glossary/Coagulation Zone]]. Caveat: preliminary study, abstract-level only, power appears set/nominal rather than independently measured.
2. Gundlapalle P, Nagappan N, Ramesh P, Ziauddhin S, Karthick BP, Paleti VSM, Kumar BV. "Comparison of Oral Mucosal Biopsies Done Using Scalpel and Diode Lasers: A Vivo Study." *J Pharm Bioallied Sci.* 2022;14(Suppl 1):S947-S954. PMID: 36110647. DOI: [10.4103/jpbs.jpbs_861_21](https://doi.org/10.4103/jpbs.jpbs_861_21). Why flagged: n=60 (30 scalpel/30 diode, split CW/pulsed); pathologist-noted "peripheral tissue damage and artifacts" per slide; pulsed mode reported advantageous over CW for thermal damage — would add a CW-vs-pulsed comparison this vault's biopsy evidence currently lacks. Caveat: abstract does not report a measured/verified output value distinct from the 3 W panel setting.
3. Suter VGA, Altermatt HJ, Sendi P, Mettraux G, Bornstein MM. "CO2 and diode laser for excisional biopsies of oral mucosal lesions. A pilot study evaluating clinical and histopathological parameters." *Schweiz Monatsschr Zahnmed.* 2010;120(8):664-71. PMID: 21038754. (No DOI in source record.) Why flagged: pilot RCT; quantifies thermal damage zone (μm and histopathological index) for diode (5.12 W pulsed) vs. two CO2 settings; found the diode's damage zone significantly larger than CO2's. Caveat: pilot scale (15 patients), abstract-level only. Also cited within Azevedo et al. 2016's own reference list (ref. 11–12), confirming its relevance independently.

Not shortlisted (lower relevance — clinical case reports/series confirming histopathologic diagnosis of specific benign lesions after diode excision, without a thermal-damage or margin-quality measurement): PMIDs 38029573, 40098816, 33425306, 41789289, 38274320, 25653822, 41382959, 42109937, 20050982.

## Related notes

- [[01 Projects/Diode Laser Master]]
- [[06 Synthesis/Research Gaps in Dental Diode Laser Output]]
- [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]

## สรุปภาษาไทย

- โครงการนี้เป็นโครงการคู่ขนานกับ [[01 Projects/Diode Laser Master]] มุ่งขยายงานวิจัยเรื่องกำลังขาออก/การสูญเสียกำลังที่มีอยู่แล้วในคลังนี้ ไปสู่คำถามเรื่องคุณภาพชิ้นเนื้อ biopsy โดยไม่ลบหรือแก้ไขงานวิจัยเดิม
- คำถามวิจัยหลัก: พารามิเตอร์การทำงานของเลเซอร์ไดโอดและกำลังขาออกที่ส่งจริง ส่งผลต่อคุณภาพทางจุลพยาธิวิทยาของชิ้นเนื้อ biopsy เนื้อเยื่ออ่อนในช่องปากอย่างไร
- ห่วงโซ่ตรรกะหลัก: ค่าตั้งเครื่อง → กำลังขาออกที่ส่งจริง → พารามิเตอร์การทำงาน → ปฏิกิริยาต่อเนื้อเยื่อ → คุณภาพชิ้นเนื้อ biopsy
- อัปเดต 2026-09-12 (รอบแรก): ประมวลผลบทความ 3 ฉบับแรกจากบทคัดย่อ/PMC API — Angiero et al. 2011, Romeo et al. 2014, Azevedo et al. 2016
- อัปเดต 2026-09-12 (รอบสอง): ทั้ง 4 บทความ (Angiero, Romeo, Azevedo, และ Gambino et al. 2026 ที่เพิ่มเข้ามาใหม่) ถูกนำเข้าคลัง Zotero/ZotLit พร้อมไฟล์ PDF/HTML ฉบับเต็ม ทำให้สามารถประมวลผลจากเนื้อหาฉบับเต็มได้ละเอียดขึ้นมาก — Angiero et al. (จากบทคัดย่ออย่างเดียว → ฉบับเต็ม พบตาราง 5 ที่แยกอัตราวินิจฉัยไม่ได้ตามขนาดชิ้นเนื้อ: 2มม.=63.63%, 3มม.=37.71%, ≥4มม.=0%), Romeo et al. (พบข้อมูลรายผู้ป่วยแยกตามอุปกรณ์), Azevedo et al. (พบค่าคะแนนการไหม้เป็นถ่านของไดโอดจริง: 2.50 ที่ 3.5W PW, 1.80 ที่ 3.5W Boost — ต่ำกว่าทั้งที่ ETTD สูงกว่า), และ Gambino et al. 2026 (n=30, วินิจฉัยได้ 100% ที่ขอบตัดมาตรฐาน 5มม. แม้เนื้อเยื่อหนาขึ้นอย่างมีนัยสำคัญทางสถิติเทียบกับกลุ่มควบคุม)
- หลักฐาน 3 รายการ ([[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Thermal Artifact]], [[04 Evidence/Surgical Margins]]) อัปเกรดเป็น PARTIAL EVIDENCE ที่มั่นคงขึ้น โดยมีแหล่งข้อมูลอิสระ 3-4 รายการสอดคล้องกันว่าขนาดชิ้นเนื้อ/ขอบตัด ≥4-5 มม. คือตัวแปรสำคัญต่อผลการวินิจฉัย
- อย่างไรก็ตาม [[04 Evidence/Power Output and Tissue Effect]] ยังคงเป็น **PLACEHOLDER (ยังต้องการหลักฐานเพิ่มเติม)** เนื่องจากทั้ง 4 บทความใช้ค่ากำลังที่ตั้ง (set power) เท่านั้น ไม่มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์คู่กับผลทางเนื้อเยื่อ/การวินิจฉัยเลย
- บันทึกวรรณกรรมที่สร้างด้วยมือในรอบแรก (ก่อนมี Zotero) ถูกทำเครื่องหมาย "SUPERSEDED" ไว้ในไฟล์เดิม ไม่ได้ลบทิ้ง เพื่อรักษาความโปร่งใสของประวัติการแก้ไข
- ยังเหลือบทความที่เกี่ยวข้อง 3 รายการที่ยังไม่ได้ประมวลผล (Capodiferro et al., Gundlapalle et al., Suter et al.) — ดูหัวข้อ "Papers to search next"
- ไม่มีการอนุมานข้อสรุปทางคลินิกใด ๆ ในบันทึกนี้
