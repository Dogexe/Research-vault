---
aliases: []
category: laser-operation
unit:
symbol:
equation:
related_terms: [Power Meter, Measured Power, Output Stability]
---

# Calibration

## Definition
Evidence that a measurement instrument's own accuracy has been established against a traceable reference — a certificate, protocol, or stated tolerance — as distinct from simply naming the instrument used, or from routinely checking a laser's output against that (possibly uncalibrated) instrument before use. A study can perform a rigorous per-incision power *verification* (comparing the laser to its power meter every time) while never describing any calibration of the meter itself.

## Unit / equation
Not applicable.

## In this project
This vault's `07 Data/` extraction table carries a "Calibration method" row for every source, and it is `UNKNOWN` in nearly all of them — including sources with otherwise rigorous per-incision measurement protocols (Hanke 2021, Strakas 2023, Prado 2022, Gutiérrez-Corrales 2020, Al-Ani 2023/2024). This is a distinct question from whether measurement happened at all ([[03 Concepts/Glossary/Measured Power]]): a study can independently verify output before every incision and still never state that its own power meter was itself calibrated, or against what standard.

## Common pitfalls
Do not read "measured with a calibrated power meter" as evidence of a described calibration protocol — most vault sources use "calibrated" only as an adjective, without stating a protocol, certificate, or traceability standard, which this vault records as `UNKNOWN` rather than inferring compliance. Do not confuse a one-time instrument calibration with the repeated-use output-verification gate some sources apply per incision (see [[03 Concepts/Glossary/Output Stability]]) — these are separate questions this vault's sources frequently blur without labeling which they mean (see [[03 Concepts/Glossary/Power Loss]]'s "Common confusion").

## Related terms
[[03 Concepts/Glossary/Power Meter]], [[03 Concepts/Glossary/Measured Power]], [[03 Concepts/Glossary/Output Stability]]

## Evidence / source note
The rare sources with any calibration detail beyond the bare adjective: [[07 Data/Girasol et al 2022 - Photobiomodulation Device Power and Beam Accuracy|Girasol et al. 2022]] (manufacturer-calibrated, <12-month acquisition-to-use interval, stated 1–1.5% error rate — a photobiomodulation, non-diode source) and [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters|Parker et al. 2022]] ("routine maintenance" stated, protocol otherwise unspecified). All other reviewed sources, including every current priority diode study (Hanke 2021, Strakas 2023, Prado 2022, Merigo 2012, Kim 2020, Gutiérrez-Corrales 2020, Goharkhay 1999, Al-Ani 2023/2024), leave calibration protocol `UNKNOWN` even where measurement itself is well described. See [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]].

## Usage in literature extraction
This note is the canonical concept for the vault's recurring "Calibration method" extraction row. Preserve the source's own wording (e.g. "calibrated power meter," "routine maintenance") rather than inferring a protocol that isn't stated.

## สรุปภาษาไทย
Calibration คือหลักฐานว่าตัวเครื่องมือวัดเองได้รับการสอบเทียบกับมาตรฐานที่ตรวจสอบย้อนกลับได้ ต่างจากการที่งานวิจัยเพียงตรวจสอบกำลังขาออกของเลเซอร์เทียบกับเครื่องมือ (ซึ่งอาจไม่เคยสอบเทียบเองเลย) เป็นประจำก่อนใช้งาน
