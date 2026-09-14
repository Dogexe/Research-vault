---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 940
set_power_w: [1, 6]
measured_power: true
measured_power_value_reported: false
measured_power_w: null
power_meter: "LabMax Top (Coherent) + PM10 detector"
measurement_location: "distal end of fiber"
incision_speed_reported: true
speed_mm_s: 2
speed_control: mechanized
cw_pw: "CW"
fiber_diameter_um: 300
tip_initiation: "initiated"
contact_mode: "contact"
histology: true
thermal_damage: true
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

- Literature note: [[02 Literature/10.1002/lsm.23639|Strakas et al. 2023]]
- Source link: https://doi.org/10.1002/lsm.23639
- Source locator: Full text (PDF) — Abstract; Materials and Methods (Experimental groups; Experimental setup; Histological preparation and evaluation); Table 1; Results; Discussion

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | EpicX (Biolase); maximum output power 10 W CW | — | Materials and Methods (Experimental groups) | FACT |
| Manufacturer | Biolase | — | Materials and Methods | FACT |
| Wavelength | 940 nm | nm | Abstract; Materials and Methods | FACT |
| Set power | 1, 1.5, 2, 2.5, 3, 3.5, 4, 5, 6 W (9 groups, n=6 samples/group), CW, initiated tip | W | Abstract; Materials and Methods | FACT |
| Independently measured power (post-set verification) | YES, as a per-incision QC gate — "Before each incision the laser output power emitted at the [[03 Concepts/Glossary/Measurement Location\|distal end of the fiber]] was measured using a [[03 Concepts/Glossary/Calibration\|calibrated]] [[03 Concepts/Glossary/Power Meter\|power meter]] (LabMax Top; Coherent) and a PM10 detector (Coherent). In case of a ≥5% deviation in the output power, the tip of the laser handpiece was replaced with a new one." Same instrument and protocol as [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] (shared senior author, J. Meister). As with Hanke 2021, the exact measured wattage per incision is **not tabulated separately** from the nominal set value | — | Materials and Methods (Experimental groups) | FACT (verification protocol) / UNKNOWN (exact measured wattage values, not separately reported) |
| Average power | = set power (CW mode) | W | Materials and Methods | FACT |
| Peak power | N/A — CW mode | — | — | N/A |
| Operating mode | Continuous wave (CW) only | — | Abstract; Materials and Methods | FACT |
| Pulse duration | N/A — CW, not applicable | — | — | N/A |
| Frequency | N/A — CW, not applicable | — | — | N/A |
| Duty cycle | N/A — CW, not applicable | — | — | N/A |
| Fiber diameter | "Bare" fiber, 300 μm diameter, 4 mm length, protruding from metal protective cover (E3-4) | μm | Materials and Methods (Experimental groups) | FACT |
| Tip type | Bare fiber, protective cover E3-4 | — | Materials and Methods | FACT |
| Tip initiation status | YES — explicit protocol: initiation performed by a linear incision on the sample at 90° to the direction of the main incisions, producing a carbon layer at the distal fiber end before each set of incisions | — | Materials and Methods (Experimental setup); Fig. 3 | FACT |
| Contact mode | Contact mode only, for all incisions | — | Abstract; Materials and Methods | FACT |
| Exposure duration | Not reported as a fixed time value; incision length not explicitly stated in the extracted text. Incisions generated via mechanized sample movement (see Incision speed row) | — | — | UNKNOWN (length) |
| Measurement method | Power meter (LabMax Top; Coherent) + PM10 detector (Coherent); measurement point = distal end of the fiber; performed before each incision | — | Materials and Methods (Experimental groups) | FACT |
| Power loss / deviation | ≥5% deviation threshold used operationally as accept/reject gate (fiber-tip replacement trigger); actual measured deviation magnitudes not reported numerically | % (threshold only) | Materials and Methods (Experimental groups) | FACT (threshold) / UNKNOWN (actual deviation values) |
| Calibration method | Described only as a "calibrated power meter" — no calibration protocol, certificate, or traceability standard is described | — | — | UNKNOWN |
| Incision / cutting speed | YES — 2 mm/s, constant, via a 3D computer-controlled micropositioner (VT-80; Micos); CONTROLLED/mechanized (same device and protocol as Hanke et al. 2021, which this study explicitly adopts as its methodological guide) | mm/s | Materials and Methods (Experimental setup); Fig. 2 | FACT |
| Contact pressure | p = 0.07 N/mm² (track force F = 0.0035 N; contact area A ≈ 0.05 mm², estimated via blue-ink imprint), checked/recalibrated after every 5 incisions | N/mm² | Materials and Methods (Experimental setup) | FACT |
| Sample | Porcine gingiva, German-land race pigs (2 months old, 30–40 kg), ex vivo; 54 samples (9 groups × n=6) + 2 setup-test samples; 5 incisions/sample = 30 incisions/group | — | Materials and Methods (Preparation of the samples) | FACT |

