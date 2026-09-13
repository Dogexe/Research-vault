---
aliases: []
category: laser-operation
unit:
symbol:
equation:
related_terms: [Measured Power, Power Meter, Delivered Power]
---

# Measurement Location

## Definition
Where along the delivery path a power measurement was actually taken — e.g. the distal end of the fiber, the fiber outflow, or an unspecified point "at the fiber tip." A measured-power value is only interpretable relative to its measurement location, since further loss can occur between that point and the tissue itself (see [[03 Concepts/Glossary/Delivered Power]]).

## Unit / equation
Not applicable — a location descriptor, not a quantity. This vault's Study Metadata Schema carries it as the free-text `measurement_location` field.

## In this project
Sources that state a measurement location use varying language for what may or may not be the same physical point: "distal end of the fiber" ([[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]]), "fiber outflow" ([[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]]), and "fiber tip" ([[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters|Gutiérrez-Corrales et al. 2020]]). Other sources describe a measurement without ever stating where it was taken ([[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]]). This vault does not assume these phrasings are interchangeable; each is preserved as the source's own wording.

## Common pitfalls
Do not assume an unstated measurement location means "at the tissue" — most vault sources measure at or near the fiber tip in air, not at the actual target surface, and non-contact working distance can introduce further loss beyond that point. Do not treat "fiber tip," "distal end of fiber," and "fiber outflow" as certainly identical across studies unless the source itself equates them.

## Related terms
[[03 Concepts/Glossary/Measured Power]], [[03 Concepts/Glossary/Power Meter]], [[03 Concepts/Glossary/Delivered Power]]

## Evidence / source note
See [[99 Templates/Study Metadata Schema]] `measurement_location` field definition, and [[03 Concepts/Glossary/Measured Power]]'s existing note that "measured power is only meaningful when its measurement location is specified."

## Usage in literature extraction
Preserve the source's exact phrasing for where measurement occurred; do not normalize "distal end of fiber," "fiber outflow," and "fiber tip" to one canonical phrase in extraction prose, even though they are grouped under this one concept for navigation purposes.

## สรุปภาษาไทย
Measurement location คือตำแหน่งที่วัดกำลังจริง (เช่น ปลายไฟเบอร์) ค่าที่วัดได้มีความหมายก็ต่อเมื่อรู้ตำแหน่งวัด เพราะอาจมีการสูญเสียเพิ่มเติมระหว่างจุดวัดกับเนื้อเยื่อเป้าหมายจริง
