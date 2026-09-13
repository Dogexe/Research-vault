# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.1097/SCS.0000000000004734|Isola et al. 2018]]
- Source link: https://doi.org/10.1097/SCS.0000000000004734
- Source locator: Full text (PDF) — Abstract; Methods (Healing Parameters; Statistical Analysis); Results; Table 1; Discussion

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Doctor Smile Diode Laser (Vicenza, Italy) | — | Methods | FACT |
| Manufacturer | Doctor Smile (as printed) | — | Methods | FACT |
| Wavelength | Printed in the source PDF as "? 810" nm — the character preceding "810" is a garbled/corrupted symbol in the source PDF (likely "λ" or "≈"); the numeral itself reads 810 nm consistently in both the Introduction and Methods | nm | Introduction; Methods | FACT (810, with an unresolved OCR artifact on the preceding symbol — not treated as a separate reported value) |
| Set power | UNKNOWN — no wattage value is reported anywhere in this paper's full text | W | — | UNKNOWN |
| Independently measured power | UNKNOWN — no power measurement of any kind (set or independently verified) is reported | — | — | UNKNOWN |
| Average power | UNKNOWN | W | — | UNKNOWN |
| Peak power | UNKNOWN | W | — | UNKNOWN |
| Operating mode | Pulsed wave (PW) — explicitly stated ("pulsed-wave mode") | — | Methods | FACT |
| Pulse duration | UNKNOWN — not reported | — | — | UNKNOWN |
| Frequency | UNKNOWN — not reported | — | — | UNKNOWN |
| Duty cycle | UNKNOWN — not reported | — | — | UNKNOWN |
| Fiber diameter | UNKNOWN — not reported | μm | — | UNKNOWN |
| Tip type | UNKNOWN — only "fiber tip" referenced generically | — | — | UNKNOWN |
| Tip initiation status | Not described using the "initiated/non-initiated" vocabulary used elsewhere in this vault, but a functionally equivalent hot-tip protocol is described: "The fiber end of the laser was controlled at every irradiation to check for a carbonized tip (hot tip), required to generate enough thermal energy to cause tissue coagulation at the incision line. Excess carbonized debris was removed with wet gauze." | — | Methods | FACT (hot-tip maintenance protocol; not verbatim "initiated") |
| Contact mode | Contact mode — "the fiber tip touching the gingival epithelium" | — | Methods | FACT |
| Exposure duration | Total surgical intervention time (incision start to final suture, not laser-on time alone): diode 221.15 ± 220.89 s vs. cold blade 316.10 ± 248.69 s (P < 0.05). This must **not** be conflated with laser-only exposure or incision time — it spans the entire surgical procedure | s | Results; Table 1 | FACT |
| Measurement method | No power meter or power measurement method is described anywhere. Thermal safety was monitored in real time via continuous infrared thermographic monitoring with an 80°C threshold as the target (a thermal-safety control, not a power measurement) | — | Methods | FACT (thermal monitoring only; no power measurement) |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN — not applicable, no power measurement reported | — | — | UNKNOWN |
| Incision / cutting speed | **Two distinct speed values are reported in this paper and must not be merged:** (a) an operator TARGET handpiece speed — "The tip was moved at a constant speed of 2.5 mm/s, evaluated visually, to minimize gingival thermal damage" — this is a visually-estimated intraoperative target, not mechanized or instrument-measured; (b) a separately defined, MEASURED/calculated primary outcome variable, "speed of incision" (Sinc) = surgical field perimeter ÷ incision time, timed with a digital chronometer and measured with a millimeter scale by a single observer — Diode: 0.61 ± 0.29 mm/s; Cold blade: 1.47 ± 1.23 mm/s (P < 0.05) | mm/s | Methods (Healing Parameters); Results; Table 1 | FACT — both values reported; (a) = visually-controlled target, (b) = measured outcome metric; they are not the same quantity and the paper does not reconcile them |
| Sample | 21 patients (10 male, 11 female; 19–66 years, mean 46.5), human, in vivo randomized clinical trial (RCT); pyogenic granuloma (PG) excision; diode group n=10 (4M/6F), cold-blade group n=11 (6M/5F) | — | Methods; Results | FACT |

