---
aliases: [Wattmeter]
category: laser-operation
unit:
symbol:
equation:
related_terms: [Measured Power, Calibration, Measurement Location, Output Stability]
---

# Power Meter

## Definition
The physical instrument used to independently verify a laser's optical output, as distinct from the console/panel display — typically a thermopile or photodiode-based sensor (e.g. a "power meter" or "wattmeter") that a study names as its verification method. This note concerns the instrument itself; the resulting value it produces is [[03 Concepts/Glossary/Measured Power]], and whether that instrument's own accuracy was ever independently checked is [[03 Concepts/Glossary/Calibration]].

## Unit / equation
Not applicable — an instrument, not a quantity.

## In this project
Nearly every `07 Data/` note extracts a named or unnamed power-verification instrument as its own row, and this vault's Study Metadata Schema carries it as a dedicated field (`power_meter`). Which specific instrument was used, and how it was used (a one-time setup check vs. a per-incision QC gate), materially changes how much weight a "measured power" claim can bear — a named, described instrument (LabMax Top + PM10, NovaII/Ophir, PM600) is a stronger basis for that claim than an undescribed "wattmeter."

## Common pitfalls
Naming an instrument is not the same as calibrating it — see [[03 Concepts/Glossary/Calibration]]. Do not assume two studies used comparable measurement rigor just because both name "a power meter"; check whether the instrument, its measurement location, and its verification frequency are actually described.

## Related terms
[[03 Concepts/Glossary/Measured Power]], [[03 Concepts/Glossary/Calibration]], [[03 Concepts/Glossary/Measurement Location]], [[03 Concepts/Glossary/Output Stability]]

## Evidence / source note
Named instruments in this vault's core sources: LabMax Top (Coherent) + PM10 detector — [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]]; PM600 (Molectron) — [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]]; NovaII (Ophir Photonics) — [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers|Kim et al. 2020]], [[07 Data/Merigo et al 2012 - Five-Wavelength Ex Vivo Thermal and Histologic Comparison Data|Merigo et al. 2012]]; an unnamed "wattmeter" — [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]].

## Usage in literature extraction
This note is the canonical concept for "power meter"/"wattmeter" as an instrument. Preserve the source's own instrument name/brand in extraction prose; use this wikilink at the first mention of the instrument in a note, not on every repetition.

## สรุปภาษาไทย
Power meter คือเครื่องมือที่ใช้วัดกำลังขาออกจริงของเลเซอร์อย่างเป็นอิสระจากหน้าปัดเครื่อง ค่าที่ได้เรียกว่า measured power ส่วนความน่าเชื่อถือของตัวเครื่องมือเองเป็นคนละประเด็นกับ calibration
