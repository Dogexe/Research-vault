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

- [[04 Evidence/Biopsy Specimen Quality]] — PARTIAL EVIDENCE (Angiero et al. 2011 + Romeo et al. 2014 processed: real diagnostic-yield outcomes now in vault)
- [[04 Evidence/Thermal Artifact]] — PARTIAL EVIDENCE (Azevedo et al. 2016 processed: direct dental-diode ETTD/carbonization measurement)
- [[04 Evidence/Surgical Margins]] — PARTIAL EVIDENCE (Angiero et al. 2011, Romeo et al. 2014, Azevedo et al. 2016 all processed)
- [[04 Evidence/Power Output and Tissue Effect]] — still NEEDS EVIDENCE (the central bridge node); all three newly processed papers report set power only, reinforcing rather than closing this gap
- Reused background (already in vault, not created by this task): [[04 Evidence/Tip Initiation and Fiber Condition - Supporting Evidence]] — contains Gutiérrez-Corrales et al. 2020's explicit conclusion that an 810 nm diode laser at 0.5–2 W was the wavelength/power combination least likely to cause thermal damage to peri-incisional margins "for oral soft-tissue biopsy."

## Processed papers (2026-09-12)

- Angiero F, et al. 2011 — [[02 Literature/Angiero et al 2011 - Diode Laser Applied to Oral Soft Tissue Lesions]] / [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]] — abstract-only (no PMCID available)
- Romeo U, et al. 2014 — [[02 Literature/Romeo et al 2014 - Biopsy of Oral Soft Tissue Lesions by KTP and Diode Laser]] / [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data]] — full text
- Azevedo AS, et al. 2016 — [[02 Literature/Azevedo et al 2016 - Surgical Margins by Different Laser Wavelengths in Tongue Tissue]] / [[07 Data/Azevedo et al 2016 - Diode Laser Thermal Damage and Carbonization Data]] — full text

## Research gaps

- CONFIRMED (inherited from [[06 Synthesis/Research Gaps in Dental Diode Laser Output]]): no source pairs controlled tip-initiation status with an independently measured, calibrated power-meter output value.
- CONFIRMED (updated after processing): no source in this vault pairs a calibrated, independently measured dental-diode power value with a histologically assessed biopsy specimen outcome (thermal damage zone, coagulation, carbonization, diagnostic yield) in the same study — now confirmed across all three newly processed full-data sources (Angiero et al. 2011, Romeo et al. 2014, Azevedo et al. 2016), which all report set/console power only.
- CONFIRMED: no source in this vault reports incision speed as an independently varied variable against specimen histologic quality; none of the three newly processed papers reports incision speed at all.
- NEW: no source in this vault has yet isolated specimen size from power/operating-parameter choice as independent variables — Angiero et al. 2011 and Romeo et al. 2014 together suggest specimen size (relative to the thermal-alteration zone) is associated with diagnostic yield, but neither varies power while holding specimen size constant, or vice versa.
- NEW: no source in this vault reports a coagulation-zone measurement for a dental diode laser (Capodiferro et al. 2008 remains the only identified, unprocessed candidate for this specific concept — see "Papers to search next").
- RESOLVED (partially): whether dental-diode-specific thermal-artifact and specimen-margin measurements exist at all — yes, now confirmed by Azevedo et al. 2016 (thermal artifact) and Angiero et al. 2011 / Romeo et al. 2014 (margins/diagnostic yield). What remains unresolved is linking any of these to a *measured* (as opposed to set) power value.

## Papers to search next

Status: unprocessed (Angiero et al. 2011, Romeo et al. 2014, and Azevedo et al. 2016 — previously listed here — were processed on 2026-09-12; see "Processed papers" above). The remaining candidates below are abstract-level review only; no literature or data-extraction notes have been created for these yet — they follow the same "identified, not yet processed" convention already used in [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]. According to PubMed, the following remain the next-highest-priority candidates:

