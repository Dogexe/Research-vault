# Diode Laser Biopsy

Primary research dashboard for this vault. Companion/secondary hub: [[01 Projects/Diode Laser Master]], which holds general diode-laser technical background (power output, calibration, device research) and now supports this project rather than competing with it.

This is a dashboard, not a processing log. Detailed paper-by-paper processing history lives in [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]; cross-study conclusions live in `06 Synthesis/`; structured per-paper extractions live in `07 Data/`.

## Scope

Dental/oral soft-tissue biopsy performed with diode lasers, focusing on how a device's preset power, actual delivered output, and operating parameters propagate through to tissue interaction and, ultimately, to the histopathologic/diagnostic quality of the excised specimen.

## Canonical research question

> How do diode laser operating parameters and actual delivered power affect histopathologic quality of oral soft-tissue biopsy specimens?

## Research rationale

This project is not asking which preset is "best." It asks how nominal device settings and operating technique translate into the actual energy/power delivered to tissue, and how that relates to histopathologic specimen quality.

- Console-set power is not assumed to equal delivered power.
- Thermal artifact is not assumed to equal diagnostic failure.
- No "optimal setting" is claimed unless evidence directly supports it — see the caveats in [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]]. Preferred terms: evidence-supported range, associated parameters, reported parameter range.

## Logic chain

Preset / set power → actual delivered power → incision behaviour → tissue interaction → thermal artifact / margin quality → histopathologic quality

The first link (preset → delivered power) is supported by this vault's existing power-output/power-loss evidence, reframed as supporting technical evidence for this chain — see [[04 Evidence/Set Power vs Measured Output]] and [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]]. The remaining links are this project's own focus.

## Key variables

**Exposure/operating:** wavelength, preset/set power, independently measured power, actual delivered power, average/peak power, CW vs. pulsed mode, pulse duration, frequency, duty cycle, fiber diameter/spot size, initiated vs. non-initiated tip, contact vs. non-contact mode, incision speed, exposure duration, number of passes, movement technique, cooling (if reported).

**Tissue/specimen outcomes:** thermal damage, histological artifact, coagulation zone, carbonization, margin readability, epithelial/connective-tissue artifact, specimen size and margin, diagnostic quality/yield, ability to render a histopathologic diagnosis.

No missing parameter is inferred; absent values are marked `UNKNOWN`.

## Current evidence status

- [[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Thermal Artifact]], [[04 Evidence/Surgical Margins]] — PARTIAL EVIDENCE, each grounded in multiple independent CORE sources (Angiero 2011, Romeo 2014, Azevedo 2016, Gambino 2026, and others per the processing log).
- [[04 Evidence/Power Output and Tissue Effect]] — the central bridge node still NEEDS EVIDENCE. Every processed dental-diode source reports set/console power only; no source pairs an independently measured (power-meter) diode output with a histologic/diagnostic outcome. Wilder-Smith et al. 1995 shows the needed design (measured power + histology) is achievable, but only for CO2, not diode, lasers.
- [[06 Synthesis/Diode Laser Biopsy Specimen Quality]] and [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] — PROVISIONAL, most current syntheses, incorporating all core and supporting sources processed to date (most recently: Shnawa et al. 2025 [CORE], Merigo et al. 2012 and Spille et al. 2026 [SUPPORTING], Romanos et al. 2013 and Lu et al. 2026 [BACKGROUND]).
- Device-level status: [[05 Devices/Device Index]] — no device in this vault currently has both an independently measured output value and a histologic/diagnostic outcome from the same or cross-referenced source.

## Major contradictions

See [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]] for full sourcing. Headline conflicts, kept visible rather than averaged:

- **CW vs. PW thermal-damage direction** — three discordant patterns across independent sources (Gundlapalle et al. 2022 and Romanos et al. 2022: PW < CW damage; Pergolini et al. 2025: PW > CW, not significant; Goharkhay et al. 1999: no consistent direction).
- **Margin-size recommendation** — ≥5 mm (Angiero 2011, Romeo 2014, Gambino 2026, Gundlapalle 2022, all real diagnostic-biopsy pathways) vs. ≥2 mm (Pergolini 2025, ex vivo, no diagnosis rendered).
- **Set power vs. actual delivered power** — established as a real, measured gap by this vault's power-output evidence ([[04 Evidence/Set Power vs Measured Output]]), but never paired with a diode biopsy histology outcome in the same study.
- **Carbonization vs. nominal power** — no clean power-dependence of thermal-damage-zone width found by two independent sources (Pergolini 2025, Goharkhay 1999), which complicates the informal assumption that higher power alone drives more damage.

