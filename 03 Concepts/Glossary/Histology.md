---
aliases: []
category: histopathology-biopsy
unit:
symbol:
equation:
related_terms: [Thermal Damage, Histological Artifact, Margin Quality, Tissue Architecture Preservation, Diagnostic Quality]
---

# Histology

## Definition
Microscopic examination of tissue structure, typically after fixation, sectioning, and staining, used in this project's literature to assess thermal alteration, tissue architecture, and diagnostic adequacy of laser-excised specimens.

## Unit / equation
Not applicable — the schema `histology` field is boolean (whether histologic evaluation of any rigor was performed).

## In this project
`histology` (per [[99 Templates/Study Metadata Schema]]) records only whether histologic evaluation occurred, at any rigor level from descriptive to quantified — it says nothing by itself about specimen quality, thermal artifact severity, or diagnostic outcome, which are tracked as separate fields/concepts (see [[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Margin Quality]], [[03 Concepts/Glossary/Diagnostic Quality]]).

## Common pitfalls
A study with `histology: true` has not necessarily assessed margin quality, tissue architecture, or diagnostic outcome — those require checking the corresponding separate fields/notes, not assuming they follow automatically from histologic evaluation having occurred.

## Related terms
[[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Histological Artifact]], [[03 Concepts/Glossary/Margin Quality]], [[03 Concepts/Glossary/Tissue Architecture Preservation]], [[03 Concepts/Glossary/Diagnostic Quality]]

## Evidence / source note
See [[06 Synthesis/Study Dashboard]] Table C for the vault's cross-tabulation of `histology` against measured power and incision speed.

## สรุปภาษาไทย
Histology คือการตรวจเนื้อเยื่อด้วยกล้องจุลทรรศน์ ฟิลด์ `histology` บอกเพียงว่ามีการตรวจหรือไม่ ไม่ได้บอกคุณภาพชิ้นเนื้อโดยอัตโนมัติ
