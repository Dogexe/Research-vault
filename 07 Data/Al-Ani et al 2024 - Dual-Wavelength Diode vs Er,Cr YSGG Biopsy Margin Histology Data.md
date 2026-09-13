# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/https_/doi.org/10.1590/1678-7757-2023-0419|Al-Ani et al. 2024]]
- Source link: https://doi.org/10.1590/1678-7757-2023-0419
- Source locator: Full text (PDF) — Abstract; Methodology (Laser systems; Laser surgical procedure; Histological evaluation); Results; Table 1–3; Discussion; Conclusion

## Special verification: incision speed, per user instruction

**This paper's own Methodology section explicitly states an incision speed, in its own words, independent of the companion 2023 paper:** "The specimens from all four groups were irradiated perpendicularly in contact mode at the same room temperature (27 ºC) and by the same experienced clinician at a speed of 0.75 mm/sec, an incision length of 1.5 cm, and an adjusted exposure time of 20 seconds." (Methodology, "Laser surgical procedure"). This is a direct statement in the 2024 paper's own full text — it is **confirmed present**, not inherited or assumed by analogy from [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]].

The companion-study relationship should still be recorded as a separate fact: the 2024 paper reuses the identical device (Quicklase 12W dual 4), identical two diode power settings (1.5 W / 2.5 W CW), identical incision length (1.5 cm) and exposure time (20 s), and the identical numeric speed value (0.75 mm/s) as Al-Ani et al. 2023 — strongly suggesting a shared experimental protocol/session between the two papers, but this is a note about *provenance*, not a reason to doubt that the 2024 paper reports the value itself. Per instruction, the two studies' data are kept as separate entries in this vault (not merged into one experiment) even though the protocol overlaps.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Diode: Quicklase 12W dual 4 (810+980 nm) (Quicklase, England, UK). Comparator (non-diode): Er,Cr:YSGG Waterlase iPlus (Biolase, California, USA) | — | Methodology (Laser systems) | FACT |
| Manufacturer | Quicklase (diode); Biolase (Er,Cr:YSGG comparator) | — | Methodology | FACT |
| Wavelength | Diode: dual 810 + 980 nm simultaneously. Er,Cr:YSGG comparator: 2780 nm | nm | Abstract; Methodology | FACT |
| Set power | Diode: 1.5 W (G1) and 2.5 W (G2), CW. Er,Cr:YSGG comparator: 2.5 W (G3) and 3.5 W (G4), PW | W | Abstract; Methodology | FACT |
| Independently measured power (post-set verification) | NO, confirmed directly from this paper's own Methodology text (not inferred from the companion paper): "The optical fiber was checked with a power meter (PINTUDY, Guangzhou CN) before the incisions in each group." This is a pre-incision setup check to standardize the fiber output to the target set value, with no independently reported, post-setup measured-output value distinct from the nominal set power — the same pattern already documented in this vault for [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]] | — | Methodology (Laser systems) | FACT (confirmed NO, from this paper's own text) |
| Average power | Diode: 1.5 W / 2.5 W (CW, average = set). Er,Cr:YSGG: average power not separately stated; peak power given instead (see below) | W | Methodology | FACT (diode) |
| Peak power | Er,Cr:YSGG: 71.43 W (G3, 2.5 W/50 mJ) and 100 W (G4, 3.5 W/70 mJ). Diode: UNKNOWN (CW, not applicable) | W | Methodology | FACT (Er,Cr:YSGG) / N/A (diode) |
| Operating mode | Diode: continuous wave (CW). Er,Cr:YSGG comparator: pulsed wave (PW) | — | Abstract; Methodology | FACT |
| Pulse duration | Diode: N/A (CW). Er,Cr:YSGG: 700 μs | μs | Methodology | FACT (Er,Cr:YSGG) / N/A (diode) |
| Frequency | Diode: N/A (CW). Er,Cr:YSGG: 50 Hz | Hz | Methodology | FACT (Er,Cr:YSGG) / N/A (diode) |
| Duty cycle | UNKNOWN — not reported for either laser | — | — | UNKNOWN |
| Fiber diameter | Diode: FC 400 μm single-file multimode. Er,Cr:YSGG: MZ6 tip, 600 μm diameter, 6 mm length | μm | Methodology (Laser systems) | FACT |
| Tip type | Diode: initiated optical fiber (explicitly stated). Er,Cr:YSGG: MZ6 tip | — | Methodology | FACT |
| Tip initiation status | Diode: YES — "used with initiated optical fiber" stated explicitly in the Laser systems section | — | Methodology | FACT |
| Contact mode | Contact mode, both lasers, all groups ("irradiated perpendicularly in contact mode") | — | Methodology (Laser surgical procedure) | FACT |
| Exposure duration | 20 seconds, fixed across all 4 groups, for a 1.5 cm incision length | s | Methodology (Laser surgical procedure) | FACT |
| Measurement method | Power meter (PINTUDY, Guangzhou, China), used to check/standardize the diode fiber output before incisions in each group; not described as independently re-verifying output after setup. Not stated whether measured specifically at the distal fiber tip (unlike Hanke 2021/Strakas 2023's explicit "distal end of fiber" language) | — | Methodology (Laser systems) | FACT |
| Calibration method | UNKNOWN — power meter brand is named (PINTUDY) but no calibration protocol, certificate, or traceability is described | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN — not reported; this study's outcome variables are histologic (epithelial/connective tissue damage scores, lateral thermal damage extent), not power-output accuracy | — | — | UNKNOWN |
| Power density (calculated) | Diode: 1153.8 W/cm² (1.5 W, G1), 1923 W/cm² (2.5 W, G2). Er,Cr:YSGG: 892.8 W/cm² (2.5 W, G3), 1250 W/cm² (3.5 W, G4) | W/cm² | Methodology | FACT |
| Water/air spray | Diode: not applicable/not reported. Er,Cr:YSGG: 10% water, 10% air | % | Methodology | FACT (Er,Cr:YSGG) / UNKNOWN (diode) |
| Incision / cutting speed | YES, explicitly reported in this paper's own text: 0.75 mm/s, fixed across all 4 groups. Described as: "irradiated perpendicularly in contact mode... by the same experienced clinician at a speed of 0.75 mm/sec" — this reads as a CONTROLLED protocol target executed manually by a single experienced clinician (not mechanized via a micropositioner, unlike Hanke 2021/Strakas 2023), and it is not stated whether the 0.75 mm/s figure was independently instrument-measured during each incision or set as a fixed operator target only | mm/s | Methodology (Laser surgical procedure) | FACT (value reported) / interpretation of "controlled vs. measured" nature is UNKNOWN beyond "manual, clinician-executed, fixed protocol target" |
| Sample | 5 sheep tongues (8–17 months old), ex vivo, halved and cut into pieces (10 mm × 20 mm × 15 mm); 28 blocks total, 14 per laser type, 7 per group (G1–G4); 3 H&E slides per block (42 slides per laser type, 21 per group) | — | Methodology (Study design) | FACT |
| Thermal / histologic outcomes | YES, quantified: Epithelial tissue (ET) damage score 0–3 (nuclear changes, cytoplasmic changes, loss of epithelial/sub-epithelial attachment) and Connective tissue (CT) damage score 0–3 (carbonization, desiccation, vascular changes), per Vescovi et al. 2010 criteria; Lateral thermal damage extent (LTDE), measured in μm from incision edge to healthy tissue. Diode significantly higher than Er,Cr:YSGG on all three (P<0.001): ET/CT median 3 (range 2–3) for diode vs. 2 (range 1–3) for Er,Cr:YSGG; LTDE mean 221.24 ± 85.44 μm (diode) vs. 110.6 ± 36.14 μm (Er,Cr:YSGG). G2 (2.5 W diode) was worst on all three criteria (LTDE 271.05 ± 83.56 μm); G3 (2.5 W Er,Cr:YSGG) was best/lowest (LTDE 93 ± 32.43 μm) | μm / ordinal score 0–3 | Results; Tables 1–3; Fig. 1 | FACT |
| Specimen margin findings | Lateral thermal damage extent reported quantitatively per group (see above); none of the four groups exceeded 0.3 mm of surgical margin damage. Authors' own stated clinical recommendation: an additional 0.5–1 mm safety margin of normal tissue beyond the incision, depending on laser wavelength, "in order to minimize any potential damage" | mm | Results; Conclusion | FACT |
| Diagnostic biopsy outcome | NOT reported — this is an ex vivo sheep-tongue model with no lesion and no clinical diagnosis rendered; the outcome is histologic artifact scoring only (ET/CT damage scores, LTDE), explicitly not a diagnosis-affected/not-affected or diagnostic-yield metric | — | — | N/A (ex vivo, non-diagnostic model) |

## Notes

- FACT: This paper directly answers the user's special check — incision speed (0.75 mm/s) is explicitly and independently stated in Al-Ani et al. 2024's own Methodology text, confirmed by full-text read, not carried over by assumption from the 2023 companion paper. The companion-study relationship (same author group, device, power settings, incision length, exposure time, and speed value as [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]]) is recorded separately as provenance context, per instruction not to merge the two studies' data into one experiment.
- FACT: The power meter (PINTUDY) role is confirmed, from this paper's own text, to be identical to its role in the 2023 companion paper — a pre-incision setup/standardization check, not an independent post-setup measured-output report. This closes the user's requirement to verify (not infer) the power-measurement status directly against the 2024 paper itself.
- FACT: This is a substantially more rigorous histologic outcome design than [[07 Data/Isola et al 2018 - Diode Laser Pyogenic Granuloma Excision Speed Data|Isola et al. 2018]] — quantified ordinal damage scores plus a numeric thermal-damage-extent measurement (μm) — but it is an ex vivo animal (sheep tongue) model with no diagnostic pathway, unlike Isola et al. 2018's human in vivo diagnostic biopsies.
- HYPOTHESIS: UNKNOWN — no explicit null hypothesis is stated beyond the general aim of determining "the most effective and safest laser system at the histopathological level."
- Classification for this vault: CORE source for the incision-speed + histologic-damage axis of the novelty chain (dental/oral-relevant ex vivo tissue); confirmed **not** usable for the independently-measured-power or diagnostic-biopsy-outcome axes.

