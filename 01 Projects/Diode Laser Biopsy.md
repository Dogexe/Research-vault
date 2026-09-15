# Diode Laser Biopsy

Primary research dashboard for this vault. Companion/secondary hub: [[01 Projects/Diode Laser Master]], which holds general diode-laser technical background (power output, calibration, device research) and now supports this project rather than competing with it.

This is a dashboard, not a processing log. Detailed paper-by-paper processing history lives in [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]; cross-study conclusions live in `06 Synthesis/`; structured per-paper extractions live in `07 Data/`.

**Reframed 2026-09-13.** This project was previously framed around clinical diagnostic-biopsy outcomes. It is now an **ex vivo experimental study** of oral soft-tissue cutting. Diagnostic biopsy outcome is retained as clinical relevance/background context, not as the primary experimental endpoint. See [[#Why this project was reframed]] below.

## Scope

Experimental ex vivo oral soft-tissue cutting with diode lasers, testing **preset reliability**: whether a manufacturer/device preset and the console-set power it produces reflect the power actually delivered to tissue, and whether either reflects **histopathologic specimen quality**, under a controlled incision speed. This is a mechanistic/methodological study of preset reliability — not a clinical trial, not a study of clinician behavior or training, and not an inquiry into misuse or malpractice. Clinician knowledge, training, and preset-reliance behavior are addressed only as literature context, in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] — they are not premises this experiment depends on, and the experiment does not require any clinician to have done anything wrong for its results to matter.

Primary experimental endpoint terminology used throughout this vault going forward: `histopathologic specimen quality` or `biopsy-oriented histopathologic specimen quality`. Thermal damage alone is not equated with total specimen quality — specimen quality is treated as a composite of thermal artifact, margin readability, and tissue architecture preservation, per [[#Primary experimental outcomes]] below.

## Canonical research question

> To what extent do diode laser preset settings reflect actual delivered power and predict histopathologic quality of ex vivo oral soft-tissue specimens under controlled incision speeds?

## Research rationale

This project does not ask which preset is "best," and it does not ask whether ex vivo findings predict clinical diagnostic success, prove clinical harm, prove operator misuse, or support a malpractice/negligence claim — none of those follow from an ex vivo design, and none is assumed here.

- **Preset ≠ delivered power.** A stored/named manufacturer preset sets a console value; console-set power is not assumed to equal the power actually delivered to tissue. This vault's own device-provenance evidence shows manufacturers stating this directly: the A.R.C. Laser FOX manual states the displayed value "may vary from the emitted value at the distal tip, by a range of ±20%," and separately instructs that stored presets do "not release the surgeon from checking the values according to his knowledge and the desired interaction with the tissue" (see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §6–§8).
- **Preset is not automatically a biological dose.** A factory preset is, by manufacturers' own description, derived from general clinical recommendation or practitioner feedback (e.g., Biolase's Epic X manual: "procedure pre-sets installed at the factory are based on clinical recommendations and feedback from experienced laser dentists") — not from a published, cited dose-response study tying that preset to a measured tissue effect. A preset existing, or being labeled for a named procedure, is not evidence that it was validated against delivered power or histologic outcome.
- **Incision speed modifies exposure.** The same preset/set power delivers a different tissue exposure at a different incision speed; no device manual reviewed in this project specifies incision speed or dwell time alongside its power presets (see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §9). A preset that specifies power but not speed incompletely defines tissue exposure.
- **Ex vivo findings do not prove clinical harm, misuse, or malpractice.** Thermal artifact is not assumed to equal reduced histopathologic quality by itself — quality is assessed across thermal artifact, margin readability, and tissue architecture preservation together. No "optimal setting" is claimed unless evidence directly supports it. Ex vivo histologic findings are not claimed to translate directly to clinical diagnostic outcomes, to demonstrate that any clinician used a device incorrectly, or to support any medico-legal conclusion — those require separate clinical, behavioral, and legal evidence entirely outside this project's ex vivo scope.

Procedure-based presets may simplify parameter selection for clinicians, but their evidentiary provenance, their relationship to actual delivered power, and their ability to predict tissue effect may be incompletely established — see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] for the full evidence review behind this statement. Actual tissue exposure may also depend on device-to-device output variation, fiber transmission loss, fiber-tip condition/initiation, tissue properties, and incision speed/operator movement — all independent of whatever the preset or console display shows. Testing preset/set power against independently measured delivered power and histopathologic effect, under a controlled incision speed, is therefore practically relevant regardless of how any individual clinician selects or adjusts that preset. See [[#Practical relevance]] below.

## Logic chain

`Manufacturer / device preset` → `console set power` → `actual delivered power` → `controlled incision speed` → `tissue interaction` → `thermal / structural alteration` → `histopathologic specimen quality`

This chain is deliberately split into two links at the front — `manufacturer/device preset` and `console set power` — rather than treated as one, because a stored preset is a named factory- or clinician-programmed parameter set (e.g., Biolase Epic X's "Gingivectomy/Gingivoplasty" preset), while the console-set power is whatever value is actually dialed in for a given incision, whether by recalling that preset unmodified or by manual override. Collapsing the two would hide exactly the distinction this project tests: a device can have a labeled preset without that label guaranteeing either the console value used or the power delivered. Modifiers of this chain, tracked alongside each link where relevant: wavelength, fiber diameter, tip initiation status, contact vs. non-contact mode, CW vs. PW, pulse parameters (duration, frequency, duty cycle).

The `console set power` → `actual delivered power` link is supported by this vault's existing power-output/power-loss evidence — see [[04 Evidence/Set Power vs Measured Output]] and [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]]. The `manufacturer/device preset` → `console set power` link is newly supported by manufacturer manual evidence gathered for this reframing — see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §6–§7. The remaining links (incision speed onward) are this project's own experimental focus.

## Primary experimental outcomes

**Primary candidates** (biopsy-oriented specimen-quality endpoints — closest to what a pathologist would need to assess):
- Thermal damage width
- Margin readability
- Preserved tissue architecture
- Epithelial thermal artifact
- Connective-tissue thermal artifact

**Secondary candidates** (mechanistic/technical endpoints):
- Carbonization
- Coagulation zone
- Incision depth
- Incision width
- Cutting efficiency

This is a candidate outcome list, not a finalized protocol — it is not converted into a specific measurement instrument or scoring scale here.

## Key variables

**Exposure/operating (experimental):** wavelength, preset/set power, independently measured delivered power, average/peak power, CW vs. pulsed mode, pulse duration, frequency, duty cycle, fiber diameter/spot size, initiated vs. non-initiated tip, contact vs. non-contact mode, incision speed, exposure duration, number of passes, movement technique, cooling (if reported).

**Incision speed** is treated as a controlled experimental variable, and every source is classified by how its speed value was obtained — this distinction is preserved, not collapsed:
- Mechanized (instrument-controlled, e.g. 3D micropositioner)
- Clinician-controlled (manual, target speed only)
- Measured (instrument- or timer-derived outcome value, distinct from a target)
- Reported descriptive movement (qualitative only, no number)
- `UNKNOWN`

Speed is never inferred from procedure duration.

**Delivered power** is likewise treated as a key experimental variable, and every source is classified by: console-set power vs. measured output; meter used; measurement location; measurement timing (once at setup vs. before every incision); acceptable deviation threshold (if any); and whether the measured value was actually used as the reported experimental exposure value, or only as a setup check. See [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] for the vault's most rigorous examples of this distinction (per-incision verification, not a one-time setup check).

**Specimen/tissue outcomes:** thermal damage, histological artifact, coagulation zone, carbonization, margin readability, epithelial/connective-tissue artifact, tissue architecture preservation, incision depth/width.

No missing parameter is inferred; absent values are marked `UNKNOWN`.

## Current evidence status

Sources are now classified into three roles, kept visibly distinct rather than pooled:

- **EXPERIMENTAL / TECHNICAL PRECEDENT** — ex vivo, mechanistic, directly relevant to this project's experimental design: [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] (closest precedent — see [[#Hanke and Strakas as direct prior art]] below), [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]], [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]], [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] (closest ex vivo biopsy-oriented histologic precedent), [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]], [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] (added 2026-09-14 — measured power with a reported numeric value + histology in ex vivo oral tissue, but no reported incision speed and not biopsy-oriented; see [[04 Evidence/Power Output and Tissue Effect]]), [[07 Data/Wilder-Smith et al 1995 - CO2 Laser Incision and Thermal Damage Data|Wilder-Smith et al. 1995]] (CO2, methodological reference only), and this vault's broader output/calibration/speed literature (Parker, Xue, Zegaib, Kim, and others catalogued in [[01 Projects/Diode Laser Master]]).
- **CLINICAL RELEVANCE / OUTCOME CONTEXT** — human in vivo diagnostic-biopsy studies, kept as background showing which histologic alterations matter clinically and when thermal artifact does or does not compromise interpretation, but not treated as direct experimental matches to this project's ex vivo design: [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield|Angiero et al. 2011]], [[07 Data/Palaia et al 2021 - 445 nm Diode Laser In Vivo Biopsy Thermal Effect Data|Palaia et al. 2021]], [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]], [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)|Suter et al. 2010]], [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data|Gambino et al. 2026]], [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]], [[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]], and — added 2026-09-14 — [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data|Monteiro et al. 2019]] (six-instrument human comparison including diode) and [[07 Data/Gobbo et al 2017 - Blue vs Infrared Diode Laser Biopsy Thermal Damage Data|Gobbo et al. 2017]] (two-wavelength diode human comparison), plus non-diode outcome-methodology precedent [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data|Vescovi et al. 2010]] (Nd:YAG, specimen-size effect) and [[07 Data/Seoane et al 2013 - Er,Cr YSGG Leukoplakia Pseudodysplastic Artifact Data|Seoane et al. 2013]] (Er,Cr:YSGG, blinded two-pathologist consensus) — none of the four independently measures power or reports incision speed, so none changes this project's novelty conclusion (see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]). [[07 Data/Tenore et al 2023 - Laser Thermal Effect Oral Biopsy Histology Systematic Review Data|Tenore et al. 2023]] (28-study systematic review) was processed as a secondary, citation-mining source only — not primary evidence. And others already processed. **Gundlapalle et al. 2022's pathologist-graded slide-quality score (good/average/poor/non-diagnostic) is this vault's strongest existing clinical analog for what a specimen-quality outcome instrument should measure** — retained here specifically for that methodological reason, not as an experimental match.
- [[04 Evidence/Power Output and Tissue Effect]] — the central bridge node, now **PARTIAL EVIDENCE** rather than a placeholder: measured power + histology in ex vivo oral tissue is demonstrated (Hanke 2021, Strakas 2023, Goharkhay 1999, and — added 2026-09-14 — [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]]). What remains NEEDS EVIDENCE is specifically an **oral, biopsy-oriented, ex vivo** design. Hanke 2021 and Strakas 2023 pair independently measured power with a controlled speed and histologic thermal-effect outcome in oral (gingival) tissue — but neither uses a biopsy-oriented specimen-quality outcome framework (margin readability, tissue architecture preservation); both are cutting-efficiency characterization studies. Prado 2022 adds a numerically reported measured-power value but no incision speed and no biopsy-oriented outcome. See [[#Hanke and Strakas as direct prior art]].
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] — full comparison table and narrowed novelty conclusion, updated for the ex vivo reframing.
- Device-level status: [[05 Devices/Device Index]] — no device in this vault currently has both an independently measured output value and a biopsy-oriented ex vivo specimen-quality outcome from the same or cross-referenced source.

## Why this project was reframed

The prior framing implied this project directly measures clinical diagnostic-biopsy success. That overstated what an ex vivo design can show. The project is repositioned as an experimental ex vivo study whose outcomes are histopathologic specimen-quality measures (thermal artifact, margin readability, tissue architecture preservation) — mechanistically informative, but requiring separate clinical validation before any diagnostic-success claim could be made. No prior evidence or novelty search was deleted; clinical biopsy literature is retained as context, repositioned as described above.

## Hanke and Strakas as direct prior art

[[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] are treated as **direct prior art for this project's experimental design**, not merely supporting evidence:

| | Hanke et al. 2021 | Strakas et al. 2023 |
|---|---|---|
| Tissue model | Porcine gingiva, ex vivo — **oral tissue** | Porcine gingiva, ex vivo — **oral tissue** |
| Measured power method | Calibrated power meter (LabMax Top + PM10 detector, Coherent), checked before **every single incision**, ≥5% deviation triggers fiber-tip replacement | Identical protocol and instrument, same senior author (J. Meister) |
| Measurement location | Distal end of the fiber | Distal end of the fiber |
| Controlled incision speed | 2 mm/s, mechanized via 3D micropositioner (VT-80, Micos) | 2 mm/s, identical device and protocol |
| Histologic outcomes | Cut depth/width, total interaction zone (TIZ) depth/width, 5-class morphological classification, efficiency factor γz | Same outcome set, extended to 940 nm across 9 power levels |
| Oral tissue used? | YES | YES |
| Specimen margins assessed? | NO — no excised lesion/specimen with a margin; TIZ measures thermal spread around a linear incision in a healthy tissue block, not a biopsy specimen margin | NO — same design |
| Biopsy-oriented? | NO — framed entirely around cutting-efficiency/therapeutic-protocol optimization, never as specimen excision or diagnostic-analog quality assessment | NO — same framing |
| Lesion excision / diagnostic tissue architecture involved? | NO — standardized linear incisions in non-lesional tissue blocks; no architecture-preservation or specimen-quality scoring instrument used | NO — same design |

**How the proposed ex vivo oral model differs:** not on tissue type (both already use oral gingiva) and not on the measured-power + controlled-speed + histology combination (both already close that). The difference is in the **outcome framework**: Hanke and Strakas quantify cutting mechanics (depth, width, thermal-interaction-zone ratio) for surgical-protocol optimization. Neither excises a specimen, scores margin readability, or grades tissue architecture preservation the way a pathologist would assess a diagnostic specimen. The proposed project's distinguishing contribution, if it exists, is applying this same measured-power + controlled-speed rigor to a **biopsy-oriented specimen-quality outcome set** (margin readability, tissue architecture preservation, peri-incisional alteration graded as a diagnostic-analog specimen) — not to the underlying power/speed measurement design itself, which has precedent.

The closest existing approximation of that biopsy-oriented outcome framework, still short of it, is [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] (ex vivo sheep tongue, ordinal epithelial/connective-tissue damage scores + lateral thermal damage extent — but no independently measured power) and [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]] (in vivo human, pathologist-graded slide quality — but not ex vivo, and no independently measured power or speed). See [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the full cross-tabulation.

## Major contradictions

See [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]] for full sourcing. Headline conflicts, kept visible rather than averaged:

- **CW vs. PW thermal-damage direction** — three discordant patterns across independent sources (Gundlapalle et al. 2022 and Romanos et al. 2022: PW < CW damage; Pergolini et al. 2025: PW > CW, not significant; Goharkhay et al. 1999: no consistent direction).
- **Margin-size recommendation** — ≥5 mm (Angiero 2011, Romeo 2014, Gambino 2026, Gundlapalle 2022, all clinical-relevance/diagnostic-biopsy pathways) vs. ≥2 mm (Pergolini 2025, ex vivo, no diagnosis rendered). These sit in different roles (clinical relevance vs. experimental precedent) and are not treated as directly comparable margin standards.
- **Set power vs. actual delivered power** — established as a real, measured gap by this vault's power-output evidence ([[04 Evidence/Set Power vs Measured Output]]); Hanke 2021 and Strakas 2023 close this gap methodologically in oral ex vivo tissue, but not within a biopsy-oriented outcome design.
- **Carbonization vs. nominal power** — no clean power-dependence of thermal-damage-zone width found by two independent sources (Pergolini 2025, Goharkhay 1999), which complicates the informal assumption that higher power alone drives more damage.

## Main research gaps

See [[06 Synthesis/Research Gaps in Dental Diode Laser Output]] and the processing log for full sourcing.

- **No ex vivo oral soft-tissue diode study integrates independently measured delivered power, controlled incision speed, and a biopsy-oriented specimen-quality outcome framework (margin readability, tissue architecture preservation) in one design.** This is this project's central, still-open gap, now stated at the correct level of precision — it is not simply "measured power + speed + histology" (Hanke 2021/Strakas 2023 already provide that).
- No source varies incision speed as an independently varied experimental variable against specimen-quality outcome (only fixed, non-transferable speed values exist across different sources: 10 mm/s, 2 mm/s, 1 mm/s, 0.75 mm/s).
- No source defines or applies a formal margin-readability or tissue-architecture-preservation scoring instrument in an ex vivo design with independently measured power — Gundlapalle et al. 2022's pathologist-graded slide-quality scale is the closest existing instrument, but it is in vivo, set-power-only.
- Coagulation-zone evidence for dental diode lasers remains abstract-level only (Capodiferro et al. 2008), unverifiable at full-text.
- No source directly compares initiated vs. non-initiated tip status under otherwise controlled conditions while independently measuring delivered output, in a biopsy-oriented ex vivo design. (Narrowed 2026-09-14: [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] pairs an initiated tip with independently measured, numerically reported power, but uses an initiated tip throughout with no non-initiated comparator, so it narrows without closing this gap. See [[06 Synthesis/Research Gaps in Dental Diode Laser Output]] §1.)

## Key synthesis links

- [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] — study-level parameter-vs-outcome mapping; now separates clinical, ex vivo experimental, and technical/measured-output studies rather than pooling one range.
- [[06 Synthesis/Diode Laser Biopsy Specimen Quality]] — cross-study synthesis of thermal artifact, margins, and diagnostic quality (clinical-relevance context).
- [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]] — the conflicts above, in full.
- [[06 Synthesis/Research Gaps in Dental Diode Laser Output]] — gap analysis for the underlying power-output evidence.
- [[06 Synthesis/Novelty Check - Prior Systematic Review]] — cross-check against Lopes-Santos et al. 2023 (a clinical systematic review); retained as clinical-relevance context for the diagnostic-biopsy literature, not the primary novelty check for this project's current ex vivo framing.
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] — the primary, current novelty cross-tabulation for the ex vivo experimental framing. Label: **POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION.**

## Potential novelty (current framing)

> Potential novelty: evaluating whether preset/set power reflects actual delivered power and predicts biopsy-oriented histopathologic specimen quality under controlled incision speed, in an ex vivo oral soft-tissue model.

This is deliberately narrower than treating "measured power + speed + diagnostic biopsy outcome" as the novel combination, because [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] already demonstrate measured power + controlled speed + histology together — novelty cannot be claimed from those three elements alone, and this remains this project's direct prior art (see [[#Hanke and Strakas as direct prior art]]). The reframing toward **preset reliability** adds a distinct axis that Hanke/Strakas do not test: both studies use researcher-selected bench power levels, not a manufacturer-labeled procedural preset, so neither speaks to whether a *named preset* — the thing a clinician actually recalls on a device panel — reliably predicts delivered power or tissue effect. The search conducted for this reframing ([[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]]) did not find any source, dental or otherwise, that pairs a manufacturer-labeled preset with both independently measured delivered power and a biopsy-oriented histologic outcome under controlled speed. The remaining novelty therefore rests on three elements together: (1) testing a preset *as labeled* — not merely a bench power value — against independently measured delivered power; (2) the biopsy-oriented outcome framing (margin readability, tissue architecture preservation, peri-incisional alteration graded as a diagnostic-analog specimen); and (3) integrating both with a controlled incision speed in a single ex vivo oral soft-tissue design. **Label: POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION.** Not "no study exists," not "first ever" — see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] and [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] for the full, cautious statements and their stated search limitations.

## Practical relevance

If a preset label does not reliably predict delivered power, and delivered power (jointly with incision speed) does not reliably predict histopathologic specimen quality, then treating a preset name as a proxy for tissue exposure is unsound for any procedure — including biopsy — where specimen quality affects diagnostic accuracy. This holds regardless of whether any individual clinician selected, adjusted, or overrode the preset correctly: it is a question about what the preset itself can be trusted to represent, not about clinician competence. Practical relevance therefore does not depend on establishing misuse, inadequate training, or negligence — see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §13–§14 for why this project does not adopt a misuse-based framing. If presets prove unreliable as a proxy for either delivered power or tissue effect, the practical implication is methodological (independent power verification and explicit speed control may be necessary alongside any preset-based protocol for biopsy-oriented use), not disciplinary.

## Immediate next steps

1. Define a formal margin-readability and/or tissue-architecture-preservation scoring instrument suitable for an ex vivo (non-lesional) oral soft-tissue specimen — the still-missing methodological piece Hanke 2021/Strakas 2023/Al-Ani 2024 each partially approximate but none fully provides.
2. Search specifically for an ex vivo oral-diode study that pairs a manufacturer-labeled preset (not just a researcher-selected bench power value), calibrated power-meter measurement, and a biopsy-oriented (not merely cutting-efficiency) histologic outcome — do not assume none exists without a targeted search.
3. Continue tracking incision speed as an explicit, extracted variable, classified by how it was obtained (mechanized / clinician-controlled / measured / descriptive / UNKNOWN) in every newly processed paper; never infer it from procedure duration.
4. For each device used in the eventual experimental design, document that device's own manufacturer preset table and stated provenance (named procedure, power/mode/pulse parameters, and whatever derivation basis the manual gives) before treating any console value as "the preset" — following the manual-extraction approach demonstrated for the Picasso, A.R.C. Laser FOX, and Biolase Epic X/Epic 10 TM platforms in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §6.
5. Do not fold clinician training gaps, preset-reliance behavior, or technical-misuse questions into the ex vivo experimental design as required premises — per [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]], direct evidence linking training gaps to preset reliance was not found, and this project's practical relevance does not depend on that link existing (see [[#Practical relevance]]).
6. Re-evaluate whether Capodiferro et al. 2008's coagulation-zone claim can ever be verified (no full text, no PMCID) or should be treated as permanently abstract-level.
7. If a clinical validation phase is ever proposed, treat it as an explicitly separate follow-on question — not folded into this project's current ex vivo scope.