## Notes

- FACT: This is the only one of the four papers processed in this batch that is a genuine human, in vivo, diagnostic excisional-biopsy pathway — a pre-treatment 2×2 mm biopsy punch and a post-excision specimen were both taken and histologically examined (H&E) for each patient, with giant-cell epulis/PG histology described narratively (nonencapsulated connective tissue stroma, proliferating fibroblasts, fibroangiomatous stroma with hemorrhage/hemosiderin/inflammatory cells, ulceration of gingival mucosa, giant cells, ossification).
- FACT: The histologic description is qualitative and narrative only. Unlike [[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|Al-Ani et al. 2024]], this paper does **not** report a formal epithelial/connective-tissue damage score, a thermal-damage-zone measurement in μm, or a specimen-margin distance. It also does not report a diagnosis-affected/not-affected or diagnostic-yield metric distinguishing the diode and cold-blade groups — the closest outcome to a diagnostic-quality metric is the clinical recurrence rate (diode: 1/10 patients at 3 weeks post-op; cold blade: 2/11 patients at 3 and 5 weeks post-op), which is a clinical-recurrence outcome, not a histopathologic-diagnostic-quality outcome.
- FACT: No power value (set or measured) appears anywhere in the full text — this is a complete gap for the power axis of this vault's novelty chain, confirmed at full-text level (not merely absent from the abstract).
- INTERPRETATION: Of the four papers processed in this batch, Isola et al. 2018 is the closest match on the "diagnostic human biopsy + measured incision-behavior" axis specifically, while [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] are closest on the "measured power + controlled speed + histologic thermal effect" axis. No single paper in this batch unifies both axes; this paper's total absence of power data is itself the specific reason it cannot do so.
- HYPOTHESIS: UNKNOWN — no explicit null hypothesis regarding power, speed, or diagnostic yield is stated; the study's stated aim is a general comparison of diode laser vs. cold blade for PG excision on intraoperative and patient-reported parameters.
- Classification for this vault: PARTIAL/supporting evidence for the incision-speed and human-diagnostic-biopsy axes; **not** usable for the power-measurement axis (complete UNKNOWN).

## สรุปภาษาไทย

- บทความนี้เป็นการศึกษาแบบ RCT ในมนุษย์จริง เปรียบเทียบเลเซอร์ไดโอด (810 nm, PW) กับใบมีดผ่าตัดในการตัด pyogenic granuloma โดยมีการตรวจชิ้นเนื้อทางพยาธิวิทยาทั้งก่อนและหลังการผ่าตัดจริง — เป็นบทความเดียวใน 4 ฉบับนี้ที่เป็นเส้นทาง biopsy วินิจฉัยจริงในมนุษย์
- **ไม่มีการรายงานค่ากำลังเลเซอร์ใด ๆ เลย** ทั้งค่าตั้งและค่าที่วัดได้จริง ตลอดทั้งบทความ
- มีค่าความเร็ว 2 ค่าที่ต้องแยกจากกัน: (1) ความเร็วเป้าหมายที่ผู้ปฏิบัติงานประเมินด้วยสายตา (2.5 มม./วินาที) และ (2) ความเร็วตัดที่คำนวณจากเส้นรอบรูปสนามผ่าตัดหารด้วยเวลา ซึ่งเป็นผลลัพธ์หลักที่วัดได้จริง (0.61 มม./วินาที สำหรับกลุ่มไดโอด)
- ไม่มีคะแนนความเสียหายของเนื้อเยื่อทางจุลพยาธิวิทยาแบบเป็นระบบ และไม่มีตัวชี้วัดคุณภาพการวินิจฉัยแบบเปรียบเทียบระหว่างกลุ่ม

## Related notes

- Literature: [[02 Literature/10.1097/SCS.0000000000004734]]
- Synthesis: [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[90 Agent/Search Reports/Novelty Verification - Measured Power and Incision Speed/Novelty Verification Report]]
