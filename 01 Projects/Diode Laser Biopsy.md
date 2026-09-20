# Diode Laser Biopsy

Primary research dashboard for this vault. Companion/secondary hub: [[01 Projects/Diode Laser Master]], which holds general diode-laser technical background (power output, calibration, device research) and now supports this project rather than competing with it.

This is a dashboard, not a processing log. Detailed paper-by-paper processing history lives in [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]; cross-study conclusions live in `06 Synthesis/`; structured per-paper extractions live in `07 Data/`.

**Reframed 2026-09-16.** This is an **ex vivo experimental study** of oral soft-tissue cutting. Clinical diagnostic-biopsy outcomes remain clinical-relevance context, not the primary experimental endpoint.

## 1. Current RQ

> How do diode-laser operating parameters, independently measured delivered power, and incision speed/movement affect thermal tissue damage and biopsy-oriented histopathologic specimen quality in ex vivo oral soft tissue?

The experimental core is operating parameters, delivered exposure, and movement. `Histopathologic specimen quality` means margin readability, tissue architecture preservation, and specimen interpretability; it is distinct from thermal damage.

## 2. Current rationale

Diode-laser treatment parameters are commonly selected through manufacturer-defined presets or manually entered nominal settings, which can simplify parameter selection in clinical practice. However, independent measurements across dental diode devices show that actual power delivered at the fiber tip may differ from the displayed value, with both the magnitude and direction of deviation varying among devices. Nominal power alone therefore does not fully characterize tissue exposure, which is also influenced by emission characteristics, fiber/tip conditions, and incision speed or movement. These interacting factors may affect two related but distinct outcomes: thermal tissue damage, including coagulation, carbonization, and thermal artifact, and biopsy-oriented histopathologic specimen quality, including margin readability, tissue architecture preservation, and specimen interpretability. Because existing evidence does not establish that lower thermal damage necessarily produces better specimen quality, both dimensions should be evaluated separately under controlled and well-characterized exposure conditions. This is relevant to experimental reproducibility, diagnostic reliability of laser-excised specimens, and laser safety, since safe and effective use requires operators to understand how adjustable parameters influence actual tissue exposure, while current awareness and training evidence does not establish that knowledge gaps cause reliance on manufacturer presets.

## 3. Scientific causal/exposure chain

`Operating parameters` + `independently measured delivered power` + `incision speed / movement` → `tissue interaction` → `thermal tissue damage`

`Operating parameters` + `independently measured delivered power` + `incision speed / movement` → `tissue interaction` → `biopsy-oriented histopathologic specimen quality`

Thermal damage and specimen quality are related but distinct outcomes. Less thermal damage is **not** assumed to mean better specimen quality.

Speed is never inferred from procedure duration. Sources distinguish mechanized control, clinician-controlled targets, measured speed, qualitative movement descriptions, and `UNKNOWN`. Delivered-power evidence likewise distinguishes set power, independent measurement, measurement location/timing, and a reported numerical measured value.

## 4. Supporting rationale branch

`Preset / manufacturer guidance` + `operator knowledge / training` + `laser safety` provide problem framing and practical context; they are not experimental core variables unless directly tested.

- FACT: manufacturer/device materials can distinguish a displayed or preset value from emitted distal-tip output and can describe preset values as general guidance; see [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] and [[05 Devices/Device Index]].
- INTERPRETATION: a preset or manufacturer recommendation is a nominal setting or guidance source, not automatically a complete description of tissue exposure, independently measured delivered power, or a validated biological dose.
- FACT: operator awareness and appropriate parameter adjustment are relevant to laser safety. This project does **not** assume that knowledge gaps cause preset reliance, and it does not require an operator-error premise.

## 5. Primary outcomes

**Thermal tissue-damage outcomes:** thermal-damage width, epithelial and connective-tissue thermal artifact, coagulation zone, and carbonization where reported.

**Biopsy-oriented specimen-quality outcomes:** margin readability, tissue architecture preservation, and specimen interpretability. These are assessed separately from thermal damage.

**Secondary mechanistic outcomes:** incision depth/width and cutting efficiency. This remains a candidate outcome set, not a finalized scoring instrument or protocol.

## 6. Current evidence gap / novelty

FACT: [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]], and [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]] demonstrate independently measured diode output, controlled/reported speed, and histologic tissue effects in ex vivo oral tissue. [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] adds independently measured, numerically reported output plus histology, but no reported speed. These are direct technical precedents, not evidence of a biopsy-oriented specimen-quality framework.

FACT: [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] is the closest ex vivo margin/histologic-damage precedent and reports 0.75 mm/s, but does not report independently measured delivered output. [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]] is the closest clinical analog for a pathologist-graded specimen-quality instrument, but is in vivo and does not independently measure power or report speed.

INTERPRETATION: the current gap is an ex vivo oral-soft-tissue study that combines independently measured delivered power, explicit speed/movement control, and biopsy-oriented specimen-quality outcomes in one design. This is **POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION**; it is not a “first ever” claim. Preset testing may be included only if a named manufacturer/device preset is directly tested, not as a required novelty element.