## Related notes

- [[01 Projects/Diode Laser Master]]
- [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]
- [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]

## สรุปภาษาไทย

- โครงการนี้เป็นแดชบอร์ดวิจัยหลักของคลังนี้ **ปรับกรอบใหม่เมื่อ 2026-09-13** จากเดิมที่เน้นผลการวินิจฉัยทางคลินิก มาเป็น**การศึกษาทดลอง ex vivo** ของการตัดเนื้อเยื่ออ่อนในช่องปากด้วยเลเซอร์ไดโอด
- คำถามวิจัยหลักใหม่: พารามิเตอร์การทำงานของเลเซอร์ไดโอด กำลังขาออกที่ส่งจริง และความเร็วในการตัด ส่งผลต่อคุณภาพทางจุลพยาธิวิทยาของชิ้นเนื้อเนื้อเยื่ออ่อนในช่องปากแบบ ex vivo อย่างไร
- ห่วงโซ่ตรรกะใหม่: ค่าตั้งเครื่อง → กำลังที่วัดได้จริงอย่างเป็นอิสระ → ความเร็วตัดที่ควบคุม → ปฏิกิริยาต่อเนื้อเยื่อ → การเปลี่ยนแปลงจากความร้อน/โครงสร้าง → คุณภาพชิ้นเนื้อทางจุลพยาธิวิทยา
- ผลการวินิจฉัยทางคลินิกยังคงเก็บไว้เป็นข้อมูลบริบท (clinical relevance) ไม่ใช่จุดยุติหลักของการทดลองอีกต่อไป
- **Hanke et al. 2021 และ Strakas et al. 2023 ถือเป็นต้นแบบโดยตรง (direct prior art)** ของการออกแบบการทดลองนี้ — ทั้งสองมีการวัดกำลังจริง + ความเร็วควบคุม + ผลจุลพยาธิวิทยาในเนื้อเยื่อช่องปาก (เหงือกหมู) แล้ว แต่ใช้กรอบผลลัพธ์แบบประสิทธิภาพการตัด ไม่ใช่กรอบคุณภาพชิ้นเนื้อแบบ biopsy (ไม่มีการให้คะแนนความอ่านง่ายของขอบชิ้นเนื้อหรือการรักษาโครงสร้างเนื้อเยื่อ)
- ความใหม่ที่เหลืออยู่ (ระมัดระวัง ไม่กล่าวเกินจริง): การผนวกกำลังที่วัดได้จริง + ความเร็วควบคุม เข้ากับกรอบการประเมินคุณภาพชิ้นเนื้อแบบ biopsy-oriented ในแบบจำลอง ex vivo เนื้อเยื่อช่องปาก — ยังไม่มีแหล่งข้อมูลใดทำครบทั้งหมดนี้
- ไม่มีการอ้าง "ไม่มีการศึกษาใดเลย" หรือ "เป็นครั้งแรก" ในบันทึกนี้