1. Capodiferro S, Maiorano E, Loiudice AM, Scarpelli F, Favia G. "Oral laser surgical pathology: a preliminary study on the clinical advantages of diode laser and on the histopathological features of specimens evaluated by conventional and confocal laser scanning microscopy." *Minerva Stomatol.* 2008;57(1-2):1-6. PMID: 18427366. (No DOI in source record.) Why flagged: n=25, diode 2–7 W; states coagulation of proteins present "only with high power density output" — directly on the power→tissue-effect link and the only identified candidate specific to [[03 Concepts/Glossary/Coagulation Zone]]. Caveat: preliminary study, abstract-level only, power appears set/nominal rather than independently measured.
2. Gundlapalle P, Nagappan N, Ramesh P, Ziauddhin S, Karthick BP, Paleti VSM, Kumar BV. "Comparison of Oral Mucosal Biopsies Done Using Scalpel and Diode Lasers: A Vivo Study." *J Pharm Bioallied Sci.* 2022;14(Suppl 1):S947-S954. PMID: 36110647. DOI: [10.4103/jpbs.jpbs_861_21](https://doi.org/10.4103/jpbs.jpbs_861_21). Why flagged: n=60 (30 scalpel/30 diode, split CW/pulsed); pathologist-noted "peripheral tissue damage and artifacts" per slide; pulsed mode reported advantageous over CW for thermal damage — would add a CW-vs-pulsed comparison this vault's biopsy evidence currently lacks. Caveat: abstract does not report a measured/verified output value distinct from the 3 W panel setting.
3. Gambino A, Magliano A, Haddad GE, Bezzi M, Cafaro A, Karimi D, Broccoletti R, Arduino PG. "Optical Coherence Tomography (OCT) Evaluation of Thermal Tissue Alterations After Diode Laser Excision of Oral Leukoplakia (OL)." *Dent J (Basel).* 2026;14(3):168. PMID: 41892776. DOI: [10.3390/dj14030168](https://doi.org/10.3390/dj14030168). Why flagged: n=30 (15 diode 980 nm CW contact/15 scalpel); quantifies epithelial (288.9 μm) and connective-tissue (430.3 μm) thermal alteration; reports diagnosis was not impaired in any specimen — the most recent and most directly quantitative source found, and would add a second full diagnostic-yield source at a standardized margin. Caveat: single-center, abstract-level only, standardized 5 mm margin protocol (not a variable-power study).
4. Suter VGA, Altermatt HJ, Sendi P, Mettraux G, Bornstein MM. "CO2 and diode laser for excisional biopsies of oral mucosal lesions. A pilot study evaluating clinical and histopathological parameters." *Schweiz Monatsschr Zahnmed.* 2010;120(8):664-71. PMID: 21038754. (No DOI in source record.) Why flagged: pilot RCT; quantifies thermal damage zone (μm and histopathological index) for diode (5.12 W pulsed) vs. two CO2 settings; found the diode's damage zone significantly larger than CO2's. Caveat: pilot scale (15 patients), abstract-level only.

Not shortlisted (lower relevance — clinical case reports/series confirming histopathologic diagnosis of specific benign lesions after diode excision, without a thermal-damage or margin-quality measurement): PMIDs 38029573, 40098816, 33425306, 41789289, 38274320, 25653822, 41382959, 42109937, 20050982.

## Related notes

- [[01 Projects/Diode Laser Master]]
- [[06 Synthesis/Research Gaps in Dental Diode Laser Output]]
- [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]

## สรุปภาษาไทย

- โครงการนี้เป็นโครงการคู่ขนานกับ [[01 Projects/Diode Laser Master]] มุ่งขยายงานวิจัยเรื่องกำลังขาออก/การสูญเสียกำลังที่มีอยู่แล้วในคลังนี้ ไปสู่คำถามเรื่องคุณภาพชิ้นเนื้อ biopsy โดยไม่ลบหรือแก้ไขงานวิจัยเดิม
- คำถามวิจัยหลัก: พารามิเตอร์การทำงานของเลเซอร์ไดโอดและกำลังขาออกที่ส่งจริง ส่งผลต่อคุณภาพทางจุลพยาธิวิทยาของชิ้นเนื้อ biopsy เนื้อเยื่ออ่อนในช่องปากอย่างไร
- ห่วงโซ่ตรรกะหลัก: ค่าตั้งเครื่อง → กำลังขาออกที่ส่งจริง → พารามิเตอร์การทำงาน → ปฏิกิริยาต่อเนื้อเยื่อ → คุณภาพชิ้นเนื้อ biopsy
- อัปเดต 2026-09-12: ประมวลผลบทความ 3 ฉบับแรกแล้ว — Angiero et al. 2011 (n=608, วินิจฉัยไม่ได้ 46.15% ในชิ้นเนื้อ <3มม.), Romeo et al. 2014 (n=17, วินิจฉัยได้ 100%, วัดความเสียหายขอบ 0.149–0.473 มม.), Azevedo et al. 2016 (วัด ETTD ของไดโอด 980nm = 456–627 ไมโครเมตร, สัมพันธ์กับการไหม้เป็นถ่าน) หลักฐาน 3 รายการ ([[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Thermal Artifact]], [[04 Evidence/Surgical Margins]]) จึงอัปเกรดจาก PLACEHOLDER เป็น PARTIAL EVIDENCE
- อย่างไรก็ตาม [[04 Evidence/Power Output and Tissue Effect]] ยังคงเป็น **PLACEHOLDER (ยังต้องการหลักฐานเพิ่มเติม)** เนื่องจากทั้ง 3 บทความที่ประมวลผลแล้วใช้ค่ากำลังที่ตั้ง (set power) เท่านั้น ไม่มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์คู่กับผลทางเนื้อเยื่อ/การวินิจฉัยเลย
- ยังเหลือบทความที่เกี่ยวข้อง 4 รายการที่ยังไม่ได้ประมวลผล (Capodiferro et al., Gundlapalle et al., Suter et al., Gambino et al.) — ดูหัวข้อ "Papers to search next"
- ไม่มีการอนุมานข้อสรุปทางคลินิกใด ๆ ในบันทึกนี้
