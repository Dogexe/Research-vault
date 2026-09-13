---
aliases: []
category: histopathology-biopsy
unit:
symbol:
equation:
related_terms: [Biopsy Specimen Quality, Diagnostic Quality, Specimen Margin, Margin Quality]
---

# Biopsy-oriented

## Definition
A study design classification indicating whether the excised/examined tissue represents a real lesion excised as a biopsy specimen — as opposed to a standardized, non-lesional incision or tissue block used for technical/mechanistic characterization. Corresponds directly to the Study Metadata Schema's `biopsy_oriented` boolean field.

## Unit / equation
Not applicable — boolean classification.

## In this project
This distinction is central to this project's novelty framing — [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] are ex vivo, oral, measured-power, controlled-speed studies but are NOT biopsy-oriented (they use standardized linear incisions in non-lesional tissue blocks for cutting-efficiency characterization, not specimen excision). A standardized non-lesional ex vivo excision should not automatically be called biopsy-oriented merely because tissue was cut and examined histologically — "biopsy-oriented" specifically requires the study to evaluate a true biopsy/excision specimen pathway (see [[01 Projects/Diode Laser Biopsy]] "Hanke and Strakas as direct prior art").

## Common pitfalls
Do not infer `biopsy_oriented: true` from `histology: true` or from the presence of a margin measurement — a technical cutting-efficiency study can measure a "total interaction zone" around a linear incision without excising anything resembling a diagnostic specimen.

## Related terms
[[03 Concepts/Glossary/Biopsy Specimen Quality]], [[03 Concepts/Glossary/Diagnostic Quality]], [[03 Concepts/Glossary/Specimen Margin]], [[03 Concepts/Glossary/Margin Quality]]

## Evidence / source note
[[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] and [[01 Projects/Diode Laser Biopsy]] both document this exact distinction using Hanke 2021/Strakas 2023 (not biopsy-oriented) versus [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]] (closest ex vivo biopsy-oriented approximation) as worked examples.

## สรุปภาษาไทย
Biopsy-oriented หมายถึงการศึกษาที่ตัดชิ้นเนื้อรอยโรคจริงในลักษณะ biopsy ไม่ใช่แค่การตัดเนื้อเยื่อปกติเพื่อศึกษาทางเทคนิค
