---
aliases: [Margin Readability, Margin Interpretability]
category: histopathology-biopsy
unit:
symbol:
equation:
related_terms: [Thermal Damage, Specimen Margin, Tissue Architecture Preservation, Diagnostic Quality, Biopsy Specimen Quality]
---

# Margin Quality

## Definition
A qualitative or quantified assessment of how well the cut edge (margin) of an excised specimen retains features a pathologist needs to read — freedom from obscuring thermal artifact, clear demarcation of margin tissue, and preserved cellular/structural detail at the edge. This vault treats "margin quality" and "margin readability" as one canonical concept (aliased together), since the vault's own synthesis notes (e.g. the Novelty Matrix's "Margin readability / specimen-quality assessment" column) use them interchangeably rather than as technically distinct measures.

## Unit / equation
Not applicable — the schema `margin_quality` field is free text (see below), not a controlled score.

## In this project
Margin quality/readability is explicitly NOT automatically equivalent to thermal damage zone width (see [[03 Concepts/Glossary/Thermal Damage]]) — a wide thermal damage zone could still leave a readable margin, and vice versa, depending on what specifically is altered. Per the Study Metadata Schema, `margin_quality` stays free text because the currently tagged notes show too much variety (quantified μm distance, qualitative statement, or not applicable) to force into fixed categories prematurely. [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data|Gundlapalle et al. 2022]]'s pathologist-graded slide-quality scale (good/average/poor/non-diagnostic) is this vault's strongest existing analog for what a formal margin-quality instrument could look like, though it is in vivo, not ex vivo.

## Common pitfalls
Do not equate margin quality/readability with thermal damage zone width — they are related but not the same measurement; a specimen can have measurable thermal damage without necessarily losing margin readability. Do not assume a "margin quality" score exists for a study just because it reports a thermal-damage or margin-alteration distance.

## Related terms
[[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Specimen Margin]], [[03 Concepts/Glossary/Tissue Architecture Preservation]], [[03 Concepts/Glossary/Diagnostic Quality]], [[03 Concepts/Glossary/Biopsy Specimen Quality]]

## Evidence / source note
[[99 Templates/Study Metadata Schema]] `margin_quality` field definition; [[07 Data/Gundlapalle et al 2022 - Diode Laser CW vs PW Biopsy Margin Data]] for the closest existing scoring-instrument analog; [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the vault's cross-study comparison.

## สรุปภาษาไทย
Margin quality/readability คือคุณภาพในการอ่านขอบชิ้นเนื้อ ไม่เท่ากับความกว้างของโซนความเสียหายจากความร้อนเสมอไป