## Notes

- FACT: This is a controlled, mechanized ex vivo cut-efficiency study, explicitly built as a direct methodological extension of [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] ("a previous study, which investigated other diode laser wavelengths, was adopted" as the research guide), applying the same efficiency-factor concept (γz = cutting depth / total [[03 Concepts/Glossary/Thermal Damage|interaction zone]] depth) to a single new wavelength (940 nm) across 9 power levels. It is not a biopsy or diagnostic study.
- FACT: Highest [[03 Concepts/Glossary/Cutting Efficiency|cutting efficiency]] at 5 W (γz = 0.81 ± 0.03); lowest at 1 W (γz = 0.45 ± 0.11); groups 1.5–5 W met Hanke et al.'s γz ≥ 0.6 "clinical orientation" threshold, 1 W and 6 W did not (6 W showed the largest thermal-damage zone). Linear regression between γz and output power showed only a poor positive correlation (r² = 0.474) — power increases did not translate proportionally into cutting efficiency, replicating Hanke et al.'s central finding at a different wavelength.
- FACT: No patient, no lesion, no biopsy, and no diagnostic outcome appear anywhere in this paper — it is an ex vivo porcine gingival-block cutting-behavior characterization study only.
- INTERPRETATION: As with Hanke et al. 2021, the power-verification protocol here (calibrated power meter, checked before every incision, ≥5% deviation triggering fiber-tip replacement) is methodologically stronger than the single-setup-check pattern already documented in this vault for the Al-Ani et al. 2023/2024 pair, but the actual delivered wattage is not reported as a value distinct from the nominal [[03 Concepts/Glossary/Set Power|set power]].
- HYPOTHESIS: UNKNOWN — the study's own null hypothesis (that different power settings would not influence cutting behavior and thermal damage) was explicitly rejected.
- Classification for this vault: CORE background/methodology source for the power-verification and incision-speed axes; explicitly **not** a biopsy or diagnostic-outcome source.

## สรุปภาษาไทย

- การศึกษานี้ต่อยอดโดยตรงจาก Hanke et al. 2021 (ผู้เขียนอาวุโสร่วมคนเดียวกัน) โดยใช้เลเซอร์ไดโอด 940 nm กำลัง 1–6 W (9 กลุ่ม) ในเหงือกหมู ex vivo ด้วยโปรโตคอลและอุปกรณ์วัดกำลัง/ความเร็วตัดชุดเดียวกันทุกประการ
- มีการวัดกำลังขาออกจริงด้วยเพาเวอร์มิเตอร์ที่สอบเทียบแล้วก่อนตัดทุกครั้ง (เกณฑ์เบี่ยงเบน ≥5%) แต่ไม่รายงานค่าที่วัดได้จริงแยกจากค่าที่ตั้งไว้
- ความเร็วตัดควบคุมคงที่ 2 มม./วินาที ด้วยเครื่อง micropositioner เดียวกับ Hanke et al. 2021
- ไม่ใช่การศึกษา biopsy หรือมีผลการวินิจฉัยทางพยาธิวิทยาใด ๆ

## Related notes

- Literature: [[02 Literature/10.1002/lsm.23639]]
- Related: [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]] (methodological source this study builds on)
- Synthesis: [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[90 Agent/Search Reports/Novelty Verification - Measured Power and Incision Speed/Novelty Verification Report]]