## Main research gaps

See [[06 Synthesis/Research Gaps in Dental Diode Laser Output]] and the processing log for full sourcing.

- No dental-diode source pairs a calibrated, independently measured power value with a histologic/diagnostic biopsy outcome in the same study. **This is this project's central, still-open gap.**
- No source reports incision speed as an independently varied variable against specimen histologic quality (only two supporting, non-transferable fixed values exist: 10 mm/s and 1 mm/s).
- No source varies power while holding specimen size constant (or vice versa) to isolate their independent effects on diagnostic yield.
- Coagulation-zone evidence for dental diode lasers remains abstract-level only (Capodiferro et al. 2008), unverifiable at full-text.
- No source pairs controlled tip-initiation status with an independently measured power-meter output value.

## Key synthesis links

- [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] — study-level parameter-vs-outcome mapping; proposes one narrow, heavily caveated evidence-supported CW range (1.6–2.7 W, 445/808/980 nm, 300–320 μm fiber), explicitly not an optimal setting.
- [[06 Synthesis/Diode Laser Biopsy Specimen Quality]] — cross-study synthesis of thermal artifact, margins, and diagnostic quality.
- [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]] — the conflicts above, in full.
- [[06 Synthesis/Research Gaps in Dental Diode Laser Output]] — gap analysis for the underlying power-output evidence.
- [[06 Synthesis/Novelty Check - Prior Systematic Review]] — cross-check against Lopes-Santos et al. 2023 (prior systematic review); current label: **POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION** for the integrated chain (set power → independently measured delivered power → controlled/measured incision speed → histologic thermal effect → histopathologic specimen quality). Review silence alone is not treated as proof of novelty.
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] (2026-09-13) — full-text cross-tabulation of the four closest-prior-art candidates (Hanke 2021, Strakas 2023, Isola 2018, Al-Ani 2024) against this vault's strongest existing sources. Label unchanged (**POTENTIAL NOVELTY — REQUIRES SYSTEMATIC VERIFICATION**), but narrowed: Hanke 2021 and Strakas 2023 show a more rigorous per-incision power-verification protocol than previously catalogued in this vault, closing measured-power + speed + histology together — but neither is a biopsy/diagnostic study.

## Immediate next steps

1. Search specifically for a dental-diode study that pairs calibrated power-meter measurement with biopsy histology (the still-open central gap) — do not assume none exists without a targeted search.
2. If found, resolve or narrow the CW-vs-PW three-way contradiction using that source's design.
3. Continue tracking incision speed as an explicit, extracted variable in every newly processed paper; do not infer it from procedure duration or descriptive text.
4. Re-evaluate whether Capodiferro et al. 2008's coagulation-zone claim can ever be verified (no full text, no PMCID) or should be treated as permanently abstract-level.

## Related notes

- [[01 Projects/Diode Laser Master]]
- [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]
- [[00 Inbox/Shortlist - PubMed Candidates 3-7 (Adjacent, Not Core Diode-Output Evidence)]]

## สรุปภาษาไทย

- โครงการนี้เป็นแดชบอร์ดวิจัยหลักของคลังนี้ คำถามหลัก: พารามิเตอร์การทำงานของเลเซอร์ไดโอดและกำลังขาออกที่ส่งจริง ส่งผลต่อคุณภาพทางจุลพยาธิวิทยาของชิ้นเนื้อ biopsy เนื้อเยื่ออ่อนในช่องปากอย่างไร
- ห่วงโซ่ตรรกะ: ค่าตั้งเครื่อง → กำลังขาออกที่ส่งจริง → พฤติกรรมการตัด → ปฏิกิริยาต่อเนื้อเยื่อ → รอยไหม้/คุณภาพขอบตัด → คุณภาพทางจุลพยาธิวิทยา
- ช่องว่างหลักที่ยังไม่ปิด: ยังไม่มีแหล่งข้อมูลใดวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์คู่กับผลทางเนื้อเยื่อ/การวินิจฉัยของเลเซอร์ไดโอดในการศึกษาเดียวกัน
- ไม่มีการอ้าง "ค่าตั้งที่ดีที่สุด" ในบันทึกนี้ — ใช้คำว่าช่วงที่มีหลักฐานสนับสนุนแทน
- ประวัติการประมวลผลบทความโดยละเอียดถูกย้ายไปที่ [[90 Agent/Processing Logs/Diode Laser Biopsy - Processing Log]]
