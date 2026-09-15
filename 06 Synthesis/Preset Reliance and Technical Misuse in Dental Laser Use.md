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

† The retrieved manual is for "Epic X," not confirmed identical to the "Epic 10 TM" model already catalogued in [[05 Devices/Epic 10 TM]] (measured in Kim et al. 2020). Both are Biolase 940 nm platforms from the same product family; this vault does not treat them as the same model without confirmation, consistent with the existing caveat in [[05 Devices/Epic 10 TM]] about a separate, unconfirmed Biolase device in Fahlstedt et al. 2021. **Update (2026-09-15):** this caveat is now resolved — see §17, which retrieves and compares the Epic™10's own manufacturer manual directly, rather than relying on the Epic X manual as a proxy.

NOT SEARCHED in this pass (`UNCLEAR` by omission, not by finding): Dentek LD 15, Gemini Evo, K2 Mobile, LITEMEDICS, Quicklase 12W Dual 4, Raffaello, SIROLaser Blue (fetch attempts returned HTTP 403 from both ManualsLib and Manualzz — access blocked, not searched further; **resolved 2026-09-15, see §18**), SOL, Saeshin Diode Laser, Wiser 3, Zolar Plus, and A.R.C. Laser WOLF (1470 nm). Absence of a manual review for these devices is a scope limitation of this pass, not evidence about their preset provenance.

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

## 17. Follow-up (2026-09-15): Epic X-family documentation vs. Epic 10 TM

This section completes the task left open by the §6/§7 footnote (†): §6–§7 above characterized Biolase's preset architecture using the **Epic X** manual only, because at the time no Epic 10-specific manual had been retrieved. This follow-up retrieves the manufacturer's own **Epic™10** manual directly (not the Epic X manual) and compares it against Epic X's, so the vault's Epic 10 TM claims rest on Epic 10's own primary documentation rather than an unconfirmed same-family assumption.

