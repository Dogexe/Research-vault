# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: SUPPORTING/BACKGROUND evidence for repeated-use output stability and fiber degradation — not dental, and not core dental set-power vs. measured-output evidence.** This source is an endovenous laser ablation (EVLA) study (varicose vein treatment), not a dental application, and its device is not a dental diode laser. It is retained because its fiber-tip power measurement methodology and repeated-use/fiber-degradation findings are directly analogous to the vault's dental power-loss question.

## Source

- Literature note: [[02 Literature/10.1016/j.jvsv.2020.10.018|Davies et al. 2020]]
- Source link: https://doi.org/10.1016/j.jvsv.2020.10.018
- Source locator: Abstract; Article Highlights; Methods; Results; Table I; Table II; Discussion; Conclusions
- Citation as published: Davies CE, Riley MI, Dabbs EB, Whiteley MS. Comparison of laser power output from the fiber tip during endovenous laser ablation against displayed power and the "first treatment" effect. *J Vasc Surg Venous Lymphat Disord*. 2021;9(4):1051-1056. (Published online Dec 2, 2020; print issue July 2021.)

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Not explicitly named in text as a specific commercial model. An endovenous laser ablation (EVLA) console and fiber; a 1470 nm "Elli 810/980" and a "Venacure 1470Nm" diode laser system are cited only as reference-list operating manuals (refs. 6, 10), not stated in-text as the study device | UNKNOWN | Methods; References 6, 10 | UNKNOWN |
| Manufacturer | UNKNOWN (not stated in-text; see Device row) | UNKNOWN | UNKNOWN | UNKNOWN |
| Wavelength | 1470 | nm | Abstract; Methods | FACT |
| Set power (console-displayed) | 5 | W | Abstract; Methods | FACT |
| Measured output power | Not reported as a direct power-meter wattage value. Measured indirectly via calorimetry (water-bath temperature rise): expected temperature rise if console power fully delivered = 9.5°C; actual measured rises ranged 5.0°C–6.5°C, i.e., approximately 60% of the calorimetrically expected value | °C (converted by source to an implied % of expected power) | Methods; Results; Table I | FACT |
| Average power | Same as console set power for this CW protocol; not reported as a separate field | UNKNOWN | UNKNOWN | UNKNOWN |
| Peak power | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Operating mode | Continuous firing for a fixed duration per trial (described as fired "continuously"); not labeled CW/pulsed using dental terminology | UNKNOWN (effectively continuous-wave) | Methods | FACT |
| Pulse duration | UNKNOWN (not pulsed) | UNKNOWN | UNKNOWN | UNKNOWN |
| Frequency | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Duty cycle | UNKNOWN | UNKNOWN | UNKNOWN | UNKNOWN |
| Fiber diameter | UNKNOWN (not reported) | UNKNOWN | UNKNOWN | UNKNOWN |
| Tip type | EVLA fiber tip, suspended directly in a water target (not applied to tissue); three separate fibers tested | UNKNOWN (detail) | Methods; Fig 1 | FACT |
| Tip initiation status | UNKNOWN — not applicable; this is not a dental initiated/non-initiated tip protocol | UNKNOWN | UNKNOWN | UNKNOWN |
| Contact mode | UNKNOWN — not applicable; fiber tip was immersed in a water bath, not tissue | UNKNOWN | UNKNOWN | UNKNOWN |
| Exposure duration | 120 sec (2 min) per standard firing (six firings per fiber); one extended firing of 1200 sec (20 min) per fiber to test degradation | sec | Methods | FACT |
| Measurement method | Calorimetric: two thermocouples in a thermally insulated 25 mL beaker containing 15 mL distilled water, connected to a Thermocouple Data Logger (TC-08) and Picolog software; energy delivered calculated from ΔQ = mcΔT (specific heat capacity of water = 4.2 J/g/°C). This is NOT a direct optical power-meter measurement at the fiber tip | UNKNOWN (detail beyond above) | Methods | FACT |
| Power loss | Measured water-heating effect was approximately 40% lower than the value calorimetrically expected from the console-displayed 5 W setting (i.e., ~60% of expected power accounted for) | % (approximate, source's own calculation, with stated model limitations) | Results; Discussion | FACT |
| Calibration method | UNKNOWN — no calibration protocol, certificate, or traceability described for the thermocouple/data-logger measurement system | UNKNOWN | UNKNOWN | UNKNOWN |

## Notes

- FACT: A significant "first treatment effect" was found: the first firing of a new fiber on a given laser console produced a significantly lower temperature rise (power output) than the second and third firings of the same fiber (P = .0004 and P < .0001, respectively). The source describes this as approximately a 15% power decrease relative to subsequent treatments.
- FACT: Pre-warming the laser console for 1 hour without firing the diode did not change this first-treatment pattern (P = .293), which the authors interpret as evidence the effect originates in the diode itself (its first use per session), not in console/electronics warm-up.
- FACT: No evidence of fiber degradation-related power loss was found within the manufacturer-recommended fiber lifetime limit (~10,000 J): temperature rises from firings before a 1200-second (20-minute) continuous firing did not differ significantly from firings after it.
- FACT: The source cites (as background, not as its own finding) that EU/IEC regulation (IEC 60601-2-22) permits laser consoles to have an inherent power-display inaccuracy of up to ±20%; this is the source's own citation of a regulatory standard, not a value the vault has independently verified.
- FACT: Three separate fibers were tested (one per day, one console), six standard firings each (5 W, 120 sec), plus one 1200-second continuous firing per fiber for the degradation test; total study design uses one laser console, one wavelength (1470 nm), and one power setting (5 W).
- INTERPRETATION (the source's own framing, not independently re-derived here): the authors attribute the first-treatment effect to reduced diode efficiency on first activation each session, not to any tested mechanical or console-level cause.
- HYPOTHESIS: UNKNOWN — the source proposes no formal hypothesis; it recommends the same protocol be repeated across other EVLA consoles/fibers and at other power settings (Discussion).
- Classification for this vault: supporting/background evidence for repeated-use power-output stability (a "first treatment effect") and for the absence of measurable fiber-degradation loss within a stated use limit. Not dental, not a core set-power-vs-measured-output source, and its measurement method (calorimetry, not a fiber-tip optical power meter) differs methodologically from the vault's dental core sources.

## สรุปภาษาไทย

- งานวิจัยนี้เป็นหลักฐานสนับสนุน (supporting/background) ไม่ใช่หลักฐานหลักของทันตกรรม เนื่องจากเป็นการศึกษาเลเซอร์ไดโอด 1470 nm ที่ใช้รักษาเส้นเลือดขอด (endovenous laser ablation) ไม่ใช่เลเซอร์ไดโอดทางทันตกรรม
- พบว่ากำลังขาออกจริงที่วัดได้ (โดยวิธีวัดอุณหภูมิน้ำ ไม่ใช่เพาเวอร์มิเตอร์โดยตรง) ต่ำกว่าค่าที่คำนวณคาดหวังจากค่าที่แสดงบนหน้าปัดประมาณ 40%
- พบปรากฏการณ์ "first treatment effect" คือการยิงเลเซอร์ครั้งแรกของไฟเบอร์แต่ละเส้นให้กำลังต่ำกว่าครั้งถัดไปอย่างมีนัยสำคัญ (ประมาณ 15%) และไม่หายไปแม้อุ่นเครื่องคอนโซลไว้ล่วงหน้า 1 ชั่วโมง
- ไม่พบหลักฐานการเสื่อมสภาพของไฟเบอร์ (fiber degradation) ทำให้กำลังลดลง ภายในขีดจำกัดการใช้งานที่ผู้ผลิตแนะนำ (10,000 J)
- ผลการศึกษานี้ไม่สามารถนำมาใช้แทนหลักฐานกำลังขาออกของเลเซอร์ไดโอดทางทันตกรรมได้โดยตรง เนื่องจากอุปกรณ์ ความยาวคลื่น และบริบทการใช้งานต่างกัน
