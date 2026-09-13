---
aliases: [Efficiency Factor]
category: tissue-interaction
unit: dimensionless
symbol: γz
equation: "γz = cutting depth (d_cut) / total interaction zone depth (TIZ_depth)"
related_terms: [Incision Depth, Thermal Damage, Power-to-Speed Relationship]
---

# Cutting Efficiency

## Definition
How much of a laser incision's total depth is useful cutting depth versus non-cutting thermal-interaction-zone depth, expressed by [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]]'s efficiency factor γz = cutting depth ÷ total interaction zone (TIZ) depth. A higher γz means proportionally more of the thermally affected tissue became an actual cut, rather than collateral thermal damage without cutting.

## Unit / equation
Dimensionless ratio, 0–1. γz = d_cut / TIZ_depth. Hanke et al. 2021 proposed γz ≥ 0.6 as a "clinical orientation" threshold; this is the source's own proposed threshold, not an independently validated standard.

## In this project
Originates in [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and is directly reused by [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] (same senior author, same instrument/protocol, extended to 940 nm). Both sources found γz does **not** increase linearly or uniformly with output power — a central, shared finding directly relevant to this project's caution against assuming higher power simply means better cutting behavior. This vault's project note also lists "cutting efficiency" among its secondary/mechanistic candidate outcomes (alongside incision depth/width), distinct from the primary biopsy-oriented specimen-quality outcomes.

## Common pitfalls
Cutting efficiency (a ratio of cut depth to total thermally affected depth) is not the same as [[03 Concepts/Glossary/Incision Depth]] alone, nor the same as [[03 Concepts/Glossary/Thermal Damage]] alone — it relates the two. A high cutting efficiency does not by itself imply low thermal damage in absolute terms, only that thermal damage is proportionally smaller relative to cut depth.

## Related terms
[[03 Concepts/Glossary/Incision Depth]], [[03 Concepts/Glossary/Thermal Damage]], [[03 Concepts/Glossary/Power-to-Speed Relationship]]

## Evidence / source note
[[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] (γz originates here, 8 wavelengths, 0.5–4 W); [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] (γz applied at 940 nm, 1–6 W, highest at 5 W = 0.81 ± 0.03). [[07 Data/Shnawa et al 2025 - Diode Laser vs Scalpel Oral Fibroma Excision Data|Shnawa et al. 2025]] uses "cutting efficiency" descriptively (an initiated tip is stated to optimize it) without computing γz — a qualitative, not quantitative, use of the same term.

## Usage in literature extraction
Use this term for Hanke/Strakas's specific γz ratio, and note explicitly when a source (e.g. Shnawa et al. 2025) uses "cutting efficiency" only descriptively/qualitatively rather than as this computed ratio — do not conflate the two usages.

## สรุปภาษาไทย
Cutting efficiency (γz) คืออัตราส่วนความลึกของรอยตัดจริงต่อความลึกรวมของโซนที่ได้รับผลกระทบจากความร้อน ยิ่งค่าสูงยิ่งหมายถึงพลังงานถูกใช้ไปกับการตัดจริงมากกว่าความเสียหายข้างเคียง
