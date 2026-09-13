---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: [445, 970]
set_power_w: 2
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW+PW"
fiber_diameter_um: 320
tip_initiation: "both"
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: SUPPORTING evidence for initiated vs. non-initiated tip and operating parameters — not direct power-loss/measured-output-deviation evidence.** This source measures histological penetration depth (a tissue-effect proxy), not fiber-tip power output against a power meter. It uses the same device model (SIROLaser Blue, Dentsply Sirona) as [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output|Xue et al. 2022]], but does not itself report a measured-output power value, so this device overlap cannot be used to compare power-deviation results between the two studies.

## Source

- Literature note: [[02 Literature/10.3390/app122412771|Romanos et al. 2022]]
- Source link: https://doi.org/10.3390/app122412771
- Source locator: Abstract; Materials and Methods §2.1; Results §3; Table 1; Discussion

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | SIROLaser Blue® (Dentsply Sirona, Charlotte, NC, USA), Class IV diode laser | UNKNOWN | Materials and Methods §2.1 | FACT |
| Manufacturer | Dentsply Sirona | UNKNOWN | Materials and Methods §2.1 | FACT |
| Wavelength | 445 (±5 nm); 970 (−10/+15 nm) | nm | Materials and Methods §2.1 | FACT |
| Set power | 2 | W | Materials and Methods §2.1 | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification of output is reported; power setting is stated as the manufacturer/literature-recommended panel value only | UNKNOWN | UNKNOWN | UNKNOWN |
| Average power | Pulsed (chopped) mode mean power: 1 | W | Materials and Methods §2.1 | FACT |
| Peak power | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Operating mode | Continuous wave (C.W.) and pulsed ("chopped-pulse"), both tested at both wavelengths | UNKNOWN | Materials and Methods §2.1 | FACT |
| Pulse duration | 10 μs–0.99 s (chopped-pulse mode) | μs–s | Materials and Methods §2.1 | FACT |
| Frequency | 35 | Hz | Materials and Methods §2.1 | FACT |
| Duty cycle | 50 | % | Materials and Methods §2.1 | FACT |
| Fiber diameter | 320 | μm | Materials and Methods §2.1 | FACT |
| Tip type | Disposable fiberoptic tip, "EasyTip 320" | UNKNOWN | Materials and Methods §2.1 | FACT |
| Tip initiation status | Both initiated and non-initiated tips tested (within-study comparison). Initiated tips were prepared using dark blue articulating paper (Accufilm; Parkell) applied for 5 sec | UNKNOWN | Materials and Methods §2.1 | FACT |
| Contact mode | Contact mode; fiber inserted parallel to the tooth axis to a depth of 3–4 mm and moved along the buccal and lingual gingival/sulcus surfaces | UNKNOWN | Materials and Methods §2.1 | FACT |
| Exposure duration | 30 sec buccal + 30 sec lingual per tooth (60 sec total per tooth) | sec | Materials and Methods §2.1 | FACT |
| Measurement method | Not a power measurement. Outcome measured: penetration depth of thermal/photothermal [[03 Concepts/Glossary/Thermal Damage\|collagen denaturation]], assessed histologically via elastin Van Gieson (EVG) staining and calibrated ocular micrometer, by two examiners, using a mixed-effect statistical model with Tukey adjustment | UNKNOWN | Materials and Methods §2.2–2.3 | FACT |
| Power loss | UNKNOWN — not reported; this study does not measure power output or power loss | UNKNOWN | UNKNOWN | UNKNOWN |
| Calibration method | UNKNOWN — power/energy [[03 Concepts/Glossary/Calibration\|calibration]] not described (no power-meter measurement was performed); histological measurement used a "calibrated ocular micrometer" (calibration protocol not further detailed) | UNKNOWN | Materials and Methods §2.2 | UNKNOWN (power) / FACT (label only, ocular micrometer) |
| Sample | Bovine mandibles from freshly slaughtered cows; 2 posterior teeth randomly selected per mandible per group, 4 mandibles total; 4 gingival samples per experimental group (8 experimental groups: 2 wavelengths × 2 modes × initiated/non-initiated); histomorphometric measurements N=96 per group (individual measurement points, not independent biological replicates) | UNKNOWN | Materials and Methods §2.1; Table 1 | FACT |

