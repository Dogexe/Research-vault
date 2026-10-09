---
classification: SUPPORTING TECHNICAL (same device model as planned study; unpublished student research report)
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: [980, 1064]
set_power_w: [4, 8]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: "not applicable (stationary spot irradiation, 2 s)"
speed_varied: false
cw_pw: "CW+PW"
fiber_diameter_um: [320, 300]
tip_initiation: null
contact_mode: "contact"
histology: false
thermal_damage: false
thermal_damage_measure: null
margin_quality: null
tissue_architecture: null
specimen_interpretability: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/Ablative properties of oral soft tissue resurfacing technique using 980 nm Diode laser and Nd_YAG laser in continuous wave and pulsed modes with India ink  and Methylene blue staining_ A porcine ex vivostudy]]
- Citation (as on report cover): ณัฐชยา ลิ้มธนะกุล, สิริวิชญ์ เทพอวยพร, อาภารัศม์ อัสสมงคล; advisor ศจี สัตยุตม์. Ablative properties of oral soft tissue resurfacing technique using 980 nm Diode laser and Nd:YAG laser in continuous wave and pulsed modes with India ink and Methylene blue staining: A porcine ex vivo study. รายงานการวิจัยทางทันตกรรม คณะทันตแพทยศาสตร์ มหาวิทยาลัยขอนแก่น; ปีการศึกษา 2567.
- NEEDS VERIFICATION: author order for citation — cover lists ลิ้มธนะกุล → เทพอวยพร → อัสสมงคล; an earlier proposal draft cited "Assamongkol A, Limtanakul N, Tepouypon S, Sattayut S". Not peer-reviewed.
- Source locator: Full text read from local Zotero PDF-text cache (zotero storage SZAW2YYP) on 2026-10-09; Abstract; วัสดุอุปกรณ์และวิธีการ; ผลการศึกษา; ตารางที่ 4.

## Parameters

| Parameter | Value | Unit | Locator | Label |
|---|---|---|---|---|
| Device (diode) | Lasotronix Smart M Diode Laser 980 nm (Poland), fibre 320 µm | — | Methods | FACT |
| Device (Nd:YAG) | LightWalker DT, 1064 nm (UK), fibre 300 µm | — | Methods | FACT |
| Diode CW setting | 4 | W | Methods | FACT |
| Diode pulsed setting | Set 8 W with on/off 200 µs "to give average power 4 W" | — | Methods | FACT |
| Nd:YAG settings | SP 0.2 ms and VLP 0.6 ms, 4 W, 50 Hz | — | Methods | FACT |
| Measured output power | UNKNOWN — not measured | — | — | UNKNOWN |
| Exposure | Stationary spot, 2 s per spot, 3 spots per rugae 5 mm apart | s | Methods | FACT |
| Contact / angle | Fibre in contact, perpendicular, held by a laser holding device | — | Methods | FACT |
| Tip initiation | UNKNOWN — not stated | — | — | UNKNOWN |
| Tissue | Porcine maxilla, palatal rugae (flat portions); stored 4 °C, studied within 24 h; brought to room temperature; excess water blotted | — | Methods | FACT |
| Staining | India ink / methylene blue 1% w/v, 0.05 µL per 1.5 cm², 1 min before irradiation; unstained controls | — | Methods | FACT |
| Design | 12 groups × 10 palates × 3 spots = 30 values/group (360 total) | — | Abstract; Results | FACT |
| Measurement | Custom parallelism-control device + 3D laser level; Olympus DSX1000, 5X lens, 16×16 grid; Olympus LEXT analysis for depth, width (circle diameter), volume | — | Methods | FACT |
| Blinding / reliability | 2 readers blinded to laser type/setting; ICC > 0.990 all parameters | — | Methods; Results | FACT |
| Depth, diode CW unstained (DC) | Mean 398.6 µm, SD 176.2 (95% CI 332.8–464.4) | µm | ตารางที่ 4 | FACT |
| Depth, diode pulsed unstained (DP) | Mean 457.0 µm, SD 145.8 (95% CI 402.6–511.4) | µm | ตารางที่ 4 | FACT |
| Depth range across diode groups | 393–673 µm (means) | µm | Results | FACT |

## Notes

- FACT: Study design term used: *ex vivo* ("การศึกษานอกร่างกายสุกร"); described as experimental laboratory study.
- INTERPRETATION: The pulsed-mode description suggests the Smart M pulsed setting entry is a peak (on-time) power with ~50% duty cycle; requires confirmation from the manufacturer manual.
- INTERPRETATION: Spot irradiation (2 s) is not a linear incision; SD values are not directly transferable to linear-cut sample-size calculations.

## สรุปภาษาไทย

รายงานวิจัยนักศึกษาทันตแพทย์ มข. ใช้ Lasotronix Smart M 980 nm (fibre 320 µm) ฉายเป็นจุด 2 วินาทีบนเพดานสุกรแบบสัมผัสตั้งฉาก วัดรอยด้วย Olympus DSX1000/LEXT โดยผู้อ่านปกปิด 2 คน (ICC > 0.990) ความลึกเฉลี่ยไดโอดแบบต่อเนื่องไม่ย้อมสี 398.6 µm (SD 176.2) ไม่ได้วัดกำลังจริง และลำดับผู้แต่งยังต้องยืนยัน
