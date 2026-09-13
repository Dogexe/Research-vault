---
aliases: [Duty Factor]
category: laser-operation
unit: "%"
symbol: D
equation: "D (%) = Pulse Duration × Frequency × 100"
related_terms: [Pulse Duration, Frequency, Average Power]
---

# Duty Cycle

## Definition

The fraction (usually expressed as a percentage) of one pulse period during which the laser is actively emitting ("on"), as opposed to off. Applies only to pulsed operation; a CW laser is, by definition, 100% duty cycle.

## นิยามภาษาไทย

Duty Cycle (สัดส่วนรอบทำงาน) คือสัดส่วน (มักแสดงเป็นเปอร์เซ็นต์) ของหนึ่งรอบพัลส์ที่เลเซอร์กำลังปล่อยแสงอยู่ ("เปิด") เทียบกับช่วงปิด ใช้ได้เฉพาะการทำงานแบบพัลส์ ส่วนเลเซอร์ CW ถือว่ามี duty cycle 100% โดยนิยาม

## Formula

Duty Cycle (%) = (Pulse Duration / Period) × 100 = Pulse Duration × Frequency × 100.

## Unit

% (dimensionless).

## In this vault

Reported explicitly in [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] (50% for all three devices) and [[07 Data/Romanos et al 2022 - Initiated vs Non-Initiated Diode Laser Penetration Depth]] (50%, chopped-pulse mode). [[07 Data/Mazzoni et al 2026 - Neonatal Frenulum Laser Parameters]] reports pulse duration (0.05 ms) and frequency (20 Hz) — from which a duty cycle of 0.1% could be calculated — but does not itself report a duty cycle value, and this vault does not assert one on the source's behalf; see [[Average Power]] for the resulting arithmetic tension with the source's separately reported average/peak power values. [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]] and [[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters]] do not report duty cycle for their diode systems (recorded as UNKNOWN).

## Common confusion

A 50% duty cycle does not mean average power is 50% of the console's power setting unless the console setting itself refers to peak power — some devices display average power as the "set power" already, in which case duty cycle has already been factored in. This vault's sources do not consistently specify which convention their console display uses. NEEDS VERIFICATION.

## Source basis

**Classification:** STANDARD TERM

The concept is standardized in ISO 11145 (*Optics and photonics — Lasers and laser-related equipment — Vocabulary and symbols*), which defines the equivalent quantity as "duty factor" (ratio of pulse duration to pulse period, or pulse duration × pulse repetition frequency). "Duty cycle" is the term more commonly used for the same quantity in clinical/PBM dosimetry literature. NEEDS VERIFICATION: exact ISO clause wording was not directly accessed (standard is paywalled).

## Related

- [[03 Concepts/Glossary/Pulse Duration]]
- [[03 Concepts/Glossary/Frequency]]
- [[Average Power]]
- [[03 Concepts/Glossary/Peak Power]]