## Results — penetration depth by group (Table 1)

| Group | N | Mean (mm) | SD | Min | Max |
| --- | --- | --- | --- | --- | --- |
| 970 nm CW Non-Initiated | 96 | 0.131 | 0.161 | 0 | 0.46 |
| 445 nm CW Non-Initiated | 96 | 0.22 | 0.15 | 0 | 0.6 |
| 970 nm CW Initiated | 96 | 0.20 | 0.14 | 0 | 0.8 |
| 445 nm CW Initiated | 96 | 0.35 | 0.20 | 0.09 | 0.8 |
| 445 nm Pulsed Initiated | 96 | 0.13 | 0.14 | 0 | 0.48 |
| 445 nm Pulsed Non-Initiated | 96 | 0.13 | 0.15 | 0 | 0.5 |
| 970 nm Pulsed Initiated | 96 | 0.10 | 0.10 | 0 | 0.46 |
| 970 nm Pulsed Non-Initiated | 96 | 0.01 | 0.05 | 0 | 0.25 |

- FACT: The source's own Table 1 reports the 970 nm pulsed group means as 0.105 mm (initiated) and 0.015 mm (non-initiated) in the Results narrative text, versus 0.10 mm and 0.01 mm in Table 1 itself — a minor rounding discrepancy between text and table, preserved here rather than silently reconciled.
- FACT: Statistically significant comparisons reported by the source: 970 nm vs. 445 nm within CW non-initiated (p < 0.001); 970 nm vs. 445 nm within CW initiated (p < 0.001); 970 nm initiated vs. non-initiated within Pulsed mode (p < 0.001); 445 nm initiated vs. non-initiated within Pulsed mode (p = 0.7939, not significant).
- FACT / internal inconsistency flagged, not resolved: the source's Abstract states "The initiated tip groups tended to display a lower penetration depth than noninitiated groups." However, the source's own Table 1 data show the opposite direction wherever a significant difference was found: 445 nm CW initiated (0.35 mm) > non-initiated (0.22 mm); 970 nm CW initiated (0.20 mm) > non-initiated (0.131 mm); 970 nm Pulsed initiated (0.10 mm) > non-initiated (0.01 mm). The Discussion section explicitly states "the 970 nm initiated laser group showed a significantly greater thermal penetration depth when compared to the non-initiated group" — directly contradicting the Abstract's general directional claim. This vault preserves the Abstract's stated claim and the Table 1/Discussion data as reported, without silently correcting either. NEEDS VERIFICATION.
- NEEDS VERIFICATION: no explicit statistical test (p-value) comparing initiated vs. non-initiated tips within CW mode is reported in Table 1 or the Results narrative — Table 1's p-values for the CW rows compare wavelengths (445 nm vs. 970 nm) within a given tip-initiation status, not initiated vs. non-initiated within a given wavelength. The Discussion's claim of a "significant" CW initiated-vs-non-initiated difference (970 nm) is therefore not traceable to an explicit p-value in this source as extracted.

## Notes