## สรุปภาษาไทย

- บทความปี 2024 นี้ **รายงานความเร็วตัด 0.75 มม./วินาที ไว้เองในเนื้อหา Methodology** อย่างชัดเจน ไม่ได้อนุมานหรือยืมค่ามาจากบทความคู่แฝดปี 2023 — ยืนยันตามที่ผู้ใช้ขอให้ตรวจสอบโดยเฉพาะ
- อุปกรณ์ ค่ากำลังที่ตั้ง ความยาวแผล เวลาสัมผัส และความเร็วตัด เหมือนกับบทความปี 2023 ทุกประการ ชี้ให้เห็นว่าทั้งสองบทความน่าจะมาจากชุดการทดลองเดียวกัน แต่ข้อมูลทั้งสองชุดยังคงถูกเก็บแยกจากกันในคลังนี้ตามคำสั่ง ไม่ผสานเป็นการทดลองเดียว
- เพาเวอร์มิเตอร์ (PINTUDY) ใช้เพียงเพื่อตรวจสอบ/ตั้งค่ากำลังก่อนการตัดในแต่ละกลุ่มเท่านั้น **ไม่มีการรายงานค่ากำลังที่วัดได้จริงแยกจากค่าที่ตั้งไว้** — ยืนยันจากเนื้อหาบทความปี 2024 เอง
- เป็นการศึกษา ex vivo ในลิ้นแกะ ไม่มีรอยโรคจริงและไม่มีการวินิจฉัยทางคลินิก ผลลัพธ์เป็นคะแนนความเสียหายทางจุลพยาธิวิทยาเท่านั้น

## Related notes

- Literature: [[02 Literature/https_/doi.org/10.1590/1678-7757-2023-0419]]
- Companion paper: [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]] (same device/power settings; temperature outcome, not histology)
- Synthesis: [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[90 Agent/Search Reports/Novelty Verification - Measured Power and Incision Speed/Novelty Verification Report]]
