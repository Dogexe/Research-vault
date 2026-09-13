---
aliases: [Temperature Elevation, Thermal Rise]
category: tissue-interaction
unit: "°C"
symbol: ΔT
equation:
related_terms: [Thermal Damage, Thermal Relaxation Time, Photothermal Interaction]
---

# Temperature Rise

## Definition
A real-time thermometric measurement (thermocouple, infrared camera, or thermographic monitoring) of actual temperature change during or immediately after laser irradiation, reported in °C — as distinct from [[03 Concepts/Glossary/Thermal Damage]], which is a retrospective histologic finding (a zone of altered tissue structure) rather than a direct temperature reading. A study can measure one without the other, and this vault does not treat them as interchangeable.

## Unit / equation
°C (temperature) or ΔT (rise). Not computed from power alone by this vault — see Common pitfalls.

## In this project
[[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]]'s primary outcome is thermocouple-measured peri-incisional temperature rise, not power-output accuracy or histologic thermal damage: mean rise 8.06 ± 2.58 °C for the diode arm vs. 3.87 ± 1.16 °C for its Er,Cr:YSGG comparator (P < 0.001), with the 2.5 W diode group highest at 10.06 ± 2.02 °C. [[07 Data/Merigo et al 2012 - Five-Wavelength Ex Vivo Thermal and Histologic Comparison Data|Merigo et al. 2012]] independently measures both superficial (infrared camera) and deep (thermocouple) temperature rise for its diode arm (e.g. 5 W CW: superficial Δ 25 ± 0.6 °C, deep Δ 15.975 ± 11.1 °C), alongside a separately scored histologic incision-quality outcome. [[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]] uses continuous infrared thermographic monitoring with an 80 °C threshold as a real-time thermal-safety control, not as a reported outcome value.

## Common pitfalls
Do not infer temperature rise from set or measured power alone — no vault source supports that calculation, and [[03 Concepts/Glossary/Thermal Relaxation Time]]/tissue-specific thermal properties mean the relationship is not simple or linear. Do not treat a measured temperature rise as equivalent to a histologic thermal-damage-zone width — they are different measurement types (direct physical reading vs. retrospective tissue-structure finding) that can, but need not, correlate.

## Related terms
[[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Thermal Relaxation Time]], [[03 Concepts/Glossary/Photothermal Interaction]]

## Evidence / source note
[[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]] (thermocouple, primary outcome); [[07 Data/Merigo et al 2012 - Five-Wavelength Ex Vivo Thermal and Histologic Comparison Data|Merigo et al. 2012]] (infrared camera + thermocouple, both superficial and deep); [[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]] (real-time thermographic safety monitoring, not a reported outcome).

## Usage in literature extraction
Use this term specifically for a real-time or thermometrically measured temperature value in °C. Do not use it as a substitute for [[03 Concepts/Glossary/Thermal Damage]] when a source reports only a histologic finding with no actual temperature measurement.

## สรุปภาษาไทย
Temperature rise คือค่าอุณหภูมิที่วัดได้จริงแบบเรียลไทม์ (เช่น thermocouple หรือกล้องอินฟราเรด) ระหว่าง/หลังการฉายเลเซอร์ทันที ต่างจาก thermal damage ซึ่งเป็นลักษณะทางจุลพยาธิวิทยาที่พบย้อนหลัง ไม่ใช่การวัดอุณหภูมิโดยตรง
