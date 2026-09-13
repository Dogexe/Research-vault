---
aliases: []
category: laser-operation
unit: s / min
symbol:
equation:
related_terms: [Incision Speed, Excision Time, Exposure Time]
---

# Procedure Time

## Definition
The total elapsed duration of a clinical or bench procedure, including any non-cutting time (positioning, hemostasis, multiple passes, pauses) — a broader quantity than the time spent actively incising tissue.

## Unit / equation
s or min. Not convertible to a speed without also knowing incision length AND that the full duration was spent cutting at constant speed — an assumption this vault does not make.

## In this project
Procedure time must never be used to back-calculate incision speed (speed ≠ incision length ÷ procedure time) because procedure time includes time the laser was not actively cutting. This vault records incision speed only when a source explicitly reports it as a value (see [[03 Concepts/Glossary/Incision Speed]] and [[99 Templates/Study Metadata Schema]] `incision_speed_reported`/`speed_mm_s` fields).

## Common pitfalls
A short procedure time does not imply a fast incision speed, and a long procedure time does not imply a slow one — both can reflect non-cutting overhead unrelated to the cutting rate itself.

## Related terms
[[03 Concepts/Glossary/Incision Speed]], [[03 Concepts/Glossary/Excision Time]], [[03 Concepts/Glossary/Exposure Time]]

## Evidence / source note
No vault source is currently tagged with a distinct `procedure_time` schema field (not part of the current schema); this note exists to guard the incision-speed-derivation boundary stated in AGENTS.md and [[99 Templates/Study Metadata Schema]].

## สรุปภาษาไทย
Procedure time คือเวลารวมของหัตถการ รวมช่วงที่ไม่ได้ตัดเนื้อเยื่อด้วย ห้ามใช้คำนวณย้อนกลับเป็นความเร็วตัด