- FACT: The study measures thermal/collagen-denaturation penetration depth as a proxy for photothermal tissue effect, not laser power output; it is therefore recorded in this vault as operating-parameter and tip-initiation-comparison evidence, not as power-loss or measured-output-deviation evidence.
- FACT: The same device model (SIROLaser Blue, Dentsply Sirona) is used here as in [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output|Xue et al. 2022]] (445 nm and 970 nm/980 nm wavelengths in both). This is a device-model overlap between two vault sources, but because this study reports no measured-output power value, the overlap cannot be used to corroborate or compare Xue et al.'s set-vs-measured power deviation findings for this device.
- FACT: The tip-initiation protocol (dark blue articulating paper, Accufilm, applied 5 sec) is directly comparable in method (though not in paper/brand) to [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]]'s [[03 Concepts/Glossary/Initiated Tip|initiated-tip]] protocol (also articulating paper), and stands in contrast to [[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters|Gutiérrez-Corrales et al. 2020]]'s deliberately non-initiated bare-fiber protocol.
- FACT: [[03 Concepts/Glossary/Pulsed Mode|Pulsed]] mode showed lower penetration depth than [[03 Concepts/Glossary/Continuous Wave|continuous-wave]] mode at the same nominal power setting (2 W) for both wavelengths, consistent across initiated and non-initiated groups.
- FACT: 445 nm wavelength showed significantly greater penetration depth than 970 nm across matched initiation/mode conditions where tested (CW initiated, CW non-initiated).
- INTERPRETATION (the source's own framing, not independently re-derived here): the source attributes the 445 nm vs. 970 nm difference to higher hemoglobin/melanin absorption at 445 nm, and attributes the pulsed-vs-CW difference to thermal relaxation of tissue between pulses.
- HYPOTHESIS: UNKNOWN — the source draws no formal hypothesis regarding power output; its stated conclusion calls for further study specifically to "better compare initiated and non-initiated tips using the novel blue laser light," implying the initiated/non-initiated comparison is treated by the authors themselves as unresolved.
- Limitation (source-stated): bovine mandibles were from relatively young animals without periodontally diseased tissue; localized gingival pigmentation was not controlled for in randomization, which may affect thermal penetration given diode-laser affinity for hemoglobin/melanin.
- Classification for this vault: supporting evidence for tip-initiation status and operating-parameter comparison (wavelength, mode) on tissue effect; explicitly NOT power-loss or measured-output-deviation evidence, per this vault's evidence workflow.

## สรุปภาษาไทย

- งานวิจัยนี้เป็นหลักฐานสนับสนุน (supporting) สำหรับพารามิเตอร์การทำงานและสถานะปลายไฟเบอร์ (initiated vs. non-initiated) ไม่ใช่หลักฐานการสูญเสียกำลังหรือส่วนต่างกำลังขาออกโดยตรง เนื่องจากวัดความลึกของผลกระทบทางความร้อนต่อเนื้อเยื่อ (penetration depth) ไม่ใช่กำลังขาออกด้วยเพาเวอร์มิเตอร์
- ใช้เครื่อง SIROLaser Blue (Dentsply Sirona) ซึ่งเป็นอุปกรณ์รุ่นเดียวกับที่ Xue et al. 2022 ใช้ แต่เนื่องจากงานนี้ไม่ได้วัดกำลังขาออกจริง จึงไม่สามารถนำมาเปรียบเทียบผลส่วนต่างกำลังกับ Xue et al. ได้โดยตรง
- พบข้อขัดแย้งภายในแหล่งข้อมูลเอง: บทคัดย่อระบุว่าปลายไฟเบอร์แบบ initiated ให้ความลึกการซึมผ่านความร้อน "ต่ำกว่า" แบบ non-initiated แต่ตารางผลลัพธ์และส่วนอภิปรายของงานวิจัยกลับแสดงตรงกันข้าม คือ initiated ให้ค่าสูงกว่า non-initiated ในทุกคู่ที่มีนัยสำคัญทางสถิติ ข้อขัดแย้งนี้ถูกบันทึกไว้ตามที่ปรากฏจริงโดยไม่มีการแก้ไขเอง (NEEDS VERIFICATION)
- โหมดพัลส์ (pulsed) ให้ความลึกการซึมผ่านความร้อนน้อยกว่าโหมดต่อเนื่อง (continuous wave) ที่กำลังตั้งเท่ากัน (2 W) และความยาวคลื่น 445 nm ให้ผลลึกกว่า 970 nm
