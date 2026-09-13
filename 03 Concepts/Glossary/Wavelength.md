---
aliases: []
category: fundamental-physics
unit: nm
symbol: λ
equation:
related_terms: [Photon Energy, Optical Frequency, Absorption, Chromophore]
---

# Wavelength

## Definition
Wavelength (λ) is the spatial period of the laser's optical output, in nanometers (nm) for the diode wavelengths used in this literature (typically 445–980+ nm). Wavelength determines which tissue chromophores preferentially absorb the light (see [[03 Concepts/Glossary/Chromophore]], [[03 Concepts/Glossary/Absorption]]).

## Unit / equation
nm. Related to photon energy via E_photon = hc/λ (see [[03 Concepts/Glossary/Photon Energy]]).

## In this project
Wavelength is tracked as the `wavelength_nm` schema field and is a primary determinant of tissue interaction, but wavelength alone does not determine tissue effect — delivered power, exposure time, fiber/tip geometry, and tissue optical properties all modify the outcome for a given wavelength (see [[03 Concepts/Glossary/Photothermal Interaction]]). This vault's evidence spans several diode wavelengths (445, 810, 940, 980 nm and others) without assuming any one wavelength's effect generalizes to another absent a direct source comparison.

## Common pitfalls
A wavelength value alone should never be used to predict tissue effect — two sources at the same wavelength but different power, speed, or tip condition are not directly comparable results.

## Related terms
[[03 Concepts/Glossary/Photon Energy]], [[03 Concepts/Glossary/Optical Frequency]], [[03 Concepts/Glossary/Absorption]], [[03 Concepts/Glossary/Chromophore]]

## Evidence / source note
Foundational optics. Wavelength values per study are drawn from `07 Data/` extractions (e.g. [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data]]) — see [[99 Templates/Study Metadata Schema]] `wavelength_nm` field.

## สรุปภาษาไทย
ความยาวคลื่น (Wavelength) กำหนดว่าโครโมฟอร์ชนิดใดในเนื้อเยื่อจะดูดกลืนแสงได้ดี แต่ไม่ได้กำหนดผลต่อเนื้อเยื่อเพียงลำพัง ต้องพิจารณาร่วมกับกำลัง ความเร็ว และรูปแบบการนำแสง
