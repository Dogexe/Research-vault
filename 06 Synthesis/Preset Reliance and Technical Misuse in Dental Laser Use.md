# Preset Reliance and Technical Misuse in Dental Laser Use

**Search date: 2026-09-15.** This note synthesizes a focused literature and manufacturer-manual search conducted to support the reframing of [[01 Projects/Diode Laser Biopsy]] around **preset reliability**. Full query log, per-source counts, deduplication notes, and stated coverage limitations: [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Report - Preset Reliance and Technical Misuse|Search Report]].

This note follows the vault's FACT / INTERPRETATION / HYPOTHESIS discipline throughout ([[AGENTS.md]]). Sources newly surfaced in this search have not been ingested through Zotero/ZotLit and therefore do not yet have `07 Data/` extraction notes — they are cited here by author/year/DOI directly, per the vault's ingestion policy (`07 Data/` is not created from a discovered citation without that ingestion step). Existing vault primary evidence (Hanke 2021, Strakas 2023, Parker 2022, Xue 2022, Zegaib 2011, Kim 2020, Prado 2022, Al-Ani 2023/2024) is reused and linked where relevant, not re-derived.

## 1. Why presets exist

FACT: All three manufacturer manuals reviewed in this search (AMD Lasers Picasso 810 nm/7 W; A.R.C. Laser FOX 810/980/1064 nm; Biolase Epic X 940 nm, same platform family as the vault's [[05 Devices/Epic 10 TM|Epic 10 TM]]) ship with stored, named parameter programs the console calls "presets": Picasso offers four user-programmable PRESET slots plus one factory-fixed protocol (tooth whitening); the A.R.C. Laser FOX stores "programs and preset values" per application; Biolase Epic X is "factory-installed with 14 preprogrammed procedural presets and 6 empty slots for custom pre-sets," each tied to a named procedure (Gingivectomy/Gingivoplasty, Troughing, Curettage, Excision, Frenectomy/Frenotomy, Implant Recovery, Perio Pockets, Pulpotomy, and others).

INTERPRETATION: The consistent structure across three independent manufacturers — a named procedure mapped to a stored power/mode/pulse value the clinician can recall without manually re-entering every parameter — suggests presets function as a parameter-selection shortcut. None of the three manuals states this purpose explicitly in those words; this is a reading of the manuals' own design, not a quoted manufacturer rationale.

## 2. Evidence of preset/default use

FACT (device level): Presets exist and are factory-installed on multiple dental diode consoles (§1).

NOT FOUND (clinician-behavior level): This search did not locate a study measuring how often, or under what circumstances, practicing dentists actually select an unmodified factory preset versus a custom or manually adjusted setting. The domain-1 searches (`dental laser preset settings`, `laser parameter selection dentistry`, `guided mode laser dentistry preset` — see search report) returned no dental-specific behavioral or survey study of preset selection frequency. This gap should be stated plainly rather than inferred from the fact that presets exist: **presets existing on a device is not evidence that clinicians rely on them.**

## 3. User knowledge and training

FACT: Cross-sectional surveys of dentist awareness/knowledge of dental lasers were found and are new to this vault:
- Palanivelu et al., "Awareness of Laser Dentistry Among Dentists in Tanjore- A survey" (2018), doi:10.13005/bpj/1530 — abstract states laser use "is limited due to the lack of knowledge, effectiveness and the high cost of laser unit."
- "Knowledge and Practice of Dentists toward Dental Lasers and Their Use during and Post-COVID-19 Pandemic Scenario in South India" (2024), doi:10.1055/s-0044-1787847.
- "Knowledge and practices of dental lasers among dental professionals in India: A survey-based study" (2018), doi:10.4103/jdl.jdl_2_18, surveyed at the 69th Indian Dental Conference.
- "'Laser dentistry'—The need of the hour: A cross-sectional study" (2020), doi:10.4103/jpbs.jpbs_89_20.

UNCLEAR: Whether these surveys separate **general device awareness** from **parameter-specific knowledge** (wavelength, CW vs. PW, power selection logic) and from **formal laser training** as distinct measured variables could not be confirmed from titles/abstracts alone; full-text review is needed (see priority list in the final report). Per the task's instruction, awareness is not equated with technical competence here.

FACT: A direct PubMed search for `(dentist OR dental practitioner) AND (laser parameter OR laser setting) AND (knowledge OR training OR awareness)` returned 13 PMIDs, of which essentially none addressed dentist-specific parameter knowledge or training on full inspection (matches were driven by broad MeSH-term expansion into unrelated topics — halitosis, TMJ physiotherapy, caries diagnosis, etc.; one tangential hit, Wigdor 2008 "Basic physics of laser interaction with vital tissue," doi:10.1016/j.aodf.2008.07.031, discusses that practitioners need laser-physics understanding to interpret "visual feedback" and adjust parameters, but is a general-education article, not an empirical training assessment). This indicates the survey literature that does exist on this topic (§3 above) is concentrated in venues not indexed by PubMed/MEDLINE (Biomedical & Pharmacology Journal, Journal of Dental Lasers, Journal of Pharmacy and Bioallied Sciences) — a coverage gap, not evidence of absence.

## 4. Parameter-selection behavior

NOT FOUND: No observational or behavioral study of how dentists actually select power, mode, or pulse parameters in practice (as opposed to self-reported awareness) was located in this search.

FACT (prescriptive, not behavioral): Manufacturer manuals instruct clinicians on how selection *should* happen, which is not evidence of how it *does* happen:
- Biolase Epic X: "Always use clinical judgement when selecting power, pulse, length, and pulse interval parameters to ensure optimal clinical results... At all times observe the clinical effects on the treatment area and adjust parameters accordingly."
- AMD Lasers Picasso: "Physicians must use their own clinical judgment and professionalism in determining all aspects of treatment, technique, proper power settings, interval, duration, etc." The same manual states elsewhere: "AMD LASERS™, LLC assumes no responsibility for parameters, techniques, methods, or results."

These are manufacturer disclaimers and instructions, not measurements of clinician behavior.

## 5. Evidence linking knowledge gaps to preset reliance

NOT FOUND — searched for directly, per the task's explicit instruction not to infer this link from co-occurring evidence.

FACT: A direct PubMed search, `laser preset OR "default setting" AND dental AND (novice OR training OR experience)`, returned **0 results**.

FACT: OpenAlex agent-search queries `novice preset reliance laser` and `laser training preset dependence` (120 raw hits each before dedup; see search report) returned no dental- or laser-relevant results after review — all top-scoring hits were unrelated physics/engineering/rehabilitation literature.

**Explicit statement per task instruction:** §1 (presets exist) and §3 (knowledge/training gaps are documented in general dental-laser awareness surveys) together do **not** establish that training gaps cause preset reliance. No source in this search states or tests that link. This must remain absent from the vault's claims until direct evidence is found.

## 6. Manufacturer preset provenance

Three manufacturer manuals were retrieved and read in full text (converted from PDF; see search report for source URLs and extraction method). Findings are tabulated against the task's specific questions. `UNCLEAR` is used where the manual did not address a question; absence in the manual does not prove no validation exists elsewhere (e.g., a separate technical file, an unpublished internal study, or a submission to a regulatory body).

| Question | Picasso (AMD Lasers, 810 nm, 7 W) | FOX (A.R.C. Laser GmbH, 810/980/1064 nm)* | Epic X (Biolase, 940 nm)† |
|---|---|---|---|
| Preset values listed? | Partial — one full fixed protocol (teeth whitening: 7.0 W, CW, 30 s); soft-tissue cutting/coagulating given only as a power *range* (0.5–5.0 W), not per-procedure values; PRESETS 1–4 are user-programmable, not factory-fixed | YES — device stores named "programs and preset values" | YES — full table of 8+ named dental procedures with mode, peak power, average power, pulse length, duty cycle |
| Labeled "preset," "recommended," "suggested," or "starting point"? | "PRESET" | "PRESET" | "PRESET" / "PRE-PROGRAMMED SETTINGS" |
| Derivation explained? | NO | NO (manual states only: "the medical application is only addressed in general... A.R.C. Laser GmbH only gives recommendations for applications") | YES, in general terms only: "The procedure pre-sets installed at the factory are based on clinical recommendations and feedback from experienced laser dentists" |
| Supporting evidence cited (a study, a trial, a reference)? | NO | NO | NO — no citation to any specific published study or dataset |
| Tissue type specified? | Generic list of 20+ soft-tissue indications; no per-procedure power value tied to tissue type | UNCLEAR (not found in reviewed sections) | YES — an "Indications for Use" column per preset (e.g., "Reduction of gingival hypertrophy, vestibuloplasty") |
| Wavelength specified? | YES (fixed, single-wavelength device) | YES (multiple wavelength variants exist) | YES (fixed, single-wavelength device) |
| Fiber diameter specified? | YES — standard 400 μm; 200–1000 μm available; a fiber-diameter/output relationship is noted for the 7 W setting | UNCLEAR (not found in reviewed sections) | YES — 300 μm vs. 400 μm tip selection is tied to tissue type ("300 μm Tips are recommended for removing thin tissue layers. 400 μm Tips are recommended for removing fibrous tissue") |
| Tip initiation specified? | Only for teeth whitening (uninitiated fiber); not addressed for soft-tissue cutting | UNCLEAR | YES — explicit tip-initiation screen/protocol tied to the selected tip |
| Contact vs. non-contact mode specified? | Implied (handpiece/fiber contact) but not stated explicitly | UNCLEAR | UNCLEAR in the reviewed excerpt |
| Incision speed or dwell time specified? | NO | NO | NO — the pre-programmed-settings table gives no speed or dwell-time field |
| Delivered/output power independently measured (by the manufacturer, for the preset)? | NO | NO | NO — the preset table reports console/panel values only |
| Power meter mentioned anywhere in the manual? | Only an internal "Energy Monitor" that flags a >20% deviation from the selected value as an error; factory calibration and annual recalibration by authorized personnel are mentioned, but no external verification procedure for the treating clinician | YES, explicitly, in the periodic safety-check (STK) procedure: "Check the set power with an external power meter (permissible tolerance ± 20%)" — performed by trained service personnel at intervals of ≤24 months, not by the clinician per use | Only in the separate calibration section, not tied to individual presets: "Laser calibration is recommended every twenty-four (24) months in order to maintain the required accuracy of output power versus displayed power," performed at a "certified depot repair facility" |
| Adjustment according to tissue response recommended? | YES, explicitly: monitor the patient for pain/discomfort and "adjust settings, apply anesthesia, or cease treatment" | YES, explicitly: stored presets do "not release the surgeon from checking the values according to his knowledge and the desired interaction with the tissue... the preset values must be adjusted" if necessary | YES, explicitly: "observe the clinical effects on the treatment area and adjust parameters accordingly"; separately for a non-dental (pain-therapy) preset, "monitor patient response; adjust power and/or distance as needed" |
| Minimum effective power recommended? | YES, explicitly, for cutting/coagulating soft tissue: "Operator should try to use the least amount of power (WATTS) to achieve desired results" | NOT found in the reviewed sections | Partially — a footnote on the endodontic (Pulpotomy-type) presets states "Minimum defaults provided," and a separate non-dental pain-therapy protocol instructs "Always start at the lowest power setting and increase as necessary"; not stated as a universal rule across all dental presets |

\* The retrieved A.R.C. Laser FOX manual (`User_Manual_FOX_rev0`, August 2021) is the general medical-device manual for the FOX platform (810/980/1064 nm); this search could not confirm whether it is identical to a dental-specific IFU for the FOX units catalogued in this vault's [[05 Devices/A.R.C. Laser FOX (810 nm)|FOX (810 nm)]] / [[05 Devices/A.R.C. Laser FOX (980 nm)|(980 nm)]] / [[05 Devices/A.R.C. Laser FOX (1064 nm)|(1064 nm)]] notes — flagged `UNCLEAR` rather than assumed identical.

† The retrieved manual is for "Epic X," not confirmed identical to the "Epic 10 TM" model already catalogued in [[05 Devices/Epic 10 TM]] (measured in Kim et al. 2020). Both are Biolase 940 nm platforms from the same product family; this vault does not treat them as the same model without confirmation, consistent with the existing caveat in [[05 Devices/Epic 10 TM]] about a separate, unconfirmed Biolase device in Fahlstedt et al. 2021.

NOT SEARCHED in this pass (`UNCLEAR` by omission, not by finding): Dentek LD 15, Gemini Evo, K2 Mobile, LITEMEDICS, Quicklase 12W Dual 4, Raffaello, SIROLaser Blue (fetch attempts returned HTTP 403 from both ManualsLib and Manualzz — access blocked, not searched further), SOL, Saeshin Diode Laser, Wiser 3, Zolar Plus, and A.R.C. Laser WOLF (1470 nm). Absence of a manual review for these devices is a scope limitation of this pass, not evidence about their preset provenance.

## 7. Preset validation/transparency

FACT: None of the three manufacturers cites a published, peer-reviewed source for its preset values. Epic X's stated derivation ("clinical recommendations and feedback from experienced laser dentists") is the most explicit of the three, but it describes an informal, non-cited basis — expert/practitioner consensus, not a controlled validation study tying the preset to measured delivered power or a histologic outcome.

NOT FOUND: No study located in this search validates a **named, manufacturer-labeled preset** — as opposed to a researcher-selected bench power level — against both independently measured delivered power and a histologic/tissue-effect outcome. This is distinct from, and narrower than, the vault's existing finding that measured power + controlled speed + histology has precedent (Hanke 2021, Strakas 2023): those studies select power levels as an independent experimental variable, not by recalling a device's stored preset.

One new candidate worth full-text follow-up: "Toward evidence-based laser dentistry: wavelength selection, parameter standardization and clinical outcomes" (2026), doi:10.18203/2394-6040.ijcmph20263229 — a narrative review whose title directly addresses parameter standardization; its actual content and evidence base were not verified beyond title/abstract in this pass.

## 8. Preset vs. set power vs. delivered power

This distinction is already established as this vault's strongest existing evidence base, and is reused rather than re-derived here — see [[04 Evidence/Set Power vs Measured Output]] for the full evidence note. Summary, keeping preset / set power / measured power / delivered power / tissue exposure / tissue effect explicitly distinct per the task's instruction:

- FACT: [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters|Parker et al. 2022]] measured post-fibre emission for 38 dental diode devices (20 device types) at control-panel settings of 100 mW/500 mW/1.0 W/2.0 W, and found statistically significant, device-specific deviation from the panel value, mainly below the set value.
- FACT: [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output|Xue et al. 2022]] found deviations both above and below the preset (+21% to +37% for two devices, −3% to −8% for a third), depending on device and CW/pulsed mode.
- FACT: [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers|Kim et al. 2020]] reported set vs. measured ("Actual") power differed at all 9 device × setting combinations tested, again in both directions depending on device.
- FACT: [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage|Zegaib et al. 2011]] found measured output below the 1.0 W panel reference in every condition, with contact-induced loss increasing progressively across repeated applications (up to a mean 40.26% loss by the fourth application).
- FACT (added 2026-09-14 to the vault): [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] reported a numeric measured-power value distinct from the display value (1.2 W display → 1.0 W measured; 1.8 W display → 1.5 W measured), independently confirming under-delivery in a fifth device.

