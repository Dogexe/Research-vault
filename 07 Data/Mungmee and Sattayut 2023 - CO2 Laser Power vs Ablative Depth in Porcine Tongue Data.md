---
classification: SUPPORTING TECHNICAL (methods precedent — immediate cutting outcome)
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: false
wavelength_nm: 10600
set_power_w: [3, 4, 5, 6, 7, 8, 9, 10]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: true
speed_mm_s: 2.5
speed_control: mechanized
speed_varied: false
cw_pw: "CW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: "non-contact"
histology: false
thermal_damage: false
thermal_damage_measure: null
margin_quality: null
tissue_architecture: null
specimen_interpretability: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.3390/life13010162|Mungmee & Sattayut 2023]]
- Citation: Mungmee A, Sattayut S. An in vitro study of the effect of CO2 laser power output on ablative properties in porcine tongue. *Life (Basel)*. 2023;13(1):162.
- Source link: https://doi.org/10.3390/life13010162
- Source locator: Full text read from local Zotero PDF-text cache (zotero storage F7U95CHL) on 2026-10-09; §2.1–2.6, §3.1–3.5, Tables 1–4, Discussion.

## Parameters

| Parameter | Value | Unit | Locator | Label |
|---|---|---|---|---|
| Device | CO2 laser, Sphere FX Phototherapy unit, Model ST-2500 (Thailand); articulated arm | — | §2.3 | FACT |
| Wavelength | 10,600 | nm | §2.3 | FACT |
| Set power | 3, 4, 5, 6, 7, 8, 9, 10 (8 groups) | W | §2.3 | FACT |
| Measured output power | UNKNOWN — not reported (title "power output" refers to set power units) | — | — | UNKNOWN |
| Operating mode | Continuous wave | — | §2.3 | FACT |
| Spot size / focal length | 0.2 mm diameter; focal length 20 mm | mm | §2.3 | FACT |
| Power density (source-calculated) | 9548.1 (3 W) to 31,826.9 (10 W) | W/cm² | §2.3 | FACT |
| Contact mode | Non-contact (articulated arm, focal handpiece) — inferred from delivery system description | — | §2.3 | INTERPRETATION |
| Incision speed | 2.5 mm/s controlled linear movement (Discussion restates as 0.25 cm/s) | mm/s | §2.4; Discussion | FACT |
| Incision length / passes | 1 cm; single pass at midline of tissue surface | — | §2.4 | FACT |
| Tissue tension | 100 g pendulums on both sides via soft-tissue hooks | g | §2.4 | FACT |
| Smoke evacuation | External evacuation (COXO C-AS) | — | §2.4 | FACT |
| Sample | 112 tissue blocks, 2 × 1 × 2 cm, ventral surface mucosa of fresh swine tongue; 8 groups × 14; block randomisation | — | §2.1–2.2 | FACT |
| Storage | Text states "frozen at 4 °C immediately after removal"; brought to 25 °C; experiment within 24 h after sacrifice | — | §2.2 | FACT (4 °C is refrigeration temperature — wording as published) |
| Sample-size basis | n/group = 2(Zα/2+Zβ)²δ²/Δ², α 0.05, β 0.2, δ = 0.108 (from Wilder-Smith et al.), Δ = 0.115 mm → 14/group | — | §2.1 | FACT |
| Outcome measurement | Immediate side-view photograph at fixed distance/angle/focal length on tripod; depth (mean of distance surface→bottom on both sides) and width (at bottom of incision) measured in ImageJ | — | §2.4–2.5 | FACT |
| Reliability | Intra-examiner ICC 0.864 (95% CI 0.513–0.967) to 0.992 (0.967–0.998) | — | §3.1 | FACT |
| Depth result | Median 0.527 mm (3 W) to 3.750 mm (9 W); 10 W median 3.388 mm; 9 vs 10 W not significant | mm | Table 1–2 | FACT |
| Correlation / regression | Pearson r = 0.81 (p < 0.001); depth (mm) = 0.491 × W − 0.731 | — | §3.3 | FACT |
| Width result | Mean 0.147 mm (3 W) to 0.700 mm (9 W) | mm | Table 3 | FACT |
| Ethics | IRB "Not applicable" | — | back matter | FACT |

## Notes

- FACT: Authors justify immediate fresh-tissue photography over histology (shrinkage/distortion) and over endodontic-file measurement (risk of penetrating tissue, over-recording).
- FACT: Authors argue a single pass is preferable because re-irradiating carbonised surface shifts absorption to carbon.
- INTERPRETATION: The prediction equation is specific to this CO2 device, spot size, speed and tension; not transferable to 980 nm diode contact cutting.
- FACT: The study uses the term *in vitro* for fresh porcine tongue tissue blocks.

## สรุปภาษาไทย

งานต้นแบบด้านวิธีวัดผลการตัดทันทีของกลุ่มวิจัย มข.: CO₂ laser 3–10 W แบบต่อเนื่อง ตัดบล็อกลิ้นสุกรด้านล่าง ดึงตึง 100 g ความเร็ว 2.5 mm/s ยาว 1 cm ลากครั้งเดียว ถ่ายภาพด้านข้างทันทีและวัดด้วย ImageJ ความลึกสัมพันธ์กับกำลัง (r = 0.81) แต่ไม่ได้วัดกำลังจริง และสมการทำนายใช้ได้เฉพาะเงื่อนไขของงานนี้
