# Average Power

## Definition

The mean optical power delivered over a defined time interval, accounting for any on/off cycling. For a continuous-wave (CW) beam, average power equals the instantaneous power (there is no cycling). For a pulsed beam with a periodic rectangular pulse train, average power equals peak power multiplied by duty cycle. Jenkins PA, Carroll JD ("How to report low-level laser therapy (LLLT)/photomedicine dose and beam parameters in clinical and laboratory studies." *Photomed Laser Surg.* 2011;29(12):785-7. DOI: [10.1089/pho.2011.9895](https://doi.org/10.1089/pho.2011.9895)) list "power" among the essential beam parameters to report and stress that pulsed lasers require distinguishing peak from average power for meaningful comparison.

## นิยามภาษาไทย

กำลังเฉลี่ย (Average Power) คือกำลังแสงเฉลี่ยตลอดช่วงเวลาที่กำหนด โดยคำนึงถึงรอบเปิด/ปิดของพัลส์ สำหรับลำแสงต่อเนื่อง (CW) กำลังเฉลี่ยเท่ากับกำลังขณะนั้น สำหรับลำแสงพัลส์ที่มีรูปแบบพัลส์สี่เหลี่ยมสม่ำเสมอ กำลังเฉลี่ย = กำลังสูงสุด × duty cycle

## Formula

P_avg = P_peak × Duty Cycle (ideal periodic rectangular pulse train); for CW, P_avg = P_set.

## Unit

W.

## In this vault

[[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] reports both a "stipulated" and "measured" mean average power in pulsed mode (e.g., 1.5/1.9 W stipulated/measured at 445 nm) — an explicit average-power field distinct from peak or per-pulse output. [[07 Data/Mazzoni et al 2026 - Neonatal Frenulum Laser Parameters]] reports a "final power" of 1.1 W alongside a separately stated peak power of 100 W, pulse duration 0.05 ms, and frequency 20 Hz, but does not report a duty cycle. NEEDS VERIFICATION: if duty cycle were pulse duration × frequency = 0.05 ms × 20 Hz = 0.1%, the formula above would predict an average power of only ~0.1 W (100 W × 0.001), which does not match the reported 1.1 W — this arithmetic tension is noted here, not resolved, since duty cycle itself is not stated by the source and this vault does not infer missing parameters.

## Common confusion

Average power is not the same as peak power (see [[03 Concepts/Glossary/Peak Power]]) — a "super pulsed" laser can have a very high peak power and a comparatively low average power. Do not assume the reported "power" in a CW-only source generalizes to a pulsed source's average power without checking the pulse parameters.

## Source basis

**Classification:** STANDARD TERM

Average power is a standard laser radiometric quantity defined in ISO 11145 (*Optics and photonics — Lasers and laser-related equipment — Vocabulary and symbols*) for periodically pulsed and CW lasers, and is used equivalently in ANSI Z136.1 (American National Standard for Safe Use of Lasers) exposure/hazard calculations. Clinical/PBM dosimetry reporting guidance (Jenkins & Carroll 2011, cited above) also treats "power" (including average power) as a required, unambiguous beam parameter. NEEDS VERIFICATION: exact ISO clause wording was not directly accessed (standard is paywalled); this classification rests on the standard's confirmed scope/title rather than verbatim text.

## Related

- [[03 Concepts/Glossary/Peak Power]]
- [[03 Concepts/Glossary/Duty Cycle]]
- [[03 Concepts/Glossary/Continuous Wave]]
- [[03 Concepts/Glossary/Pulsed Mode]]
