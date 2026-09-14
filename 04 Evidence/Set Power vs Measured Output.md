# Evidence Note

## Claim

- Claim: Reported panel set power and measured output should be retained as separate values for dental diode devices.
- Scope: Dental diode laser output measurements in Parker et al. 2022, Xue et al. 2022, Zegaib et al. 2011, and Kim et al. 2020.

## Supporting findings

- FACT: Parker et al. measured post-fibre emission for 38 dental diode units at control-panel settings selected from 100 mW, 500 mW, 1.0 W, and 2.0 W, with device-specific values retained in the source table. [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]]
- FACT: Parker et al. mainly found post-fibre output below control-panel settings; the source reports device-specific percentage losses and no study-wide output value. [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]]
- FACT: Xue et al. reported measured mean continuous-wave outputs of 3.6 W, 2.5 W, and 2.3 W for 445 nm, 970 nm, and 810 nm devices set to 3 W, 2 W, and 2.5 W, respectively. [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]]
- FACT: Xue et al. used both continuous-wave and pulsed protocols, with reported pulse duration, frequency, duty cycle, fibre diameter, and measurement method. [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]]
- FACT: Zegaib et al. used a control-panel setting distinct from the clinical treatment setting purely to standardize fibre-tip power measurement (1.0 W CW for measurement vs. 1.7 W CW for periodontal-pocket irradiation), measuring absolute output at the tip before each application. [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]]
- FACT: Zegaib et al. reported measured output consistently below the 1.0 W panel reference in both the contact (study) and non-contact (control) groups, with a mean 9% fibre-transmission loss before tissue contact and progressive contact-induced loss reaching a mean 40.26% by the fourth application. [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]]
- FACT: Kim et al. reported both a set value ("Output Power") and an independently measured value ("Actual Power") for three dental diode devices at 1.0/2.0/3.0 W, using a calibrated power meter (NovaII, Ophir Photonics); the two columns differ from each other at every one of the 9 device × setting combinations reported. [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]]
- FACT (added 2026-09-14): [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] independently checked output with a power meter (PM600, Molectron) before each surgical procedure and reported both the display/console value and the measured value for a 940 nm diode: 1.2 W display → 1.0 W measured, and 1.8 W display → 1.5 W measured (both a ~17% under-delivery). This is an ex vivo oral soft-tissue (pig tongue) study, not a bench power-survey study like Parker/Xue/Zegaib/Kim, but it independently confirms the same set-vs-measured distinction in a device not otherwise represented in this note's core evidence.

## Conflicting findings

- FACT: Xue et al. reported signed mean-output deviations versus preset of +21%, +22%, and −8% in continuous-wave mode, and +37%, +26%, and −3% in pulsed mode for the 445 nm, 970 nm, and 810 nm devices, respectively. [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]]
- FACT: Xue et al. therefore reported both positive and negative deviations by device and mode, unlike the mainly-below-panel pattern reported by Parker et al. [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]]
- FACT: Kim et al. likewise reported both positive (+11.9% to +18.1%, K2 mobile) and negative (−13.9% to −27.3%, Epic 10 TM and Saeshin) deviations, but within one study using a single shared measurement protocol — unlike Xue et al.'s mixed pattern, which spans two devices measured under that study's own separate protocol. [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]] [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]]

## Assessment

- INTERPRETATION: The studies support recording set power and measured output as separate, device-level fields; they do not support calculating one correction factor across devices. [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]] [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]]
- HYPOTHESIS: UNKNOWN
- Limitations: Parker et al. report device-specific table values without a study-wide measured-output aggregate; Xue et al. evaluated two dental devices under specified bench protocols; Zegaib et al. measured a single 810-nm diode unit under a periodontal-curettage protocol, with a source-reported figure ("mean PO loss of 54%" between panel setting and 4th-application tip output) that is arithmetically inconsistent with the study's own Table 1 value (0.54 W remaining of a 1.0 W reference ≈ 46% loss); this is flagged as NEEDS VERIFICATION rather than resolved. Kim et al. measured three devices in vitro (titanium-disc irradiation) and do not report calibration protocol detail beyond describing the power meter as "calibrated." [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]] [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]]
- Uncertainty: Direct numerical comparison is limited by different devices, panel settings, operating modes, fibre characteristics, measurement setups, and calibration reporting. [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]] [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]] [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]]
- Possible explanations for disagreement: INTERPRETATION: Device-level hardware and protocol differences may account for the differing directions of deviation; this requires testing rather than inference. [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]]
- Research gaps: NEEDS VERIFICATION — standardized, multi-device studies reporting complete operating parameters and the same measurement protocol are needed before direct comparison.

## Related notes

- Concepts: [[03 Concepts/Power Output]], [[03 Concepts/Power Loss]], [[03 Concepts/Laser Presetting]], [[03 Concepts/Operating Parameters]]
- Primary evidence: [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]], [[07 Data/Xue et al 2022 - Two Semiconductor Lasers Power Output]], [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]], [[07 Data/Kim et al 2020 - Set vs Actual Power Across Three Dental Diode Lasers]], [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data]]

## สรุปภาษาไทย

- ข้อสรุปของหลักฐานนี้คือ ค่ากำลังที่ตั้งไว้ที่หน้าปัด (set power) และค่ากำลังขาออกที่วัดได้จริง (measured output) ควรถูกบันทึกแยกจากกันเสมอ ไม่ควรนำมารวมหรือแทนค่ากัน
- Parker et al. วัดกำลังขาออกหลังไฟเบอร์ (post-fibre emission) ของอุปกรณ์ 38 เครื่อง ที่ค่าตั้งหน้าปัดหลายระดับ
- Xue et al. ใช้ทั้งโหมดต่อเนื่อง (continuous wave) และโหมดพัลส์ (pulsed) พร้อมรายงานพารามิเตอร์ครบถ้วน
- Zegaib et al. ตั้งค่าหน้าปัดแยกกันระหว่างขั้นตอนการวัด (1.0 W) กับขั้นตอนการรักษา (1.7 W) และพบว่ากำลังขาออกที่วัดได้ต่ำกว่าค่าอ้างอิง 1.0 W ในทุกเงื่อนไขที่วัด
- Kim et al. รายงานค่าตั้งและค่าที่วัดได้จริงคู่กันสำหรับอุปกรณ์ 3 เครื่อง โดยพบว่าค่าทั้งสองต่างกันในทุกคู่ค่าตั้งที่ทดสอบ (รวม 9 คู่)
- ไม่ควรคำนวณ "ตัวคูณแก้ไข" (correction factor) เดียวใช้ร่วมกันทุกอุปกรณ์ เนื่องจากแต่ละแหล่งข้อมูลมีอุปกรณ์ โหมด และโพรโทคอลการวัดต่างกัน

## Related synthesis

- Synthesis note: [[06 Synthesis/Current Evidence on Diode Laser Power Output]]