## 7. Key unresolved assumptions

- `Thermal damage → specimen quality` is not established as a universal relationship. Clinical biopsy studies show that thermal artifact can coexist with preserved diagnosis.
- No source in the vault directly establishes that less thermal damage automatically improves margin readability, architecture preservation, or specimen interpretability.
- No source varies incision speed as an independently varied experimental variable against biopsy-oriented specimen quality.
- No source applies a formal ex-vivo margin-readability or tissue-architecture-preservation instrument together with independently measured delivered power.
- CW/PW effects are not directionally consistent across the current evidence base; see [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]].
- Margin-width recommendations differ between clinical and ex-vivo studies and are not treated as transferable standards.
- Nominal power alone does not show a clean, universal relation to thermal-damage-zone width across current sources.
- Coagulation-zone evidence for dental diode lasers remains abstract-level only in [[07 Data/Capodiferro et al 2008 - Oral Laser Surgical Pathology Abstract-Level Data|Capodiferro et al. 2008]].
- Device-level evidence remains incomplete: [[05 Devices/Device Index]] reports no device with both independently measured output and a biopsy-oriented ex-vivo specimen-quality outcome from the same or cross-referenced source.

## 8. Links to canonical evidence/synthesis notes

- Delivered power: [[04 Evidence/Set Power vs Measured Output]], [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]], [[04 Evidence/Power Output and Tissue Effect]]
- Speed/movement: [[06 Synthesis/Incision Speed and Movement in Diode Laser Tissue Interaction]]
- Thermal damage: [[04 Evidence/Thermal Artifact]]
- Specimen quality: [[04 Evidence/Surgical Margins]], [[04 Evidence/Biopsy Specimen Quality]]
- Technical and clinical context: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]], [[06 Synthesis/Research Gaps in Dental Diode Laser Output]]
- Novelty/prior art (authoritative gap/novelty source): [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[06 Synthesis/Novelty Check - Prior Systematic Review]]
- Supporting rationale only: [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]], [[05 Devices/Device Index]]
- Structured source extractions: [[07 Data]]; provenance and processing history: [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]
- Supporting comprehensive narrative (background/provenance only, not canonical for current RQ/gap decisions): [[06 Synthesis/Literature Review - Diode Laser Biopsy]]

### Direct technical precedent: Hanke and Strakas

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

The closest existing approximation of that biopsy-oriented outcome framework remains [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]]; [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]] remains the closest clinical specimen-quality analog. See [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the full cross-tabulation.

## สรุปภาษาไทย

- โครงการนี้เป็นการศึกษาทดลอง **ex vivo** ของการตัดเนื้อเยื่ออ่อนในช่องปากด้วยเลเซอร์ไดโอด โดยผลการวินิจฉัยทางคลินิกเก็บไว้เป็นข้อมูลบริบท (clinical relevance) ไม่ใช่จุดยุติหลักของการทดลอง
- คำถามวิจัยหลักคือ พารามิเตอร์การทำงาน กำลังขาออกที่วัดได้จริง และความเร็ว/การเคลื่อนไหวของการตัด ส่งผลต่อความเสียหายจากความร้อนและคุณภาพชิ้นเนื้อทางจุลพยาธิวิทยาแบบ biopsy-oriented อย่างไร
- คุณภาพชิ้นเนื้อประกอบด้วยความอ่านง่ายของขอบชิ้นเนื้อ การรักษาโครงสร้างเนื้อเยื่อ และความสามารถในการแปลผลชิ้นเนื้อ ซึ่งแยกจากความเสียหายจากความร้อน ไม่อนุมานว่าความเสียหายจากความร้อนน้อยกว่าจะทำให้คุณภาพชิ้นเนื้อดีกว่าเสมอ
- พรีเซ็ต/คำแนะนำผู้ผลิต ความรู้หรือการฝึกอบรมของผู้ปฏิบัติ และความปลอดภัยของเลเซอร์เป็นเหตุผลสนับสนุน ไม่ใช่แกนการทดลอง เว้นแต่มีการทดสอบโดยตรง
- **Hanke et al. 2021 และ Strakas et al. 2023** เป็นงานก่อนหน้าที่วัดกำลังจริง ควบคุมความเร็ว และประเมินผลทางจุลพยาธิวิทยาในเนื้อเยื่อช่องปาก ex vivo แล้ว แต่ไม่มีกรอบผลลัพธ์คุณภาพชิ้นเนื้อแบบ biopsy-oriented
- ช่องว่างปัจจุบันคือการรวมกำลังขาออกที่วัดได้จริง การควบคุมความเร็ว/การเคลื่อนไหว และผลลัพธ์คุณภาพชิ้นเนื้อแบบ biopsy-oriented ในการศึกษา ex vivo เนื้อเยื่ออ่อนในช่องปากเดียวกัน โดยเป็น **POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION** ไม่ใช่การอ้างว่าเป็นงานแรก
