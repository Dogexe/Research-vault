---
classification: SUPPORTING TECHNICAL (parameter-effect precedent — immediate macroscopic incision score)
oral_tissue: false
ex_vivo: true
human_tissue: false
diode_laser: false
wavelength_nm: 10600
set_power_w: [10.4, 235]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: true
speed_mm_s: [40, 2830]
speed_control: mechanized
speed_varied: true
cw_pw: "CW+PW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: "non-contact"
histology: false
thermal_damage: true
thermal_damage_measure: "Hohmann et al. 2022 macroscopic 1–5 score (colour/darkened area) applied to the 'cutting front'; 5 = best"
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

- Literature note: [[02 Literature/10.1038/s41598-024-51449-1|Hohmann et al. 2024]]
- Citation: Hohmann M, Kühn D, Ni D, Späth M, Ghosh A, Rohde M, Stelzle F, Klämpfl F, Schmidt M. Relevant parameters for laser surgery of soft tissue. *Sci Rep*. 2024;14(1):1263. PMID 38218912; PMCID PMC10787782.
- Source link: https://doi.org/10.1038/s41598-024-51449-1
- Source locator: Full text read from local Zotero PDF (storage 94SIJA8Y) on 2026-10-11; Methods, Tables 1–11, Fig. 2–6, Limitations, Conclusion.
- Scoring-method source: [[07 Data/Hohmann et al 2022 - Macroscopic Laser Incision Scoring System Reliability Data|Hohmann et al. 2022]]

## Parameters

| Parameter | Value | Unit | Locator | Label |
|---|---|---|---|---|
| Device | MICROSTORM diffusion-cooled CO2 laser (FEHA LaserTec, Germany), acousto-optical modulator driven by external pulse generator (Rigol DG1032Z); Scanlab scan head | — | Experimental procedure | FACT |
| Wavelength | 10.6 | µm | Table 1 | FACT |
| Temporal beam shape | Rectangular | — | Table 1 | FACT |
| Focus distance / spot size | 13.7 cm lens-to-tissue; 258 µm | — | Table 1 | FACT |
| Contact mode | Non-contact (scan-head beam at 13.7 cm focal distance) | — | Table 1; Fig. 1 | INTERPRETATION (not stated as a term) |
| Incident angle | ≈ 0° | — | Table 1 | FACT |
| Incision | 1 cm long; 20 scans per incision; 10 ms scan time; depth up to 4 mm | — | Experimental procedure | FACT |
| Breaks between scans | 1, 3 or 19 breaks of 2 s | — | Experimental procedure; Table 3 | FACT |
| Measured output power | UNKNOWN — no power-meter verification described | — | — | UNKNOWN |
| Tissue | 1 cm thick pork topside (food quality, local butcher) | — | Experimental procedure | FACT |
| Total cuts | 1,710 (non-laser parameters 1,440 cuts, 6 animals; laser parameters 270 cuts, 3 animals); n = 30 per parameter setting | — | Abstract; Table 2 | FACT |
| Experiment A | Air cooling (on/off), breaks (1/3/19), pulse duration (CW 10 ms, 100 µs, 964 ns); at 83 W (160 kW/cm²) and 129 W (247 kW/cm²); scan speed 1 m/s | — | Influence non-laser parameters; Table 3 | FACT |
| Experiment B | Plume exhaust (off, 90°, 45°), breaks, air cooling; 129 W, 964 ns | — | Table 3 | FACT |
| Laser-parameter experiment | Line energy El = P / v_scan: 83, 172, 235 J/m; 3 power/speed pairs each; speed 0.04–2.83 m/s; power 10.4–235 W | — | Eq. 1; Table 4; Fig. 6 | FACT |
| Power/speed pairs (Fig. 6 labels) | 83 J/m: 50 W @ 0.60 m/s, 83 W @ 1.00 m/s, 235 W @ 2.83 m/s; 172 J/m: 27 W @ 0.16, 172 W @ 1.00, 235 W @ 1.37 m/s; 235 J/m: 10 W @ 0.04, 120 W @ 0.51, 235 W @ 1.00 m/s | — | Fig. 6 axis labels | FACT |
| Statistics | Mann–Whitney U (α tiers 0.01/0.001/0.0001/0.00001); ANOVA (statsmodels) with partial η²; animal as factor (benchmark) | — | Statistical analysis | FACT |
| ANOVA, 83 W | Breaks ∂η² 0.19 (p 3e-23); air 0.01 (p 0.04); pulse duration 0.04 (p 2e-05); animal 0.09 (p 6e-10); adj. R² 0.38 | — | Table 5 | FACT |
| ANOVA, 129 W | Breaks 0.32 (p 4e-41); air 0.03 (p 3e-5); pulse duration 0.01 (p 0.01); animal 0.04 (p 2e-5); adj. R² 0.45 | — | Table 6 | FACT |
| ANOVA, exhaust (129 W) | Breaks 0.30; air 0.02; exhaust 0.02 (p 0.005); animal 0.07; adj. R² 0.43 | — | Table 7 | FACT |
| ANOVA, laser parameters | Line energy ∂η² 0.54 (p 3e-65); power/speed 0.22 (p 3e-33); animal 0.11 (p 0.003); adj. R² 0.76 | — | Table 8 | FACT |
| Power/speed within line energy | ∂η² 0.11 at 83 J/m; 0.32 at 172 J/m; 0.73 at 235 J/m | — | Tables 9–11 | FACT |

