---
aliases: [Measured Delivered Power]
category: laser-operation
unit: W
symbol:
equation:
related_terms: [Set Power, Delivered Power, Power Loss]
---

# Measured Power

## Definition

A power value obtained by an independent measurement instrument (typically a calibrated optical power meter, or an indirect proxy such as calorimetry), as opposed to a value read from the device's own control panel. Measured power is only meaningful when its measurement location is specified (e.g., at the fiber tip, post-fibre, at a bench sensor), since power can differ between locations.

## นิยามภาษาไทย

กำลังที่วัดได้ (Measured Power) คือค่ากำลังที่ได้จากเครื่องมือวัดอิสระ (มักเป็นเพาเวอร์มิเตอร์ที่ผ่านการสอบเทียบ หรือวิธีวัดทางอ้อม เช่น แคลอรีมิเตอร์) ไม่ใช่ค่าที่อ่านจากหน้าปัดเครื่อง ค่าที่วัดได้จะมีความหมายก็ต่อเมื่อระบุตำแหน่งวัดด้วย (เช่น ที่ปลายไฟเบอร์) เนื่องจากกำลังอาจต่างกันตามตำแหน่ง

## Unit

W (or mW).

## In this vault

Measured power is the "Actual Power" column in [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]], the "post-fibre emission" value in [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]], the fiber-tip absolute power in [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]], and the device-specific measured value (2%–134% of declared) in [[07 Data/Girasol et al 2022 - Photobiomodulation Device Power and Beam Accuracy]]. Two vault sources performed a fiber-tip power-meter measurement but never published the resulting number — recorded in this vault as UNKNOWN for measured power despite the measurement having physically taken place: [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]], [[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters]].

## Common confusion

Measured power is not always lower than set power — Kim et al. 2020's K2 mobile device measured above its panel setting (see [[03 Concepts/Glossary/Power Loss]]). Also distinguish the measurement *method*: [[07 Data/Davies et al 2020 - EVLA Fiber Tip Power Output and Degradation]]'s "measured" value is inferred indirectly from water-bath temperature rise (calorimetry), not a direct optical power-meter reading — methodologically different from this vault's core dental sources, which all use a named power meter.

## Source basis

**Classification:** FIELD-USAGE TERM

ISO 11145 and ANSI Z136.1 define the underlying physical quantity "power," but neither standard names "measured power" as a term distinct from a device's displayed value. The set-vs-measured distinction used in this note is an operational/methodological convention from the device-testing and clinical laser literature (see In this vault above, e.g. Kim et al. 2020, Parker et al. 2022), not a term defined by a formal vocabulary standard.

## Schema field mapping (Study Metadata Schema v1.2)

This vault's `07 Data/` extraction schema splits "measured power" into three separate fields that must not be collapsed into one glossary meaning (see [[99 Templates/Study Metadata Schema]]):

- `measured_power` (boolean/`null`) — was output independently measured at all, regardless of whether a number was tabulated?
- `measured_power_value_reported` (boolean/`null`) — did the source additionally report the actual numerical measured value, distinct from set power?
- `measured_power_w` (number/list/`null`) — that explicit measured value in watts; populated only when `measured_power_value_reported` is `true`.

A study can have `measured_power: true` with `measured_power_value_reported: false` and `measured_power_w: null` — e.g. Hanke et al. 2021 and Strakas et al. 2023, which verify output with a calibrated meter before every incision but only report a QC pass/fail deviation threshold, not a tabulated wattage. This is not a gap in extraction; it reflects what the source itself reported.

## Related

- [[03 Concepts/Glossary/Set Power]]
- [[03 Concepts/Glossary/Delivered Power]]
- [[03 Concepts/Glossary/Power Loss]]
- [[03 Concepts/Power Output]] (vault concept note, evidence-grounded)
