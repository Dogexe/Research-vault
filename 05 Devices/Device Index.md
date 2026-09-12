# Device Index

Index of device notes in this vault. Populated only for devices whose exact model is explicitly reported in a processed vault source, with enough source data to be useful (per `AGENTS.md` § Device Notes). Devices mentioned in the literature only by manufacturer or by laser type (no exact model name) do not get a note — see "Excluded devices" below.

## Devices with independent measured-output data

Independent = measured with a power meter/wattmeter against a set/panel value, not the manufacturer's own claim.

- [[Dentek LD 15]] — 810 nm (Goharkhay et al. 1999); wattmeter-measured output 0.5–4.5 W (panel/set value itself not reported by the source)
- [[SIROLaser Blue]] — 445/970 nm (Xue et al. 2022); measured output +21% to +37% above set power
- [[Picasso]] — 810 nm (Xue et al. 2022); measured output −8% to −3% below set power
- [[K2 Mobile]] — 980 nm (Kim et al. 2020); measured output +11.9% to +18.1% above set power
- [[Epic 10 TM]] — 940 nm (Kim et al. 2020); measured output −23.7% to −27.3% below set power
- [[Saeshin Diode Laser]] — 980 nm (Kim et al. 2020); measured output −14.0% to −18.3% below set power

## Devices appearing in biopsy / diagnostic-yield studies

Real or ex vivo excision studies with a pathologist-rendered histologic outcome (diagnostic yield, margin damage, or thermal-damage width tied to a named device).

- [[Raffaello]] — 980 nm (Gambino et al. 2026); 100% diagnostic yield (30/30), epithelium/connective-tissue thermal damage quantified
- [[SOL]] — 808 nm (Romeo et al. 2014); 100% diagnostic yield (17/17, pooled with KTP comparator), per-lesion-type margin damage
- [[Zolar Plus]] — 980 nm (Gundlapalle et al. 2022); real human biopsies, CW vs. PW necrotic-border width, no numeric diagnostic-yield %
- [[Wiser 3]] — 450/808 nm (Pergolini et al. 2025); ex vivo thermal damage only, no diagnosis rendered
- [[Dentek LD 15]] — 810 nm (Goharkhay et al. 1999); ex vivo incision/thermal-damage geometry only, no diagnosis rendered
- [[LITEMEDICS|LITEMEDICS®]] — 980 nm (Azevedo et al. 2016); ex vivo thermal damage/carbonization only, no diagnosis rendered
- [[A.R.C. Laser FOX IV (445 nm)]], [[A.R.C. Laser FOX (810 nm)]], [[A.R.C. Laser FOX (980 nm)]], [[A.R.C. Laser FOX (1064 nm)]], [[A.R.C. Laser WOLF (1470 nm)]] — ex vivo tissue-effect ranking only (Gutiérrez-Corrales et al. 2020), no diagnosis rendered
- [[SIROLaser Blue]] — histologic penetration depth (Romanos et al. 2022), not a diagnostic-yield outcome

## Devices with both measured-output AND histology/diagnostic data

None. No device in this vault currently has both an independent measured-output value and a histologic/diagnostic-yield outcome from the same or cross-referenced source. This is a standing research gap — see `06 Synthesis/` for related contradictions/gaps notes.

- Closest partial case: [[SIROLaser Blue]] has measured-output data (Xue et al. 2022) and tissue-effect data (Romanos et al. 2022), but the two come from different studies and neither reports the other's outcome type, so they cannot be cross-validated against each other for this device.

## All device notes

| Device | Manufacturer | Wavelength | Measured output? | Biopsy/histology outcome? |
| --- | --- | --- | --- | --- |
| [[Quicklase 12W Dual 4]] | Quicklase, UK | 810+980 nm dual | No (set only) | No (temperature-rise study only) |
| [[A.R.C. Laser FOX IV (445 nm)]] | A.R.C. Laser GmbH | 445 nm | No (measured, not published) | Qualitative ranking only |
| [[A.R.C. Laser FOX (810 nm)]] | A.R.C. Laser GmbH | 810 nm | No (measured, not published) | Qualitative ranking only |
| [[A.R.C. Laser FOX (980 nm)]] | A.R.C. Laser GmbH | 980 nm | No (measured, not published) | Qualitative ranking only |
| [[A.R.C. Laser FOX (1064 nm)]] | A.R.C. Laser GmbH | 1064 nm | No (measured, not published) | Qualitative ranking only |
| [[A.R.C. Laser WOLF (1470 nm)]] | A.R.C. Laser GmbH | 1470 nm | No (measured, not published) | Qualitative ranking only |
| [[Dentek LD 15]] | Dentek Austria GMBH | 810 nm | Yes (0.5–4.5 W) | Ex vivo incision geometry, no diagnosis |
| [[Gemini Evo]] | Ultradent Products | 810+980 nm dual | No | Reoperation rate only, no histology |
| [[SIROLaser Blue]] | Dentsply Sirona | 445+970 nm dual | Yes (Xue et al. 2022 only) | Penetration depth (Romanos et al. 2022 only) |
| [[Picasso]] | AMD Lasers | 810 nm | Yes | No |
| [[Raffaello]] | DMT, Lissone | 980 nm | No | Yes — 100% diagnostic yield |
| [[Wiser 3]] | Doctor Smile | 450+808 nm dual | No | Ex vivo thermal damage, no diagnosis |
| [[Zolar Plus]] | UNKNOWN | 980 nm | No | Yes, but no numeric diagnostic yield % |
| [[K2 Mobile]] | Hulaser | 980 nm | Yes | No (titanium disc study) |
| [[Epic 10 TM]] | Biolase | 940 nm | Yes | No (titanium disc study) |
| [[Saeshin Diode Laser]] | Saeshin | 980 nm | Yes | No (titanium disc study) |
| [[SOL]] | DenMat Italia | 808 nm | No | Yes — 100% diagnostic yield (pooled) |
| [[LITEMEDICS\|LITEMEDICS®]] | LITEMEDICS® (unstated location) | 980 nm | No | Ex vivo thermal damage, no diagnosis |