## Notes

- FACT: Lowest tested line energy (83 J/m) gave the best scores. Authors state line energy sets the maximum achievable cut quality, and that a scan speed of ~1 m/s was best at every line energy.
- FACT: More breaks between scans improved scores (attributed to heat dissipation). Pulse duration, air cooling and plume exhaust had small, inconsistent or negligible effects relative to inter-animal variation.
- FACT: Authors state the pulse-duration finding cannot be transferred to near-infrared lasers (CO2 is absorbed superficially), and that CO2 is unsuitable for handheld use because line energy and speed matter so much.
- FACT: Authors list as limitations ex vivo only, one tissue type, porcine tissue, and fixed 1 cm length / fixed focus.
- NEEDS VERIFICATION: Methods say scoring looks at "the rim or the cutting front" and that the whole analysis uses the cutting front because it "could be shown" to be more reliable [ref. 30 = Hohmann 2022]. But Hohmann 2022 reported higher ICC for the cutting *area* (0.71) than the cutting *edge* (0.62). Whether "cutting front" here means CA or CE is ambiguous.
- INTERPRETATION: "Laser power" here is set power from a scanner-driven CO2 system. The paper has no measured-output data and cannot inform display-versus-measured agreement.
- INTERPRETATION: Supports energy-per-length thinking (power ÷ speed) and therefore mechanized speed control in the planned study. It does not supply transferable parameter values for 980 nm contact diode cutting.

## สรุปภาษาไทย

งานต่อยอดของกลุ่มเดียวกัน ใช้ระบบคะแนนปี 2022 ประเมินรอยตัด CO₂ laser (10.6 µm, non-contact, scan head) บนเนื้อหมู 1,710 รอย และวิเคราะห์ด้วย ANOVA โดยเทียบกับความแปรปรวนระหว่างตัวสัตว์ พบว่า line energy (กำลังหารความเร็ว) สำคัญที่สุด (∂η² 0.54) โดย 83 J/m ให้ผลดีที่สุด ความเร็วประมาณ 1 m/s ให้ผลดีทุกระดับ และการหยุดพักระหว่างสแกนช่วยลดความเสียหาย ส่วน pulse duration, air cooling และการดูดควันมีผลน้อย ไม่มีการวัดกำลังจริง และผู้เขียนระบุเองว่าผลเรื่อง pulse duration ใช้กับเลเซอร์ช่วง near-infrared ไม่ได้
