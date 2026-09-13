---
aliases: [Beam Area]
category: fundamental-physics
unit: μm / mm (diameter); cm² / mm² (derived area)
symbol: d
equation: A = π(d/2)²
related_terms: [Fiber Diameter, Irradiance, Fluence, Contact Mode, Non-contact Mode]
---

# Spot Size

## Definition
The diameter (or characteristic dimension) of the laser beam at the point it strikes the target tissue. The corresponding beam area (used in irradiance/fluence calculations) is derived from spot size as A = π(d/2)² for a circular spot. This vault keeps "spot size" (a length) and "beam area" (its derived area) as one canonical note rather than two, since no vault source reports beam area independently of a stated or assumed spot diameter — see Common pitfalls in [[03 Concepts/Glossary/Fiber Diameter]] for why the two are not automatically identical to fiber diameter either.

## Unit / equation
μm or mm (spot size, diameter); cm² or mm² (beam area). A = π(d/2)².

## In this project
Spot size is not automatically identical to fiber core diameter — divergence, working distance in non-contact mode, and tip shaping can all change the effective spot size at tissue. Spot size is the denominator in irradiance (W/cm²) and fluence (J/cm²) calculations, so an incorrect spot-size assumption propagates directly into both.

## Common pitfalls
Do not assume fiber core diameter equals spot size at tissue, especially in non-contact mode where working distance introduces beam divergence. Do not back-calculate a study's spot size from a reported irradiance value unless the source itself states the spot size used.

## Related terms
[[03 Concepts/Glossary/Fiber Diameter]], [[03 Concepts/Glossary/Irradiance]], [[03 Concepts/Glossary/Fluence]], [[03 Concepts/Glossary/Contact Mode]], [[03 Concepts/Glossary/Non-contact Mode]]

## Evidence / source note
[[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]] and [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]] calculate power density (irradiance) from a stated spot size/fiber diameter — see [[03 Concepts/Glossary/Irradiance]].

## สรุปภาษาไทย
Spot size คือขนาดจุดลำแสงที่ตกกระทบเนื้อเยื่อ ไม่เท่ากับขนาดไฟเบอร์เสมอไป โดยเฉพาะในโหมดไม่สัมผัสที่มีระยะทำงาน