## Excluded devices (manufacturer/type known, exact model not reported — no note created)

- 808 nm diode laser, DMT, Milan, Italy — [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]] (largest biopsy sample in this vault, n=608; manufacturer named, no model name given)
- 810 nm diode laser, Biolase, Irvine, CA — [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]] ("specific model number not given")
- Diode laser, Fotona, Ljubljana, Slovenia — [[07 Data/Li et al 2022 - Diode vs Er-YAG vs Cold Scalpel Mice Oral Mucosa Data]]
- Double-wavelength system, 940 nm diode, Biolase Inc. — [[07 Data/Fahlstedt et al 2021 - Laser Operating Parameters]] (model explicitly UNKNOWN; not merged with Epic 10 TM)
- Blue diode laser, Eltech K-Laser srl, Treviso, Italy — [[07 Data/Palaia et al 2021 - 445 nm Diode Laser In Vivo Biopsy Thermal Effect Data]] (company named, no product model given)
- 38 semiconductor diode dental laser units, 20 device types — [[07 Data/Parker et al 2022 - Delivery Power Losses and Operating Parameters]] (survey of unnamed devices)
- Diode laser, manufacturer not named — [[07 Data/Capodiferro et al 2009 - Diode Laser Chondroid Lipoma Case Report Data]], [[07 Data/Capodiferro et al 2008 - Oral Laser Surgical Pathology Abstract-Level Data]], [[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)]] (abstract-level only)
- DILAS laser-diode module (equivalent-load bench test, not a clinical device) — [[07 Data/Ma and Zhang 2024 - Laser Diode Driver]]
- Multimode blue diode laser, prism-etalon feedback (physics paper, not a named commercial device) — [[07 Data/Muller 2024 - Prism-Etalon Diode Laser]]
- Non-diode comparator lasers used in the same papers as vault diode devices (out of this vault's diode-laser scope, no note created): KTP SmartLite (DEKA) and Er,Cr:YSGG Waterlase iPlus (Biolase) — [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data]], [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]]; KTP NuvoLas (A.R.C. Laser GmbH) — [[07 Data/Gutierrez-Corrales et al 2020 - Diode Wavelength Operating Parameters]]; CO2 lasers (Medical Optics Inc., Sharplan Lasers, Luxar Corp.) — [[07 Data/Wilder-Smith et al 1995 - CO2 Laser Incision and Thermal Damage Data]]
- Endovenous laser ablation console/fiber (not named in-text; "Elli 810/980" and "Venacure 1470Nm" cited only as reference-list operating manuals, not the study device) — [[07 Data/Davies et al 2020 - EVLA Fiber Tip Power Output and Degradation]]
- 24 photobiomodulation devices (Ibramed Laserpulse, Ibramed Antares, HTM Fluence, DMC Therapy XT) — [[07 Data/Girasol et al 2022 - Photobiomodulation Device Power and Beam Accuracy]]; exact models are named, but this vault's own classification of this source marks it non-dental, supporting/background evidence only (physical-therapy PBM devices, not dental surgical diode lasers), so no device note was created — flag if this scope decision should be revisited.

## สรุปภาษาไทย

- ดัชนีนี้รวบรวมอุปกรณ์เลเซอร์ไดโอดที่มีการรายงานรุ่นที่ชัดเจนในแหล่งข้อมูลที่ผ่านการประมวลผลแล้วในคลังนี้ 18 รายการ
- ไม่มีอุปกรณ์ใดเลยที่มีทั้งข้อมูลกำลังขาออกที่วัดได้จริงและข้อมูลผลชิ้นเนื้อ/การวินิจฉัยจากแหล่งข้อมูลเดียวกัน — นี่คือช่องว่างงานวิจัยที่สำคัญของคลังนี้
- อุปกรณ์ที่ทราบเพียงชื่อผู้ผลิตแต่ไม่ทราบรุ่นที่แน่นอน (เช่น DMT ของ Angiero et al. 608 ราย) ไม่ได้สร้างโน้ตแยก ตามกฎ "ห้ามอนุมานรุ่นอุปกรณ์"
