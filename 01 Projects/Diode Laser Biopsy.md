# Diode Laser Biopsy

Primary research dashboard for this vault. Companion/secondary hub: [[01 Projects/Diode Laser Master]], which holds general diode-laser technical background (power output, calibration, device research) and now supports this project rather than competing with it.

This is a dashboard, not a processing log. Detailed paper-by-paper processing history lives in [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]; cross-study conclusions live in `06 Synthesis/`; structured per-paper extractions live in `07 Data/`.

**Reframed 2026-09-13.** This project was previously framed around clinical diagnostic-biopsy outcomes. It is now an **ex vivo experimental study** of oral soft-tissue cutting. Diagnostic biopsy outcome is retained as clinical relevance/background context, not as the primary experimental endpoint. See [[#Why this project was reframed]] below.

## Scope

Experimental ex vivo oral soft-tissue cutting with diode lasers, focusing on how operating parameters, actual delivered power, and incision speed influence **histopathologic specimen quality** — not clinical diagnostic-biopsy success. This is a mechanistic/methodological study design, not a clinical trial.

Primary experimental endpoint terminology used throughout this vault going forward: `histopathologic specimen quality` or `biopsy-oriented histopathologic specimen quality`. Thermal damage alone is not equated with total specimen quality — specimen quality is treated as a composite of thermal artifact, margin readability, and tissue architecture preservation, per [[#Primary experimental outcomes]] below.

## Canonical research question

> How do diode laser operating parameters, actual delivered power, and incision speed affect histopathologic quality of ex vivo oral soft-tissue specimens?

## Research rationale

This project does not ask which preset is "best," and it does not ask whether ex vivo findings predict clinical diagnostic success — that would require separate clinical validation, which is out of scope here.

- Console-set power is not assumed to equal delivered power.
- Thermal artifact is not assumed to equal reduced histopathologic quality by itself — quality is assessed across thermal artifact, margin readability, and tissue architecture preservation together.
- No "optimal setting" is claimed unless evidence directly supports it. Preferred terms: evidence-supported range, associated parameters, reported parameter range.
- Ex vivo histologic findings are not claimed to translate directly to clinical diagnostic outcomes. Where clinical implications are discussed, language is limited to "may inform," "may support parameter selection," "may provide mechanistic evidence" — never "predicts diagnostic success" or equivalent.

## Primary experimental chain

`Preset / set power` → `independently measured delivered power` → `controlled incision speed` → `tissue interaction` → `thermal / structural alteration` → `histopathologic specimen quality`

Modifiers of this chain, tracked alongside each link where relevant: wavelength, fiber diameter, tip initiation status, contact vs. non-contact mode, CW vs. PW, pulse parameters (duration, frequency, duty cycle).

The first link (preset → delivered power) is supported by this vault's existing power-output/power-loss evidence — see [[04 Evidence/Set Power vs Measured Output]] and [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]]. The remaining links are this project's own experimental focus.

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
- **CLINICAL RELEVANCE / OUTCOME CONTEXT** — human in vivo diagnostic-biopsy studies, kept as background showing which histologic alterations matter clinically and when thermal artifact does or does not compromise interpretation, but not treated as direct experimental matches to this project's ex vivo design: [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield|Angiero et al. 2011]], [[07 Data/Palaia et al 2021 - 445 nm Diode Laser In Vivo Biopsy Thermal Effect Data|Palaia et al. 2021]], [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]], [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)|Suter et al. 2010]], [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data|Gambino et al. 2026]], [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]], [[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]], and others already processed. **Gundlapalle et al. 2022's pathologist-graded slide-quality score (good/average/poor/non-diagnostic) is this vault's strongest existing clinical analog for what a specimen-quality outcome instrument should measure** — retained here specifically for that methodological reason, not as an experimental match.
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

> Potential novelty: integrating independently measured delivered power and controlled incision speed with biopsy-oriented histopathologic specimen-quality assessment in an ex vivo oral soft-tissue model.

This is deliberately narrower than the prior framing (measured power + speed + diagnostic biopsy outcome), because [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] already demonstrate measured power + controlled speed + histology together — novelty cannot be claimed from those three elements alone. The remaining, narrower distinction rests on: the biopsy-oriented outcome framing itself (margin readability, tissue architecture preservation, peri-incisional alteration graded as a diagnostic-analog specimen); the specific combination of parameters not already jointly covered by one source; and the integration of these elements into a single ex vivo oral soft-tissue study design. **Label: POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION.** Not "no study exists," not "first ever" — see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the full, cautious statement and its stated search limitations.

## Immediate next steps

1. Define a formal margin-readability and/or tissue-architecture-preservation scoring instrument suitable for an ex vivo (non-lesional) oral soft-tissue specimen — the still-missing methodological piece Hanke 2021/Strakas 2023/Al-Ani 2024 each partially approximate but none fully provides.
2. Search specifically for an ex vivo oral-diode study that pairs calibrated power-meter measurement with a biopsy-oriented (not merely cutting-efficiency) histologic outcome — do not assume none exists without a targeted search.
3. Continue tracking incision speed as an explicit, extracted variable, classified by how it was obtained (mechanized / clinician-controlled / measured / descriptive / UNKNOWN) in every newly processed paper; never infer it from procedure duration.
4. Re-evaluate whether Capodiferro et al. 2008's coagulation-zone claim can ever be verified (no full text, no PMCID) or should be treated as permanently abstract-level.
5. If a clinical validation phase is ever proposed, treat it as an explicitly separate follow-on question — not folded into this project's current ex vivo scope.

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
