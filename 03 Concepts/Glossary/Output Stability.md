---
aliases: []
category: laser-operation
unit: "%"
symbol:
equation:
related_terms: [Power Loss, Measured Power, Power Meter, Calibration]
---

# Output Stability

## Definition
Whether a laser's measured output stays consistent across repeated use (successive incisions, or extended irradiation time), as distinct from [[03 Concepts/Glossary/Power Loss]], which this vault treats as a single set-vs-measured discrepancy at one point in time. A device can show stable output that nonetheless differs from its panel setting, or unstable output that drifts across a session regardless of any single-point deviation.

## Unit / equation
Not applicable — typically reported as a deviation threshold (%) over repeated measurements, or as a qualitative degradation/no-degradation finding, rather than a single computed value.

## In this project
This is the operational basis of Hanke et al. 2021's and Strakas et al. 2023's per-incision QC gate (output re-measured before every single cut, ≥5% deviation triggering fiber-tip replacement) — a real-time stability check, not merely a one-time calibration. [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage|Zegaib et al. 2011]] documents declining fiber-tip power with repeated tissue contact (attributed to tip fouling) as a within-session instability. [[07 Data/Davies et al 2020 - EVLA Fiber Tip Power Output and Degradation|Davies et al. 2020]] and [[07 Data/Girasol et al 2022 - Photobiomodulation Device Power and Beam Accuracy|Girasol et al. 2022]] both explicitly test repeated-use/over-time output stability (non-dental sources, cited here for the concept only).

## Common pitfalls
Do not conflate a single set-vs-measured deviation ([[03 Concepts/Glossary/Power Loss]]) with a repeated-use instability — a device could be perfectly stable while still reading below its panel setting, or could start on-target and drift with use. This vault's sources frequently blur the two without labeling which they mean; see [[03 Concepts/Glossary/Power Loss]]'s "Common confusion" section.

## Related terms
[[03 Concepts/Glossary/Power Loss]], [[03 Concepts/Glossary/Measured Power]], [[03 Concepts/Glossary/Power Meter]], [[03 Concepts/Glossary/Calibration]]

## Evidence / source note
[[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] (per-incision ≥5% deviation gate); [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage|Zegaib et al. 2011]] (tip-fouling degradation); [[07 Data/Davies et al 2020 - EVLA Fiber Tip Power Output and Degradation|Davies et al. 2020]] (repeated-use stability, non-dental).

## Usage in literature extraction
Use this term when a source describes output consistency across repeated use or time, not for a single set-vs-measured comparison (use [[03 Concepts/Glossary/Power Loss]] for that).

## สรุปภาษาไทย
Output stability คือความคงที่ของกำลังขาออกที่วัดได้เมื่อใช้งานซ้ำหลายครั้ง ต่างจาก power loss ซึ่งเป็นส่วนต่างระหว่างค่าตั้งกับค่าที่วัดได้ ณ จุดเดียว