**Newly added in this search (manufacturer's own voice, primary source):**
- FACT: The A.R.C. Laser FOX manual states directly: "The displayed value may vary from the emitted value at the distal tip, by a range of ± 20%."
- FACT: The Biolase Epic X manual frames its recalibration interval explicitly around this same gap: calibration "is recommended every twenty-four (24) months in order to maintain the required accuracy of output power versus displayed power" — the manufacturer's own stated purpose for calibration is to keep two different, separately named quantities (output power, displayed power) close to each other, which presupposes they can diverge.
- FACT: The AMD Lasers Picasso manual describes an internal "Energy Monitor" that halts operation if measured output deviates more than 20% from the console-selected value — again presupposing that the two values are not guaranteed identical.

INTERPRETATION (retained from the existing evidence note, now reinforced by manufacturer-manual evidence): console-set power (and, by extension, a recalled preset's console value) cannot be treated as a reliable proxy for actual delivered power without independent, per-use verification — this is not only an experimental finding from bench studies, but a limitation manufacturers themselves state in their own manuals, with tolerance bands as wide as ±20%.

## 9. Incision speed / operator technique

FACT (reused from the vault's existing project scaffolding, reconfirmed by this search): among diode ex vivo oral-tissue studies, only [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] (2 mm/s, mechanized) and [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]] / [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] (0.75 mm/s, explicit) report a numeric, controlled incision speed; [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]] reports 10 mm/s, mechanized.

FACT, newly confirmed in this search: **none of the three manufacturer manuals reviewed (Picasso, FOX, Epic X) specifies incision speed or dwell time anywhere alongside their power/mode presets.** Every preset table found gives power, mode, and (where pulsed) pulse length/duty cycle — never a speed or movement-time field.

INTERPRETATION: This directly supports the task's framing — a preset specifying power but not speed incompletely defines tissue exposure, since the same power delivered over a slower pass necessarily transfers more energy per unit tissue length/area than a faster pass. This is a device-manual-level finding, not yet a tested experimental one; the ex vivo project's own controlled-speed design (see [[01 Projects/Diode Laser Biopsy#Logic chain]]) is the mechanism that would test it directly.

One new candidate flagged for full-text follow-up, not yet reviewed beyond title/abstract: "In vitro histological evaluation of the surgical margins made by different laser wavelengths in tongue tissues" (2016), doi:10.4317/jced.52830, and "Reduction of collateral thermal impact of diode laser irradiation on soft tissue due to modified application parameters" (2011), doi:10.1007/s10103-011-1007-x — both may report speed or movement-technique detail; UNCLEAR without full text.

## 10. Technical misuse / operator risk

NOT FOUND: No case series, incident report, or empirical study documenting technical misuse of a dental diode laser (inappropriate parameter selection, prolonged dwell, excessive power, wrong pulse mode, incorrect fiber/tip use) specifically attributed and verified as misuse was located. The dedicated domain-8 searches (`dental laser operator error`, `laser thermal injury carbonization dental`, `inappropriate laser parameters dental injury` — 90–120 raw hits each) returned almost entirely off-topic results (implant/3D-printing/materials-science literature); the few dental-laser hits were general reviews of thermal effects, not misuse case evidence.

FACT (context, not misuse evidence): Manufacturer manuals place the responsibility for technique and parameter selection explicitly on the clinician and disclaim manufacturer responsibility (§4). This is a liability/responsibility framing statement, not a finding that misuse has occurred or is common.

FACT (general laser-safety literature, theoretical/background): Thermal injury and carbonization are established, well-described biophysical phenomena in laser-tissue interaction literature generally (not disputed), but this search found no source connecting a documented dental-laser thermal-injury case specifically to preset use, parameter misselection, or training deficiency, as opposed to any other cause. **Per the task's explicit instruction, nothing here is labeled "misuse" — the correct label for what this search found is "not documented," not "documented but rare."**

## 11. Safety / adverse events

FACT: General dental-laser safety and regulatory guidance was found, new to this vault: "Safety Guidelines for the Laser Removal of Dental Calculus" (2012), doi:10.5978/islsm.12-sg-05; "Laser regulation and safety in general dental practice" (2007), doi:10.1038/bdj.2007.370; "Principles and practice of laser dentistry" (2011), doi:10.1038/sj.bdj.2011.329; "Eye safety in operative dentistry — A study in general dental practice" (2006), doi:10.1038/sj.bdj.4813257; "Therapeutic and Adverse Effects of Lasers in Dentistry: A Systematic Review" (2023), doi:10.3390/photonics10060650.

FACT (general dental, not laser-specific): "How dental team members describe adverse events" (2016), doi:10.1016/j.adaj.2016.04.015, is a general dental patient-safety study, not laser-specific.

UNCLEAR: For every source above, whether any reported adverse event is attributed to parameter selection, operator technique, equipment malfunction, training deficiency, or unknown cause could not be determined from title/abstract; this requires full-text review (see priority list in the final report). No causal attribution is asserted here.

## 12. Medico-legal evidence

FACT: Two medico-legal sources were found that discuss laser-related or dental malpractice trends: "A trend of Medical Negligence in Laser Therapy in the Capital City: A Nine-Year Survey" (2022), doi:10.34172/jlms.2022.29 — a legal-document analysis of laser-therapy malpractice claims; UNCLEAR whether this is dental-specific or spans laser medicine broadly (dermatology, ophthalmology, etc.) without full-text review. "Malpractice Payments and Adverse Actions against Dentists in Texas — A Fifteen-Year Trend Analysis" (2022), doi:10.46889/jdhor.2022.3215 — general dental malpractice trend analysis, not laser-specific per its abstract. A related general-dentistry source, "Iatrogenic mistakes in dentistry, when to disclose: a literature review" (2025), doi:10.18203/2394-6040.ijcmph20250649, is not laser-specific either.

NOT FOUND: No source in this search ties a specific dental-laser malpractice or negligence finding to parameter selection, preset use, or a delivered-power discrepancy.

**Per the task's explicit instruction: this section is retained as context only. It is not used as scientific evidence of tissue mechanisms, and no causal inference is drawn from it about this project's ex vivo hypotheses.**

## 13. Established vs. plausible/speculative concerns

**Established** (multiple independent primary sources, several already in this vault, reinforced here by manufacturer-manual evidence):
- Console-set/preset power and independently measured delivered power differ, in direction and magnitude that vary by device — not a single universal correction factor. (§8; [[04 Evidence/Set Power vs Measured Output]])
- Manufacturers themselves state that displayed/console values may diverge from delivered values (FOX: ±20%) and that stored presets do not remove the need for the clinician to verify against tissue response (§6, §8).
- Independently measured power + controlled speed + histologic thermal-effect assessment has direct methodological precedent in ex vivo oral diode-laser tissue cutting (Hanke 2021, Strakas 2023), though not tied to a named preset or a biopsy-oriented outcome.
- No manufacturer manual reviewed specifies incision speed or dwell time alongside its power presets (§9).

**Supported but incomplete:**
- General dentist awareness/knowledge of dental lasers is documented by multiple cross-sectional surveys (§3), but whether these surveys isolate parameter-specific knowledge or formal training as distinct variables is unconfirmed without full-text review.
- Manufacturer preset provenance is described in general terms for one of three devices reviewed (Epic X: "clinical recommendations and feedback from experienced laser dentists"), but is not tied to any cited, published validation study for any device (§6, §7).

**Plausible, not evidenced in this search (remains HYPOTHESIS):**
- That less-trained or novice clinicians rely more heavily on unmodified factory presets than experienced clinicians. Reasonable by general human-factors reasoning; no dental-laser source found to test it directly (§5).

**Speculative / not supported by this search (remains HYPOTHESIS, and is precisely what this project's ex vivo experiment is designed to test rather than assume):**
- That preset reliance specifically causes adverse tissue effects or diagnostic-quality-compromising outcomes in biopsy practice. No source found links preset use to a documented adverse tissue outcome or malpractice finding (§10, §12).

**Explicitly not established, searched for directly and not found:**
- A direct link between clinician knowledge/training gaps and preset-reliance behavior (§5).
- Any case of documented technical misuse of a dental diode laser specifically attributed to parameter misselection (§10).

## 14. Implications for the ex vivo study

INTERPRETATION: This search supports, and narrows, the reframed research question in [[01 Projects/Diode Laser Biopsy]]. Three findings matter most for the experimental design:

1. Preset provenance is real (named, stored, procedure-mapped values exist on real devices) but general and unvalidated against either delivered power or histologic outcome — so testing an actual manufacturer-labeled preset, rather than an arbitrary researcher-chosen bench power level, is a meaningful and currently untested experimental choice (see [[01 Projects/Diode Laser Biopsy#Immediate next steps]] item 4).
2. Delivered power reliably diverges from console/preset value, but not in one consistent direction across devices — so any preset tested must be independently, per-incision verified with a calibrated power meter (following the Hanke 2021/Strakas 2023 protocol), not assumed correct from the panel display.
3. Incision speed is essentially unaddressed in the manufacturer guidance reviewed — reinforcing that this project's controlled-speed design fills a real gap in what manufacturers themselves specify, not just a gap in prior published studies.

No source found in this search combines a named preset, independently measured delivered power, controlled incision speed, and a biopsy-oriented histologic outcome in one design — this remains the project's central open gap, now stated with an added, more precise dimension (the preset itself, not just a bench power value, is untested).

## 15. Updated study rationale

Procedure-based presets may simplify parameter selection, but their evidentiary provenance, their relationship to actual delivered power, and their ability to predict tissue effect may be incompletely established. This search supports that statement directly: derivation is described only in general terms (§6–§7), no cited validation study was found for any preset reviewed, and independent measured-power evidence shows console values cannot be trusted as delivered-power proxies without verification (§8). Actual exposure may also depend on device output, fiber transmission, tip condition, tissue properties, and incision speed/operator movement — none of which any reviewed manual ties to its stated presets (§6, §9). Testing preset/set power against independently measured delivered power and histopathologic effect under controlled incision speed is therefore practically relevant on its own terms — this rationale does not require, and does not make, clinician misuse a premise of the experiment (§10, §13). The full updated rationale, canonical research question, and logic chain are recorded in [[01 Projects/Diode Laser Biopsy#Research rationale]].

## 16. สรุปภาษาไทย

- โน้ตสังเคราะห์นี้รวบรวมผลการค้นวรรณกรรมและคู่มือผู้ผลิตที่ทำขึ้นเพื่อสนับสนุนการปรับกรอบโครงการ [[01 Projects/Diode Laser Biopsy]] ให้เน้นเรื่อง **ความน่าเชื่อถือของค่าพรีเซ็ต (preset reliability)**
- **พรีเซ็ตมีอยู่จริง**: อุปกรณ์เลเซอร์ไดโอดทางทันตกรรมจากผู้ผลิต 3 ราย (AMD Lasers Picasso, A.R.C. Laser FOX, Biolase Epic X) มีค่าพรีเซ็ตที่ตั้งชื่อตามหัตถการติดตั้งมาจากโรงงาน
- **ที่มาของพรีเซ็ตไม่ชัดเจน**: มีเพียงเครื่องเดียว (Epic X) ที่ระบุที่มาเป็นคำทั่วไปว่า "อิงคำแนะนำทางคลินิกและความคิดเห็นจากทันตแพทย์เลเซอร์ที่มีประสบการณ์" ไม่มีเครื่องใดอ้างอิงงานวิจัยที่ตีพิมพ์
- **พรีเซ็ต ≠ กำลังที่ส่งจริง**: คู่มือ A.R.C. Laser FOX ระบุตรงๆ ว่าค่าที่แสดงบนจออาจต่างจากค่าที่ปล่อยออกจริงที่ปลายไฟเบอร์ได้ถึง ±20% และทั้งสามคู่มือแนะนำให้ปรับตามการตอบสนองของเนื้อเยื่อเสมอ ไม่ใช่ใช้ค่าพรีเซ็ตตรงๆ โดยไม่ตรวจสอบ
- **ไม่มีคู่มือใดระบุความเร็วในการตัดหรือเวลาสัมผัสควบคู่กับค่ากำลัง** ซึ่งสนับสนุนแนวคิดว่าพรีเซ็ตที่ระบุแต่กำลังไฟฟ้าโดยไม่ระบุความเร็ว อาจนิยามปริมาณรังสีที่เนื้อเยื่อได้รับไม่ครบถ้วน
- **ไม่พบหลักฐานตรง** ที่เชื่อมโยงช่องว่างความรู้/การฝึกอบรมของทันตแพทย์เข้ากับพฤติกรรมการพึ่งพาพรีเซ็ต (ค้นใน PubMed ได้ผลลัพธ์ 0 รายการ) — จึงไม่สรุปว่าความรู้ที่ขาดหายเป็นสาเหตุของการพึ่งพาพรีเซ็ต
- **ไม่พบหลักฐานการใช้งานผิดพลาดทางเทคนิค (misuse) ที่มีการบันทึกไว้อย่างเป็นรูปธรรม** สำหรับเลเซอร์ไดโอดทางทันตกรรม จึงไม่ใช้คำว่า "misuse" ในโน้ตนี้
- ข้อสรุปเหล่านี้สนับสนุนเหตุผลของโครงการ ex vivo โดยไม่จำเป็นต้องตั้งสมมติฐานว่ามีการใช้งานผิดพลาดของแพทย์เป็นเงื่อนไขเบื้องต้น

## Related notes

- Project: [[01 Projects/Diode Laser Biopsy]]
- Evidence: [[04 Evidence/Set Power vs Measured Output]]
- Data: [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]], [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]], [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]], [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]], [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data]], [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data]], [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]], [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data]]
- Devices: [[05 Devices/Epic 10 TM]], [[05 Devices/A.R.C. Laser FOX (810 nm)]], [[05 Devices/A.R.C. Laser FOX (980 nm)]], [[05 Devices/A.R.C. Laser FOX (1064 nm)]], [[05 Devices/Device Index]]
- Concepts: [[03 Concepts/Laser Presetting]], [[03 Concepts/Power Output]], [[03 Concepts/Power Loss]], [[03 Concepts/Operating Parameters]]
- Search report: [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Report - Preset Reliance and Technical Misuse]]
