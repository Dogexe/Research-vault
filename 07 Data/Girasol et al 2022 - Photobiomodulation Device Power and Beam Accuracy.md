# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: SUPPORTING/BACKGROUND evidence for output accuracy, repeatability, and measurement methodology — not confirmed dental, and not core dental set-power vs. measured-output evidence.** This source surveys low-power photobiomodulation (LLLT/PBM) devices drawn from physical therapy clinics, hospitals, universities, and research laboratories in Brazil; the equipment brands and clinical context described are physiotherapy/rehabilitation, not dentistry. It is retained because its multi-device power-accuracy survey design and its within-session output-stability sub-analysis are directly analogous to the vault's dental power-loss and calibration questions.

## Source

- Literature note: [[02 Literature/10.1371/journal.pone.0266193|Girasol et al. 2022]]
- Source link: https://doi.org/10.1371/journal.pone.0266193
- Source locator: Abstract; Materials and methods; Table 1; Table 2; Table 3; Results; Discussion; Conclusion

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | 24 low-power laser photobiomodulation devices in clinical use in Brazil, multiple brands/models: Ibramed Laserpulse (n=18), Ibramed Antares (n=2), HTM Fluence (n=2), DMC Therapy XT (n=2), by wavelength per Table 1; not identified as dental devices — drawn from physical therapy clinics, hospitals, universities, and research laboratories | UNKNOWN | Materials and methods; Table 1 | FACT |
| Manufacturer | Ibramed (Amparo, São Paulo, Brazil); HTM (São Carlos, São Paulo, Brazil); DMC (Amparo, São Paulo, Brazil) | UNKNOWN | Table 1 | FACT |
| Wavelength | 450, 660, 808, 830, 904 | nm | Table 1 | FACT |
| Set power (manufacturer-declared/nominal) | Device-specific; not a single value — each of the 24 units has its own manufacturer-stated power in its manual; measured values expressed by the source as a percentage of this declared value | mW (device-specific, see Table 1) | Materials and methods; Table 1 | FACT |
| Measured output power | Device-specific average power measured (mW), ranging from 0.61 mW to 103 mW across the 24 units; corresponding to 2%–134% of the manufacturer-declared value per device | mW | Table 1; Results | FACT |
| Average power | Same measurement as "measured output power" above (source's own metric, one-minute or three-minute sequential irradiation mean) | mW | Materials and methods; Table 3 | FACT |
| Peak power | "Maximum power" measured only for the 830 nm and 904 nm subset during the 1-min vs. 3-min sequential-emission sub-analysis (not for all 24 devices) | mW | Table 3 | FACT (subset only) |
| Operating mode | UNKNOWN — not explicitly stated as CW or pulsed for the surveyed devices | UNKNOWN | UNKNOWN | UNKNOWN |
| Pulse duration | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Frequency | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Duty cycle | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Fiber diameter | UNKNOWN — devices are hand-held probe/emitter units; beam diameter (not fiber diameter) was measured instead (see Tip type row) | UNKNOWN | UNKNOWN | UNKNOWN |
| Tip type | Not fiber-delivered; direct probe/emitter beam. Beam diameter differences of 38%–543% of nominal (manufacturer-stated) values were observed, including differences between units of the same brand and model; beam geometry found to be more elliptical than circular for the evaluated equipment | UNKNOWN (detail); % deviation reported | Results; Fig 3; Fig 4; Table 2 | FACT |
| Tip initiation status | UNKNOWN — not applicable; no initiated/non-initiated tip concept used for these PBM probe devices | UNKNOWN | UNKNOWN | UNKNOWN |
| Contact mode | UNKNOWN — devices were positioned to irradiate a power sensor directly at perpendicular incidence in a bench setup, not applied to tissue | UNKNOWN | UNKNOWN | UNKNOWN |
| Exposure duration | Red-spectrum devices: 1 minute sequential irradiation. Infrared devices (830 nm, 904 nm): 1 minute and 3 minutes sequential irradiation, to test power-output stability over time | min | Materials and methods | FACT |
| Measurement method | Average power: PowerMax-USB Power Sensor (Coherent, Santa Clara, CA) with associated software, sensor positioned for perpendicular incidence; power sensor calibrated by manufacturer within 12 months of use, stated error rate 1%–1.5%. Beam diameter: LM-2 VIS or LM-2 NIR detector (Coherent) coupled to a FieldMaxII TOP power meter (Coherent) via a 0.25 mm-diameter optical fiber segment on an XYZ translation stage (0.005 mm resolution); Gaussian-fit beam-profile analysis at Z = 0, 3, 6, 9, 12, 15 mm | UNKNOWN (further detail) | Materials and methods | FACT |
| Power loss / deviation | Overall measured power ranged from 2% to 134% of the manufacturer-declared value; only 9 of 24 devices fell within 90%–110% of declared power; among the remainder, 9 devices were at least 20% below predicted (up to 98% below), and 1 device was 34% above predicted | % | Results; Discussion | FACT |
| Calibration method | Power sensor (PowerMax-USB) calibrated by the manufacturer, acquisition-to-use interval <12 months, stated manufacturer error rate of 1%–1.5%; no calibration protocol described for the beam-diameter detection system (LM-2/FieldMaxII) beyond identifying the instruments used | UNKNOWN (protocol detail beyond above) | Materials and methods | FACT (power sensor) / UNKNOWN (beam system protocol) |

## Notes

- FACT: In the 1-min vs. 3-min sequential-emission sub-analysis (830 nm and 904 nm devices only), both mean and maximum power increased slightly but statistically significantly from 1 minute to 3 minutes: 830 nm mean 28.77→30.20 mW (P = .031), 830 nm maximum 29.60→31.13 mW (P = .047); 904 nm mean 40.02→41.09 mW (P = .006), 904 nm maximum 41.08→41.92 mW (P = .019). No significant difference was found between the two wavelengths in the size of this time-related change (mean comparison P = .865; maximum comparison P = .673).
- FACT: No significant correlation was found between device age (time since purchase) and measured power (Spearman's rs = -0.051, P = .813) or beam diameter (rs = -0.249, P = .277); likewise no significant correlation between time since last maintenance and measured power (rs = -0.107, P = .619) or beam diameter (rs = -0.282, P = .216).
- FACT: The source explicitly frames these findings as relevant to reproducibility of published PBM clinical results, noting that many clinical studies report only the manufacturer-declared power rather than an independently measured value.
- FACT: Beam-diameter differences were observed even between units of identical brand and model, which the source attributes to a combination of possible manufacturing-batch variation (certification tests only sample batches) and lack of routine preventive maintenance; the source states it cannot distinguish between these two causes from its data (no before/after comparison was available).
- FACT: All 24 devices were reported by the source as being in active clinical use (average weekly use <30 minutes; average device age 11±5 years) at the time of measurement, not new/factory-condition units.
- INTERPRETATION (the source's own framing, reproduced here, not independently re-derived): the wide spread of measured-to-declared power ratios reflects a combination of insufficient preventive maintenance in the field and possible original manufacturing variation, rather than a single dominant cause.
- HYPOTHESIS: UNKNOWN — the source proposes no formal testable hypothesis; it recommends shared manufacturer/operator standardization and maintenance protocols (Conclusion).
- Classification for this vault: supporting/background evidence for output-accuracy survey methodology (a multi-device, real-world-use design analogous to Parker et al. 2022's dental survey) and for within-session output-repeatability testing. Not confirmed dental, not a core dental set-power-vs-measured-output source, and its device class (PBM/LLLT low-power emitters) differs from the vault's core dental soft-tissue surgical diode lasers.

## สรุปภาษาไทย

- งานวิจัยนี้เป็นหลักฐานสนับสนุน (supporting/background) ไม่ใช่หลักฐานหลักของทันตกรรม เนื่องจากเป็นการสำรวจเครื่องเลเซอร์กำลังต่ำสำหรับ photobiomodulation (PBM/LLLT) ที่ใช้ในคลินิกกายภาพบำบัดในบราซิล ไม่ใช่เลเซอร์ไดโอดทางทันตกรรม
- จากอุปกรณ์ 24 เครื่อง พบว่ากำลังขาออกที่วัดได้จริงอยู่ในช่วง 2%–134% ของค่าที่ผู้ผลิตระบุไว้ มีเพียง 9 เครื่องเท่านั้นที่อยู่ในช่วง 90–110% ของค่าที่ระบุ
- เส้นผ่านศูนย์กลางลำแสง (beam diameter) ก็คลาดเคลื่อนจากค่าที่ระบุไว้ถึง 38%–543% แม้เป็นยี่ห้อและรุ่นเดียวกัน
- เมื่อทดสอบความเสถียรของกำลังขาออกระหว่างการฉายต่อเนื่อง 1 นาที เทียบกับ 3 นาที (เฉพาะความยาวคลื่น 830 และ 904 nm) พบว่ากำลังเพิ่มขึ้นเล็กน้อยแต่มีนัยสำคัญทางสถิติ
- ไม่พบความสัมพันธ์ที่มีนัยสำคัญระหว่างอายุเครื่องหรือระยะเวลาตั้งแต่การบำรุงรักษาครั้งล่าสุด กับค่ากำลังหรือเส้นผ่านศูนย์กลางลำแสงที่วัดได้
- ผลการศึกษานี้ไม่สามารถนำมาใช้แทนหลักฐานกำลังขาออกของเลเซอร์ไดโอดทางทันตกรรมได้โดยตรง เนื่องจากกลุ่มอุปกรณ์และบริบทการใช้งานต่างกัน