**Sources retrieved (official manufacturer, full text, not yet Zotero-ingested — cited directly per the vault's ingestion policy):**
- "EPIC 10 User Manual," P/N 5400321 Rev. H — `biolase.com/media/EPIC_User_Manual.pdf` — the model catalogued in this vault as [[05 Devices/Epic 10 TM]] (the manual's own running header renders the model name as "Epic™10").
- "Epic X User Manual," Rev. A — `biolase.com/media/5400228-RevA_EpicX_UserManual-.pdf` — same file already used in §6–§7, re-examined here for direct table-by-table comparison.
- Context only (marketing pages, not clinical/technical documentation): `biolase.com/products/dental-lasers-soft-tissue/epic-10/` and `.../epic-x/` — used only to establish market positioning (§17.3), not cited for any parameter value.

### 17.1 Exact model names

FACT: The Epic 10 manual's own header text reads "EpicTM10" (i.e., Epic™10) throughout, and its cover/table-of-contents reads "EPIC 10 User Manual." This vault's existing device note title, [[05 Devices/Epic 10 TM]], is the same model — the "TM" in the note title is a plain-text rendering of the ™ symbol, not a separate model variant. This was previously unconfirmed and is now settled directly from the manufacturer document itself, not inferred.

FACT: Epic X's own manual header reads "Epic X User Manual." Epic 10 and Epic X are two separately named, separately manualed products in Biolase's current soft-tissue diode lineup — they are not the same model, and the manufacturer's own product pages describe them as different generations (§17.3), so they are correctly kept as distinct entries in this vault.

### 17.2 Side-by-side comparison (both values read directly from each device's own manual)

| Field | Epic 10 (own manual) | Epic X (own manual) | Same? |
|---|---|---|---|
| Wavelength | 940 ± 10 nm | 940 ± 10 nm | YES |
| Max power output | 10 W | 10 W | YES |
| Power accuracy (manufacturer-stated tolerance) | ± 20% | ± 20% | YES |
| Power modes | Continuous, Pulse Modulation | Continuous, Pulse Modulation | YES |
| Fiber tip diameters | 200 μm, 300 μm, 400 μm | 200 μm, 300 μm, 400 μm | YES |
| Pulse duration range | 0.01 ms – 20 ms | (not independently re-extracted in this pass; not a discrepancy found) | UNCLEAR (not re-checked) |
| Number of named + custom presets | 14 named + 6 custom = 20 slots | 14 named + 6 custom = 20 slots | YES |
| Preset table values (peak power, avg. power, mode, pulse interval, pulse length, duty cycle) | See §17.4 | See §17.4 | YES, for every one of the 14 named presets, checked line by line |
| Preset provenance wording | "The Procedure Pre-Sets installed at the factory are based on clinical recommendations and feedback from experienced laser dentists." | Same sentence, verbatim. | YES, verbatim match |
| Minimum-power guidance | "Always use clinical judgment... Always start treatment at the lowest power setting for that specific indication and increase as required." | "Always start treatment at the lowest power setting for the specific indication and increase as required. BIOLASE assumes no responsibility for parameters, techniques, methods or results." | YES, near-verbatim (Epic X manual adds the liability-disclaimer sentence; Epic 10 does not) |
| Tissue-response adjustment | "At all times observe the clinical effects on the treatment area and adjust parameters accordingly." | Same clause, same wording. | YES, verbatim match |
| Recalibration interval / stated purpose | "Calibration procedure is recommended to be performed every twenty-four (24) months in order to maintain the required accuracy of output power versus displayed power." | Same clause, same wording (minor phrasing: "The calibration can be performed at a certified depot repair facility" vs. Epic 10's "Bi-annual calibrations can be performed..."). | YES, same purpose and interval |
| Incision speed or dwell time specified | NO — not present anywhere in the preset table or surrounding text | NO | YES (both silent) |
| Settings editable by clinician | YES — "To store your personal preferred settings for any procedure: ... Enter the new values ... Touch and hold the Procedure name for more than 2 seconds ... settings are saved." | Same store/edit mechanism described. | YES |
| Tip initiation requirement | Explicit protocol (touch tip to initiation block, fire footswitch, pull out while firing); "Not required if using pre-initiated tips" | Same protocol described; pre-initiated tips also supported | YES |
| Validation study cited for preset values | NO — none | NO — none | YES (both silent) |

FACT: All 14 named presets (Gingivectomy/Gingivoplasty, Troughing, Curettage, Excision, Frenectomy/Frenotomy, Implant Recovery, Perio Pockets, Pulpotomy, Crown Lengthening, Infected Pockets, Endo, Hemostasis, Aphthous Ulcers, Exposure of Unerupted Teeth) carry numerically identical peak power, average power, mode (CP0/CP1/CP2/CW), pulse interval, pulse length, and duty cycle values in the Epic 10 manual's Table 7.4 and the Epic X manual's Table 8.3. (One row — Frenectomy/Implant Recovery — rendered ambiguously across two lines in the Epic X PDF's `pdftotext` extraction due to a layout artifact, not a value discrepancy; cross-checking against the Epic 10 table, which extracted cleanly, resolves it as the same two values in the same order.)

### 17.3 What differs between Epic 10 and Epic X (context, not preset data)

FACT (from manufacturer marketing pages, not the manuals themselves): Epic 10 is described as Biolase's "Undisputed Classic Diode System," originally launched in 2012; Epic X is positioned as the newer, "most up-to-date and enhanced everyday diode laser," sold in the US/Canada, while Epic 10 is sold in markets where Epic X has not yet received regulatory clearance. Epic X's marketed advantages over Epic 10 are software/UI and workflow features — new cordless foot-pedal software, laser-assisted whitening, and pain-therapy modes bundled as core positioning — not different soft-tissue-surgery power/mode values. Epic 10's own manual (§7.5, §7.6) shows Epic 10 also supports whitening and pain-therapy procedures, so this marketing distinction is softer than the product pages imply; it was not independently verified further, as it is not a preset-value question.

INTERPRETATION: The generational/market difference between Epic 10 and Epic X is real (different manuals, different model names, different launch dates) but does not extend to the soft-tissue surgical preset table, which is identical between the two, as read directly from each device's own manufacturer manual.

### 17.4 Classification

**SAME DEVICE FAMILY / CLEARLY TRANSFERABLE** — with an important qualification: this classification is not based on inferring that Epic X settings apply to Epic 10 TM. It is based on Epic 10 TM having its **own** manufacturer-published preset table (§17.2), which independently states the same wavelength, power-accuracy tolerance, fiber-tip range, and all 14 named preset values as Epic X's manual. The Epic X-family documentation reviewed in §6–§7 is confirmed, not merely assumed, to describe the same preset architecture and values as Epic 10 TM's own documentation. No transfer across models was necessary or performed — both models' own manuals were read and compared directly.

## 18. Follow-up (2026-09-15): SIROLaser Blue IFU/manual

The §6 table's "NOT SEARCHED" list previously included SIROLaser Blue, blocked by HTTP 403 on both mirror hosts it was searched for at the time (ManualsLib, Manualzz). This follow-up retrieves the manufacturer's own current IFU directly from `dentsplysirona.com`.

**Source retrieved (official manufacturer, full text, not yet Zotero-ingested — cited directly per the vault's ingestion policy):**
- "Instructions for use SiroLaser Blue," document ref. 66 56 842 D3648, revision code `D3648.201.03.09.23`, dated 2025-03, "valid for USA," English.
- **Access note:** the URL surfaced by web search (`.../ifu/INS-IFU-SiroLaser-Blue-USA-EN-6656842-2025-03-19.pdf`) returned HTTP 404. The same document, same 2025-03 revision, was successfully retrieved from a sibling path with `/archived/` inserted before the filename (`.../ifu/archived/INS-IFU-SiroLaser-Blue-USA-EN-6656842-2025-03-19.pdf`), which returned HTTP 200. This is logged as a retrieval-path quirk on Dentsply Sirona's CDN, not evidence that the 2025-03 revision is superseded — the document's own title page and running header both self-identify as the current, non-archived 2025-03 US IFU. Full access log: [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Log - Epic 10 and SIROLaser Blue Manual Verification 2026-09-15]].

### 18.1 Device scope: three wavelengths, not two

FACT, new to this vault: the SIROLaser Blue IFU documents **three** laser wavelengths, not the two (445 nm, 970 nm) recorded in [[05 Devices/SIROLaser Blue]] from the vault's existing primary sources (Xue et al. 2022, Romanos et al. 2022). The IFU's technical-data section lists:
- 445 nm (−10/+15 nm), ≈0.2–3.0 W, CW, Class 4 — surgical/whitening wavelength.
- 970 nm (−10/+15 nm), ≈0.2–2.0 W, CW, Class 4 — surgical/whitening wavelength.
- 660 nm (±5 nm), ≈25/50/100 mW, Class 2 — used only for Low-Level-Laser Therapy (LLLT); explicitly stated to have **no preset programs**: "The device has one general preset program for 445nm and no preset programs for 660 nm."

This is a device-note-level finding (the existing [[05 Devices/SIROLaser Blue]] note is not edited in this pass per task scope, but this gap is flagged here for a future update): neither Xue et al. 2022 nor Romanos et al. 2022 tested or reported the 660 nm wavelength, so the vault's existing device note is not wrong, only incomplete relative to the full manufacturer spec — this is a scope gap in prior study coverage, not a data-quality problem in the existing note.

### 18.2 Preset table (§6.2 "List of preset indications" of the IFU)

FACT — extracted directly:

| Category | Preset name | Wavelength | Power | Mode | Time | Fiber | Notes |
|---|---|---|---|---|---|---|---|
| Endodontics | Pulpotomy | 970 nm | 1.5–2.0 W | CW | 20 s | 200 μm | "After conventional pulp removal, residual pulp tissue can be removed with the laser." |
| Endodontics | Pulpotomy as adjunct to root canal therapy | 970 nm | 2.0 W | CW | 20 s | 200 μm | Hemostasis and residual pulp-tissue removal |
| Miscellaneous | Aphthous Ulcers | 970 nm | (table value not clearly resolved in extraction — see UNCLEAR below) | CW | 20 s | 320 μm | "Apply laser 1–3 mm away from lesion... semicontact, wave the laser fiber over the entire lesion." |
| Periodontology | Sulcular Debridement | 970 nm | (not clearly resolved) | PF (pulsed) | continuous | 320 μm | "Move the fiber tip around the tooth gently up and down with a sinuous movement... Keep the laser tip always in motion!" |
| Periodontology | Gingival incisions of granulation tissue | 970 nm | (not clearly resolved) | PF (pulsed) | continuous | 320 μm | "Reduce power, if pain sensations appear." |
| Surgery | Soft-Tissue Surgery | 445 nm | 2.0 W shown as the worked example; manual states power is user-adjustable 0.2–3.0 W in 0.1 W steps | CW | continuous | 320 μm | Only **one general preset** exists for all surgical indications: "use the laser tip like a scalpel to incise and excise the respective tissues... Caution: Avoid bone contact during treatment!" |
| Additional | Treatment of canker sores | 970 nm | 2.0 W | CW | continuous | 320 μm | Same semicontact technique as Aphthous Ulcers |

UNCLEAR: the duty-cycle and frequency figures for the periodontology (pulsed) and Aphthous Ulcers rows did not extract cleanly from the source PDF's table layout (columns visually merged in `pdftotext` output); the power values for Aphthous Ulcers and the two periodontology rows are similarly ambiguous in the extracted layout. These are flagged `UNCLEAR` rather than guessed — re-extraction from the original PDF's table (not the flattened text) would be needed to resolve them with confidence, and is not done in this pass.

FACT: For surgical (incision/excision) procedures specifically, the IFU offers **exactly one** named preset ("Soft-Tissue Surgery"), not a per-procedure table like Biolase's 14-entry surgical preset table (§17). The clinician is expected to adjust power manually within the 0.2–3.0 W range for the specific surgical indication, rather than selecting among multiple named surgical presets.

### 18.3 Manufacturer wording for presets

FACT: "A number of output settings are preset in the unit. Manual setting changes can be made and custom presets may also be introduced." (§1.1, "Dear Customer" introduction). The IFU uses the word "preset" throughout (e.g., "preset treatment parameters," "preset applications," "preset power levels") but does not use "recommended," "suggested," or "starting point" as a distinct qualifier for preset values, and — unlike the Biolase manuals (§6, §17) — does **not** offer any general statement of preset provenance (no "based on clinical recommendations and feedback from..." equivalent was found anywhere in this IFU).

### 18.4 Settings editability

FACT: Settings are editable, and editability is permission-gated by a key-user/PIN system: "The key user decides if this user will be allowed to change preset applications," and a per-user power limit can restrict which presets a given user can even select ("when you choose a power limit of 2 W the user cannot choose a preset application with more than 2 W. If the power limit [is] 0.5 W (default), so the user has no access to preset applications.").

### 18.5 Tissue-response adjustment and minimum effective power

FACT: Tissue-response adjustment is explicitly recommended: "Parameters should be adjusted as needed according to the clinical conditions (e.g., level of bleeding, tissue type, etc.)" (Soft-Tissue Surgery); "Reduce power, if pain sensations appear" (periodontology presets).

FACT, and a genuine contrast with the three manuals reviewed in §6: SIROLaser Blue's IFU does **not** instruct the clinician to start at the lowest/minimum power and increase as needed. Instead its explicit warning cuts both directions: "The preset power levels are considered to be safe for patients. Increasing the power levels entails the risk of overheating the patient's soft or hard tissue. **Setting the power to excessively low levels may result in reduced treatment efficacy.**" This is the opposite emphasis from Biolase's and AMD's "always start at the lowest power setting" instruction (§6, §17.2) — SIROLaser Blue's IFU frames the factory preset itself as the safe reference point, and warns against moving power in either direction from it, rather than instructing the clinician toward a minimum.

### 18.6 Incision speed / dwell time

FACT: No numeric incision speed (e.g., mm/s) or numeric dwell/contact time is specified anywhere in the IFU for any surgical or periodontal preset. Qualitative movement technique is described instead ("keep the laser tip always in motion," "sinuous movement," "use the laser tip like a scalpel"), consistent with the §9 finding (Picasso/FOX/Epic) that manufacturer guidance addresses power and mode but not speed or dwell time as a quantified parameter.

### 18.7 Actual delivered power / calibration

FACT: This IFU gives the most detailed calibration guidance found among any manual reviewed in this vault to date. It describes:
- A **self-calibration** the device performs automatically ("The SiroLaser Blue performs a self-calibration. During this procedure, the system checks that the laser emission parameters are correct.").
- A **weekly manual calibration check** the manufacturer recommends the clinician perform ("We recommend performing this check at least once a week."), with specific numeric check points: 1 W at 445 nm, 1 W at 970 nm, 100 mW at 660 nm, each with a stated wavelength tolerance and "resolution: 5% or higher."
- An explicit recommendation to verify with an **external measuring instrument** at a longer interval: "We recommend that you check these values using a suitable external measuring instrument at least every twelve months."
- A **± 20% pass/fail tolerance** for the calibration check screen: "the tolerance of ±20%... Press 'Yes' on the screen if the measured value is within the tolerance of ±20%."

INTERPRETATION: The ± 20% tolerance figure matches the Biolase Epic 10/Epic X "Power Accuracy ± 20%" spec (§17.2) and the A.R.C. Laser FOX manual's stated ± 20% external power-meter check tolerance (§6, §8) — three independent manufacturers converge on the same ± 20% figure for how far delivered power is permitted to diverge from the set/displayed value before being flagged as out of tolerance. This is not evidence the actual deviation is bounded at ± 20% in practice (Xue et al. 2022's measured deviations for this same device, +21% to +37%, already exceed the manufacturer's own ± 20% band — see [[05 Devices/SIROLaser Blue]] and §8 above) — it only shows that ± 20% is the tolerance manufacturers themselves treat as their acceptance threshold, and that at least one independently measured dataset already exceeds it for this exact device.

### 18.8 Preset-validation evidence

NOT FOUND: No citation to a published study, dataset, or clinical trial behind any preset value was located anywhere in this IFU. Unlike Biolase (§6, §17: "based on clinical recommendations and feedback from experienced laser dentists"), SIROLaser Blue's IFU does not offer even a general, uncited provenance statement for its preset values — provenance is entirely unstated for this device.

### 18.9 Tip initiation

FACT: This IFU does not describe a tip-initiation procedure or concept anywhere (no equivalent of Biolase's "touch tip to initiation block, fire footswitch" protocol, §17.2). SIROLaser Blue's EasyTips are single-use, factory-sterilized, snap-fit tips with no user-performed initiation step described in the IFU. This is consistent with, but not confirmation of, the "uninitiated and new" tip condition reported in [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] and the initiated-tip protocol Romanos et al. 2022 applied as an independent experimental manipulation (dark-blue articulating paper) rather than a manufacturer-specified step — see [[05 Devices/SIROLaser Blue]] for that existing finding, not re-derived here.

## 19. Updated implications from the follow-up (§17–§18)

INTERPRETATION: Both follow-up findings **strengthen**, not weaken, this note's existing preset-reliability rationale (§13–§15), for different reasons:

1. **Epic X → Epic 10 TM (§17):** resolving this from "unconfirmed" to "directly confirmed, same values, both manuals silent on the same points" removes a caveat but does not change the substantive finding — both Biolase manuals independently confirm no incision-speed/dwell-time specification, no cited validation study, and a preset-provenance statement that is general and uncited. The uncertainty that is resolved is about *which document* the vault can rely on for Epic 10 TM, not about *whether presets are validated* — that finding is now on firmer ground (two independent primary manufacturer documents agree) but its content is unchanged.
2. **SIROLaser Blue (§18):** this is the vault's first look at a full manufacturer IFU for a device that already has independent measured-power evidence in this vault (Xue et al. 2022, [[05 Devices/SIROLaser Blue]]). It adds two findings not previously available for any device in this note: (a) a manufacturer-stated ± 20% calibration tolerance that Xue et al.'s independently measured deviation (+21% to +37%) already exceeds for this exact device — the clearest documented case in this vault of measured deviation exceeding the manufacturer's own stated acceptance band, not merely diverging from a bare console value; and (b) a manual that gives no preset-provenance statement at all (weaker disclosure than any of the three manuals reviewed in §6), while also being the one manual that does *not* instruct the clinician toward minimum effective power — a genuine cross-manufacturer inconsistency in preset philosophy, not just in preset values.

No source retrieved in this follow-up changes the vault's existing NOT FOUND findings in §2, §4, §5, §10, or §12 — those searches were not repeated here, and this follow-up is scoped to manufacturer documentation only, per the task that requested it.

## 20. สรุปภาษาไทย (เพิ่มเติม 2026-09-15)

- **Epic 10 TM กับ Epic X**: พบคู่มือผู้ผลิตฉบับจริงของ Epic™10 โดยตรง (ไม่ใช่การอนุมานจากคู่มือ Epic X) และพบว่าตารางค่าพรีเซ็ตทั้ง 14 หัตถการ ความยาวคลื่น (940±10nm) กำลังสูงสุด (10W) ค่าความแม่นยำ (±20%) และขนาดไฟเบอร์เหมือนกันทุกประการกับ Epic X ข้อสรุป: **สามารถใช้ข้อมูลร่วมกันได้ (transferable)** โดยไม่ต้องอาศัยการอนุมานอีกต่อไป เพราะมีคู่มือของ Epic 10 เองยืนยันโดยตรง
- **SIROLaser Blue**: เข้าถึงคู่มือ IFU ฉบับทางการ (2025-03) ได้สำเร็จผ่านเส้นทาง URL สำรอง พบว่าเครื่องนี้มี 3 ความยาวคลื่น (445/970/660 nm) ไม่ใช่ 2 ตามที่บันทึกไว้เดิม (660 nm ไม่มีพรีเซ็ต ใช้เฉพาะการบำบัดด้วยเลเซอร์กำลังต่ำ)
- คู่มือ SIROLaser Blue **ไม่ระบุที่มาของค่าพรีเซ็ตเลย** (ต่างจาก Biolase ที่อย่างน้อยระบุว่าอิงคำแนะนำทางคลินิก) และเป็นคู่มือเดียวที่ไม่แนะนำให้เริ่มจากกำลังต่ำสุด แต่เตือนว่าอย่าลดกำลังต่ำเกินไปเพราะจะลดประสิทธิภาพการรักษา
- ทั้งสองอุปกรณ์ **ไม่ระบุความเร็วในการตัดหรือเวลาสัมผัสเป็นตัวเลข** เหมือนคู่มืออื่นๆ ที่ตรวจสอบไปก่อนหน้านี้
- ค่าความคลาดเคลื่อนที่ยอมรับได้ ±20% ปรากฏตรงกันในผู้ผลิตอิสระ 3 ราย (Biolase, A.R.C. Laser, Dentsply Sirona) แต่ข้อมูลวัดจริงจาก Xue et al. 2022 สำหรับ SIROLaser Blue (+21% ถึง +37%) เกินขอบเขตนี้ไปแล้ว — เป็นกรณีแรกในคลังนี้ที่ค่าคลาดเคลื่อนที่วัดได้จริงเกินกว่าเกณฑ์ที่ผู้ผลิตกำหนดเอง

## Full-text verification of priority sources

**Date: 2026-09-15 (follow-up session).** The three sources named in §3, §7, and §12 as newly surfaced but not yet full-text-verified have now been added to Zotero and were read in full text (via the local Zotero library, PDF attachments confirmed present; `pdftotext -layout` extraction; full text read start to finish for all three, not abstract/summary only). This section reports what full text changes versus what was previously inferred from title/abstract alone. Per this task's explicit instruction, a review-level call for "standardization" is not treated as proof that manufacturer presets are validated, and legal-allegation outcomes are not treated as scientific proof of mechanism.

### Source 1 — Dashti et al. 2026, "Toward evidence-based laser dentistry: wavelength selection, parameter standardization and clinical outcomes" (Int J Community Med Public Health, doi:10.18203/2394-6040.ijcmph20263229)

**What it is:** a structured narrative review (not a primary study, not a systematic review with meta-analysis) surveying laser dentistry across nine clinical domains (periodontics/peri-implant, endodontics, restorative, prosthodontics, oral surgery, pediatric, orthodontics, photobiomodulation, aPDT), searched in PubMed/Scopus/Web of Science through July 2026. It never mentions dental diode-laser presets, factory/default settings, or manufacturer recommendations — confirmed by exhaustive keyword search of the full text (`preset`, `default setting`, `manufacturer.*recommend`, `factory`: zero matches).

FACT: The review states plainly that "laser-assisted dentistry is not a single intervention" and that "average power alone is therefore insufficient to reproduce treatment, and the power selected on the device may differ from that delivered at the fiber or handpiece tip" — citing Parker et al.'s delivery-power-losses study (their ref. 12), which is the same primary study already in this vault as [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] (title match: "The influence of delivery power losses and full operating parametry on the effectiveness of diode visible–near infra-red (445–1064 nm) laser therapy in dentistry — a multi-centre investigation," Lasers Med Sci 2022;37(4):2249-57). This is a citation of evidence this vault already holds, not new primary data.

FACT: "Accurate reporting should identify the target, wavelength, delivered output, pulse structure, irradiated area, exposure time, contact or non-contact mode, movement, cooling, and treatment repetition" — a call for complete **parameter reporting in published research studies**, not a statement about what clinicians should do chairside with a device's preset menu.

FACT: "Thermal injury remains the principal tissue-level hazard and is determined by pulse structure, **dwell time**, movement, cooling, and the properties of adjacent tissues or materials rather than nominal power alone" — this is the review's only use of "dwell time," stated once, generically, as a safety principle across all laser dentistry (not diode- or biopsy-specific, and not tied to any specific device or preset).

FACT: The conclusion calls for future research to prioritize "standardized, reproducible protocols and long-term clinical outcomes over device-centered claims of superiority," and for studies to report "device and wavelength, verified output at the treatment site, emission mode, pulse energy and duration, repetition rate, spot size, irradiance or radiant exposure... irradiation time, delivery geometry, movement, cooling, and treatment frequency." This is addressed to **researchers designing future clinical trials**, not to manufacturers writing IFUs or clinicians selecting chairside presets.

FACT: For soft-tissue oral surgery specifically, the review states technical perioperative benefits (hemostasis, reduced early morbidity) "are established for selected procedures," but "long-term superiority is not universal and biopsy margins require thermal caution," citing a systematic review (their ref. 58) confirming "all evaluated laser categories can produce histological thermal changes, with the extent depending on wavelength and operating parameters" — this ref. 58 is Tenore et al. 2023, already in this vault as [[07 Data/Tenore et al 2023 - Laser Thermal Effect Oral Biopsy Histology Systematic Review Data]].

INTERPRETATION: This review's central thesis — that laser dentistry is parameter-dependent and that current *published-study* reporting of those parameters is frequently incomplete — is consistent with, and lends independent 2026 secondary-source support to, this vault's existing primary-source finding (§8) that console/preset power is not a reliable proxy for delivered power. It strengthens the general "parameter reporting in the literature is inadequate" observation.

NOT ESTABLISHED: The review does not demonstrate, discuss, or even mention (a) manufacturer preset values, (b) preset provenance or validation, (c) clinician preset-selection behavior, (d) a link between clinician knowledge/training and preset reliance, or (e) any dental-diode-specific incision-speed or per-preset dwell-time specification. **Per the task's explicit instruction, this review's call for "standardization" in research reporting must not be read as evidence that manufacturer presets are validated — the review does not discuss manufacturer presets at all, in either direction.**

**Primary studies cited by this review worth citation-chasing (checked against this vault's `07 Data/` folder first):**
- **New, not yet in vault:** Suter VGA, Altermatt HJ, Bornstein MM. "A randomized controlled clinical and histopathological trial comparing excisional biopsies of oral fibrous hyperplasias using CO2 and Er:YAG laser." Lasers Med Sci. 2017;32(3):573-81 (their ref. 57). This is a **different** paper from the vault's existing [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)]] (Suter et al., "CO2 and diode laser for excisional biopsies of oral mucosal lesions," Schweiz Monatsschr Zahnmed 2010;120(8):664-671, PMID 21038754) — same senior author group, different comparator laser (Er:YAG vs. diode) and different year. A histopathological RCT of excisional biopsy margins is directly relevant to this vault's biopsy-quality project scope.
- **New, not yet in vault:** Parker S, Grzech-Leniak K, Cronshaw M, Matys J, Brugnera AJ, Nammour S. "Full operating parameter recording as an essential component of the reproducibility of laser-tissue interaction and treatments." Adv Clin Exp Med. 2024;33(6):653-6 (their ref. 11) — directly on-topic for the reproducibility/parameter-reporting angle this synthesis note already tracks; appears to be a commentary/position piece rather than a primary study, so its evidentiary weight should be checked before citing it as data.
- **Already in vault, confirmed by this citation check (no chase needed):** Hanke et al. 2021 (their ref. 16 = [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]]); Palaia et al. 2021 (their ref. 17 = [[07 Data/Palaia et al 2021 - 445 nm Diode Laser In Vivo Biopsy Thermal Effect Data]]); Tenore et al. 2023 (their ref. 58, matched above); Parker et al. 2022 delivery-power-losses (their ref. 12, matched above); Malcangi et al. 2023 "Therapeutic and adverse effects of lasers in dentistry" (their ref. 63, already cited in this synthesis note's §11).
- **Lower priority** (photobiomodulation-specific, not diode soft-tissue surgery/biopsy): Parker et al. 2019 systematic review of PBM delivery parameters (their ref. 9); Cronshaw et al. 2020 PBM dose-parameter meta-analysis (their ref. 10).

**Does this paper materially strengthen the preset-reliability rationale? PARTLY.** It strengthens the general, literature-wide "parameter reporting/standardization is inadequate" claim with an independent, current (2026) secondary source that cites primary evidence already in this vault — useful corroboration. It does **not** strengthen the specific preset-reliability claim (manufacturer preset provenance, preset validation, or clinician preset-selection behavior), because it never addresses manufacturer presets in any form. Citing it as evidence for preset unreliability specifically would overstate what it supports.

### Source 2 — Harini & Arjunkumar 2018, "Awareness of Laser Dentistry Among Dentists in Tanjore- A survey" (Biomed Pharmacol J, doi:10.13005/bpj/1530)

**What it measures, exactly:** A cross-sectional questionnaire study. **Population:** dentists practicing in Tanjore, Tamil Nadu, India (city of ~60 dental clinics, ~70 practicing dentists). **Sample size:** questionnaire distributed to 70 dentists; 28 responded (17 male, 11 female) — a 40% response rate. **Questionnaire domains, verified from the full text's Materials/Methods and Tables 1–3:**
- Part 1 (7 items): laser awareness ("aware that lasers are used in dental practice," "practiced laser dentistry before," "interest in dental laser"), self-reported hours of laser education received in dental college (0 hr / 1–3 hr / >4 hr), which specialty rotations included laser education, and which laser **types by name** (CO2, Er:Cr:YSGG, Diode, Er:YAG, Nd:YAG, Argon) the respondent knew of.
- Part 2 (34 items, 6 sections): true/false-style items on **what laser can be used for** in each specialty (e.g., "can laser be used for gingivectomy," "can laser be used for calculus removal," "can laser be used for caries detection") — clinical-indication knowledge, scored correct/incorrect, feeding a per-section knowledge score.
- Part 3 (19 items, 5 sections): general advantages of laser (less pain, less bleeding, less time, less anesthesia need), general tissue effects (hemostasis, ablation, decontamination — named as concepts, not linked to specific parameters), cost/expense perception, biggest deterrents to practice, and which laser type the respondent would like to have in practice.

Overall knowledge was scored 1–42 and classified adequate (29–42, 14% of respondents) / moderate (15–28, 46%) / inadequate (1–14, 39%).

**Domain-by-domain classification, per the task's required categories:**

| Domain | Classification | Basis |
|---|---|---|
| Population | DIRECTLY ASSESSED | Tanjore dentists, described explicitly |
| Sample size | DIRECTLY ASSESSED | 70 invited, 28 responded |
| Questionnaire domains | DIRECTLY ASSESSED | 3-part structure fully described in Methods |
| General laser awareness | DIRECTLY ASSESSED | "Aware lasers used in dental practice" item (96.4% yes); overall adequate/moderate/inadequate score |
| Formal laser training | DIRECTLY ASSESSED (self-reported exposure hours, not a validated competency instrument) | "Hours of dental laser education" (0/1–3/>4 hr) and which specialty courses included laser content |
| Wavelength knowledge | NOT ASSESSED | Zero questionnaire items ask for a wavelength value or wavelength-selection logic; "wavelength" and "nm" appear only in the paper's background/discussion text about other authors' devices, never in a questionnaire item |
| Power-setting knowledge | NOT ASSESSED | Zero occurrences of "power" or "watt" anywhere in the full text |
| CW/PW knowledge | NOT ASSESSED | Zero occurrences of "CW," "PW," or "continuous wave" |
| Pulse parameter knowledge | NOT ASSESSED | Zero occurrences of "pulse" in a questionnaire context |
| Laser–tissue interaction knowledge | INDIRECTLY ASSESSED | Part 3's "effect of laser on dental tissues" section asks whether respondents know laser produces hemostasis/ablation/decontamination as general concepts — this is awareness that an effect exists, not knowledge of how operating parameters modulate that effect |
| Confidence in parameter selection | NOT ASSESSED | No confidence-rating item of any kind; "interest in dental laser" (yes/no) is not a confidence measure |
| Actual parameter-selection behavior | NOT ASSESSED | Not observed or self-reported; the closest item is binary "practiced laser dentistry before" (yes/no), which records usage history, not parameter choices |
| Use of manufacturer recommendations | NOT ASSESSED | Never mentioned |
| Use of presets/default settings | NOT ASSESSED | The word "preset" does not appear anywhere in the full text |
| Manual adjustment behavior | NOT ASSESSED | Never addressed |
| Relationship between training and parameter selection | NOT ASSESSED | Cannot be assessed because parameter selection was never measured; the paper's Discussion does correlate *education hours* with *general knowledge score* ("the more education the dentists had, the more knowledge they gained about laser") — a narrower, already-general-knowledge-level finding, not a parameter-selection finding |
| Relationship between knowledge and preset use | NOT ASSESSED | Preset use was never measured, so no relationship to it can exist in this dataset |

**Critical-rule check:** this survey's Part 2/3 items assess *clinical-indication awareness* (what laser can be used for) and *general-benefit/effect awareness* (hemostasis, less pain), not parameter-selection knowledge (wavelength, power, CW/PW, pulse) in any form. Per the task's explicit rule, this is **not** relabeled "parameter-selection knowledge" anywhere in this update.

**Answers to the four explicit questions:**
1. Does it document general knowledge gaps? **YES** — directly, with a numeric distribution (14% adequate / 46% moderate / 39% inadequate) and named gap areas (dentin desensitization, pediatric applications, orthodontic etching were the least-known indications).
2. Does it document parameter-specific knowledge gaps? **NO** — it cannot, because it never asks a parameter-specific question (see table above).
3. Does it document preset reliance? **NO** — "preset" is not a construct this survey measures at all.
4. Does it directly link knowledge/training to preset reliance? **NO** — neither variable (parameter knowledge, preset reliance) was measured, so no such link could be tested, let alone found, in this study.

**Relevance to preset reliability:** none directly — this survey cannot speak to preset provenance, validation, or use. **Relevance to user-knowledge framing:** confirms and quantifies *general* dental-laser awareness gaps in one regional population, consistent with (and no stronger than) the other awareness surveys already logged in §3 of this note. **Implications for the ex vivo project:** none beyond what §3 already established — this full-text read closes out the "full-text review needed" flag left in §3/§5 for this specific source, with the result that it adds a numeric general-knowledge distribution but does not fill the parameter-knowledge or preset-reliance evidence gaps this note has already logged as NOT FOUND.

### Source 3 — Jahani-Sherafat et al. 2022, "A trend of Medical Negligence in Laser Therapy in the Capital City: A Nine-Year Survey" (J Lasers Med Sci, doi:10.34172/jlms.2022.29, PMC9841381)

**What it is:** a retrospective descriptive study of 383 laser-related medical-malpractice legal case files from the Coroner's Office of Forensic Medicine in Tehran, Iran, 2012–2020, across **all** fields of medicine using lasers (not dentistry-specific).

**Extraction, verified from full text:**
- **Clinical field involved:** Overwhelmingly dermatology/cosmetic (274/383 cases, 71.5%) and ophthalmology (62/383, 16.2%), plus general surgery, gynecology, anesthesiology, neurology, urology, and dentistry as minor categories.
- **Whether dentistry is included:** YES, but marginally — Table 1 lists "Dentists: 3 total complaints (1.05%), 2 of them within the paper's 'laser skin treatment scope' sub-analysis (0.72%)." No further detail (no case narrative, no procedure type, no laser type, no outcome, no cause-of-action breakdown) is given for these 3 cases anywhere in the paper.
- **Whether dental lasers are specifically involved:** UNCLEAR/NOT ESTABLISHED — the paper never states what procedure or laser type the 3 dentist-attributed cases involved. Given the paper frames "laser skin treatment scope" as a specific analytic subset, at least one of the 3 dentist cases may not even involve an intraoral or diode application.
- **Laser types:** the word "diode" does not appear anywhere in the full text (confirmed by exhaustive search). The paper's laser-type discussion is entirely dermatologic/ophthalmic (hair-removal lasers, LASIK, cataract, trabeculoplasty), never oral/dental diode systems.
- **Adverse events described:** burns (29.2%), burns+pigmentation (14.9%), burns+scars (9.9%), pigmentation (10.4%), eye/vision problems (15.7%), and smaller categories including 4 deaths (all reported as mole-removal/melanoma-related, i.e., dermatologic, not dental) — none attributed to a specific dental case.
- **Whether parameter selection is implicated:** NOT ESTABLISHED for any case, dental or otherwise — the paper reports only three aggregate legal fault-categories across all 383 cases ("lack of skill" 62.2%, "improper treatment" 26%, "negligence" 11.8%), none of which is defined in terms of a specific laser parameter (power, wavelength, pulse mode, dwell time).
- **Whether excessive power is implicated:** NOT ESTABLISHED — "power" and "watt" do not appear anywhere in the full text.
- **Whether prolonged dwell/movement technique is implicated:** NOT ESTABLISHED — not discussed for any case.
- **Whether operator error is implicated:** ATTRIBUTED BY SOURCE, but only in aggregate and only as the legal category "lack of skill" (a coroner's-office fault-liability finding, not a mechanistic description of what the operator did wrong) — and this attribution is never broken out by specialty, so it cannot be confirmed for the 3 dental cases specifically.
- **Whether training deficiency is implicated:** POSSIBLE, discussion-level only — the paper's Discussion and Conclusion argue generally that "a lack of comprehensive surveillance of laser operators' training" and "untrained operators" are contributing factors nationally, especially for non-physician hair-removal operators; this is the authors' discussion-section interpretation applied to the dataset as a whole (mainly dermatology/hair-removal), not a finding attributed to any dental case.
- **Whether equipment malfunction is implicated:** NOT ESTABLISHED — "malfunction" and equipment-failure language do not appear anywhere in the full text; the entire fault analysis is operator/process-centered, not device-centered.
- **Whether causality is actually established:** NOT ESTABLISHED in the scientific sense for any case. The paper reports **legal fault-liability determinations** by a coroner's office (i.e., a legal/administrative judgment process), not a mechanistic or scientific causal analysis. 62.4% of decided cases were "fault liability in paid judgment" — a legal outcome category, not a verified causal chain from a specific technical error to a specific injury.
- **Whether cases are medico-legal allegations, judgments, incident reports, or observational records:** **medico-legal judgments/decisions** — official coroner's-office case files with recorded verdicts (fault/innocence/closed-without-vote), not clinical incident reports and not an observational clinical dataset.

**Critical-rule check:** per the task's explicit rules, this update does **not** treat the paper's legal fault-liability findings as scientific proof of mechanism, does **not** apply the word "malpractice" beyond what the source itself already uses (the source's own title and framing already use "malpractice"/"negligence" as its subject matter, so using those terms to describe *what the source is about* is source-faithful; but no additional finding is elevated to "malpractice" beyond what the coroner's office itself adjudicated), and does **not** generalize this paper's overwhelmingly dermatologic/ophthalmic findings to dental diode-laser use — the 3 dental cases carry no case-level detail that could support such a generalization.

**Relevance classification: CONTEXT ONLY.** This source establishes that laser-related medico-legal claims exist and are rising *in general medical/cosmetic laser use* in one jurisdiction (Tehran, Iran), and that "lack of skill" and "improper treatment" are the dominant legal fault categories found *in that overwhelmingly non-dental dataset*. It provides essentially no case-level, laser-type-level, or parameter-level detail for the 3 dental cases it does contain, and diode lasers are never mentioned. It cannot support any dental-diode-specific claim about parameter misuse, preset misuse, or technical-misuse mechanism — it can only be cited, if at all, as background evidence that laser-related medico-legal risk exists as a general phenomenon, consistent with this note's existing §12 treatment of it as context rather than mechanistic evidence.

**Relevance to preset reliability:** NONE — presets, default settings, and manufacturer recommendations are never mentioned. **Relevance to user-knowledge/misuse framing:** weak/context-only — the paper's own Discussion and Conclusion argue for more operator training and supervision in general laser medicine, which is thematically adjacent to this note's §3/§5 training-gap material, but provides no dental-specific or parameter-specific evidence to strengthen that argument for this project. **Implications for the ex vivo project:** none — this source cannot be used to support a "misuse" or "malpractice" framing for dental diode-laser preset use, and this update recommends it continue to be treated exactly as §12 already treats it: context only, not mechanistic evidence, with no causal inference drawn about this project's ex vivo hypotheses.

### Cross-source synthesis

1. **Does the 2026 standardization paper strengthen the claim that current laser parameter reporting/standardization is inadequate?** YES, for published-study reporting quality specifically (citing evidence already in this vault). This is a literature-reporting-quality claim, not a clinical-practice claim.
2. **Does it directly support manufacturer preset unreliability, or only broader parameter-standardization concerns?** Only the broader concern. It never discusses manufacturer presets in any form (zero mentions, confirmed by exhaustive keyword search).
3. **Does Tanjore 2018 support general knowledge gaps only, or parameter-specific gaps?** General knowledge gaps only — confirmed by exhaustive keyword search showing zero parameter-related questionnaire items (no power, pulse, CW/PW, or wavelength-selection items exist in the instrument).
4. **Is there now any direct evidence that knowledge gaps cause preset reliance?** NO. None of the three sources measures preset reliance at all, so none can establish this link. This vault's existing §5 finding (searched for directly, 0 PubMed results, NOT FOUND) is unchanged and now further corroborated — three additional full-text-verified sources, read specifically with this question in mind, also fail to supply it.
5. **Does the negligence paper provide dental-laser-specific evidence of parameter misuse?** NO. Dentistry is 3/383 cases (0.78%) with zero case-level detail; diode lasers are never mentioned; no case (dental or otherwise) is broken down by parameter.
6. **Does it justify "misuse," "abuse," or "malpractice" framing for this project?** NO. It documents general laser-medicine legal risk (overwhelmingly dermatologic/ophthalmic) and legal fault-liability outcomes, not a scientifically established mechanism of dental-diode-laser technical misuse. Using it to justify a misuse/malpractice framing for this project's dental-diode-laser scope would be a generalization the source does not support — exactly the error the task's critical rules warn against.
7. **Does any of these three sources weaken the current preset-reliability rationale?** NO. None contradicts the existing device-documentation findings (§6–§8, §17–§18) about preset provenance, ±20% tolerance, or absence of incision-speed specification. They simply do not add or subtract evidence at the clinician-behavior layer.
8. **Does any source require changing the current research question?** NO. Nothing here invalidates the current framing, so per this task's instruction, the canonical RQ, novelty matrix, and main literature review are **not** edited in this pass.
9. **Does any source materially strengthen the rationale enough to justify updating the main literature review?** NO — for the same reason as above. The 2026 review offers corroborating secondary-source context (already-cited primary studies, general reporting-inadequacy framing) rather than new primary findings; Tanjore 2018 adds a numeric general-knowledge distribution but no parameter- or preset-level data; the negligence paper adds essentially no dental-relevant data. None crosses the bar of "materially changing" an existing finding.

## Related notes

- Project: [[01 Projects/Diode Laser Biopsy]]
- Evidence: [[04 Evidence/Set Power vs Measured Output]]
- Data: [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]], [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]], [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]], [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]], [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data]], [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data]], [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]], [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data]]
- Devices: [[05 Devices/Epic 10 TM]], [[05 Devices/A.R.C. Laser FOX (810 nm)]], [[05 Devices/A.R.C. Laser FOX (980 nm)]], [[05 Devices/A.R.C. Laser FOX (1064 nm)]], [[05 Devices/Device Index]]
- Concepts: [[03 Concepts/Laser Presetting]], [[03 Concepts/Power Output]], [[03 Concepts/Power Loss]], [[03 Concepts/Operating Parameters]]
- Search report: [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Report - Preset Reliance and Technical Misuse]]
- Follow-up search log (§17–§19, 2026-09-15): [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Log - Epic 10 and SIROLaser Blue Manual Verification 2026-09-15]]
- Full-text-verified priority sources (2026-09-15, see "Full-text verification of priority sources" section above): Dashti et al. 2026, doi:10.18203/2394-6040.ijcmph20263229 (Zotero item GVLHRDJW); Harini & Arjunkumar 2018, doi:10.13005/bpj/1530 (Zotero item BHB6D8MS); Jahani-Sherafat et al. 2022, doi:10.34172/jlms.2022.29, PMC9841381 (Zotero item 3A8F39GH). These three are in Zotero with attached full-text PDFs but do not yet have ZotLit-synced `02 Literature/` notes in this vault as of this update — cited here directly by DOI/Zotero key per the vault's ingestion policy for sources ahead of their `02 Literature`/`07 Data` note creation.
