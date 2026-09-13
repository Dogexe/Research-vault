---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 808
set_power_w: [3, 5]
measured_power: true
measured_power_value_reported: false
measured_power_w: null
power_meter: "Nova II (Ophir)"
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 320
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.1007/s10103-012-1081-8]]
- Source link: https://doi.org/10.1007/s10103-012-1081-8
- Source locator: Full text retrieved from the local Zotero PDF-text cache (`.zotero-ft-cache`, zotero-key QDB676F3g6669922). Merigo E, Clini F, Fornaini C, Oppici A, Paties C, Zangrandi A, Fontana M, Rocca JP, Meleti M, Manfredi M, Cella L, Vescovi P. "Laser-assisted surgery with different wavelengths: a preliminary ex vivo study on thermal increase and histological evaluation." *Lasers Med Sci.* Received 16 Dec 2011, accepted 2 Mar 2012, published online 14 Apr 2012 (© Springer-Verlag London Ltd 2012); print pagination 2013;28(2):497-504. Cited here as "Merigo et al. 2012" per the task's naming, consistent with this vault's existing convention for Angiero et al. (processed as "2011" for a source whose print pagination is 2012).

## Scope note

This is a five-wavelength ex vivo bench comparison (CO2, KTP, Er:YAG, Nd:YAG, and a GaAlAs diode), not a diode-only study and not a diagnostic-biopsy pathway — freshly excised calf tongue was cut with each device/setting and scored for thermal rise and histologic incision quality; no lesion was excised and no pathologist diagnosis was rendered. Only the diode (GaAlAs, 808 nm) arm is extracted in the table below; the other four laser types are described only where needed for context (e.g., the pooled [[03 Concepts/Glossary/Power Loss|power-loss]] figure, which the source states applies to "all the used laser devices"). Two diode settings were tested: 3 W [[03 Concepts/Glossary/Continuous Wave|CW]] and 5 W CW.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | GaAlAs laser (Fotona XD-2) | — | Materials and methods, item 5 | FACT |
| Manufacturer | Fotona, Lubiana [Ljubljana], Slovenia | — | Materials and methods | FACT |
| Wavelength | 808 | nm | Materials and methods | FACT |
| Set power | 3 W and 5 W (two separate CW settings) | W | Materials and methods | FACT |
| Measured output power | UNKNOWN as a diode-isolated value. FACT (pooled, not diode-isolated): every laser device, including this one, was checked with a power meter (Nova II, Ophir, Jerusalem, Israel) before the experimental protocol, and "for all the used laser devices, the loss of power was between 18% and 25%." No per-device breakdown of this range is given, so the diode's own individual loss percentage cannot be isolated from the pooled 18–25% figure. | % | Materials and methods | FACT (pooled across 5 device types) |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) only — no pulsed diode arm in this source | — | Materials and methods | FACT |
| Pulse duration | N/A (CW only) | — | — | N/A |
| Frequency | N/A (CW only) | — | — | N/A |
| Duty cycle | N/A (CW only) | — | — | N/A |
| Power density | 3,750 W/cm² (3 W); 6,250 W/cm² (5 W) | W/cm² | Materials and methods | FACT |
| Fiber diameter | 320 | μm | Materials and methods | FACT |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | Contact | — | Materials and methods | FACT |
| Exposure duration / excision time | 3 W CW: 764 s (the single slowest of all 9 tested wavelength/power combinations across all 5 laser types). 5 W CW: UNKNOWN — not individually stated in the retrieved Results prose (only 8 of the 9 tested settings are itemized in the "increasing times" list; the 5 W diode value is not among them and is not fabricated here). Per vault instruction, incision speed (mm/s) is NOT inferred from this excision-time value. | s | Results — "Excision time" | FACT (3 W only) / UNKNOWN (5 W) |
| Measurement method — thermal | Surface: infrared thermal camera (Thermovision A800, FLIR Systems), 320×240 px, 0.08 °C resolution, ROI mean over 1 cm diameter. Depth: 4× K-type naked-bead thermocouples (TP-01, Lutron), 0.5 mm probe, placed 2–5 mm from incision margins and 2–5 mm deep, read via 4-channel thermometer (TM-946, Lutron, 0.1 °C accuracy). Peak temperature per thermocouple recorded (probes recede from tissue during excision). | — | Materials and methods | FACT |
| Measurement method — histology | H&E, 5 μm sections, low/high-power light microscopy (Nikon Eclipse 80i), two blinded pathologists; incision quality scored 0–4 per examiner per specimen (summed 0–16 across two examiners), per criteria from Vescovi et al. 2010; epithelial/stromal/vascular change widths measured at 40×/100×. Section width 13–25 mm. | — | Materials and methods | FACT |
| Calibration method | Power-meter check (Nova II, Ophir) performed on every device before the start of the experimental protocol — the study's own stated purpose was "to check the real emitted power," yielding the pooled 18–25% loss figure above. | — | Materials and methods | FACT |
| Power loss / deviation | See "Measured output power" row above — 18–25%, pooled across all 5 device types, not diode-isolated. | % | Materials and methods | FACT (pooled) |
| Thermal rise, superficial (3 W CW) | Initial 23.7±0.4 °C → final 45.1±0.9 °C; Δ 21.4±0.6 | °C | Results, Table 1 | FACT |
| Thermal rise, superficial (5 W CW) | Initial 24.1±0.5 °C → final 49.1±1.1 °C; Δ 25±0.6 | °C | Results, Table 1 | FACT |
| Thermal rise, deep (3 W CW) | Initial 21.7375±1.6 °C → final 30.4875±5.6 °C; Δ 8.75±5.2 | °C | Results, Table 2 | FACT |
| Thermal rise, deep (5 W CW) | Initial 24.1625±0.9 °C → final 39.6125±11.2 °C; Δ 15.975±11.1 | °C | Results, Table 2 | FACT |
| Combined (superficial+deep) thermal rise | 3 W CW: approx. 25–35 °C (grouped narratively with CO2 and Nd:YAG); 5 W CW: approx. 40 °C — explicitly stated as the single largest combined temperature increase of all 9 tested settings. Statistical significance for 3 W CO2 vs. 5 W diode specifically: p=0.0027 (deep temperature comparison). | °C | Results — "Temperature elevations" | FACT |
| Incision quality score (0–16, two examiners) | 3 W CW: Examiner 1 = 7, Examiner 2 = 6, total = 13 ("good quality," threshold ≥12). 5 W CW: Examiner 1 = 6, Examiner 2 = 6, total = 12 ("mean quality," threshold 8–12; text places 5 W diode at the boundary, calling it "mean quality"). Scalpel control (Bard-Parker 15c): 8+8=16 (highest of all instruments tested). | score (0–16) | Results, Table 3 | FACT |
| Incision regularity | UNKNOWN as a numeric percentage for diode specifically; source states CO2 and diode were used in continuous mode and this "could determine a more precise cut," attributing good/regular incision quality to CO2 and diode as a pair, not diode alone with an isolated number. | — | Discussion | FACT (qualitative, paired with CO2) |
| Epithelial change width (diode) | UNKNOWN — the source names specific widths only for Nd:YAG (~750 μm) and Er:YAG (~130 μm) and describes CO2 as "intermediate"; diode's own epithelial width is not given a specific number in the retrieved text. | μm | Results — "Histological evaluations" | UNKNOWN |
| Stromal change width (diode) | 5 W CW: 500–600 μm (named specifically, grouped with Nd:YAG as the two greatest). 3 W CW: UNKNOWN as an isolated value — the text states "for all the other wavelengths, mean changes in width were between 100 and 300 μm," which by elimination would include 3 W diode, but the source does not itself name 3 W diode specifically at a stated value; treating 3 W diode as falling in the 100–300 μm band is INTERPRETATION (arithmetic-by-elimination performed in this vault), not a value the source directly attributes to 3 W diode. | μm | Results — "Histological evaluations" | FACT (5 W) / INTERPRETATION (3 W, by elimination) |
| Vascular change width (diode) | UNKNOWN as an isolated diode value — the source names specific widths only for Nd:YAG (~1,000 μm) and 4 W KTP (~600 μm), with "200–400 μm" given as the pooled range for all other wavelengths/settings. | μm | Results — "Histological evaluations" | UNKNOWN (not isolated for diode) |
| Loss of attachment | Observed only in the Nd:YAG-excised sample; not reported for diode. | — | Results — "Histological evaluations" | FACT |
| Carbonization | Not separately scored for diode; "possible carbonization area" appears only in the source's general histologic-criteria definition (applicable to all instruments), not as a diode-specific measured finding. | — | Materials and methods (criteria definition only) | UNKNOWN (as a diode-specific finding) |
| Coagulation zone | Not scored or measured as an isolated variable for any instrument in this source. | — | — | UNKNOWN |
| Diagnostic quality | N/A — no lesion excised, no pathologist diagnosis rendered; this is a bench thermal/histologic-quality comparison, not a diagnostic-biopsy pathway. | — | — | N/A |
| Sample | Freshly extracted calf tongue, used within 6 h of sacrifice; each of 9 wavelength/power combinations (5 laser types, 2 with multiple settings) repeated on 2 samples ×4 tests each = mean/SD of 4 measurements per setting; 2 scalpel-excised controls. | — | Materials and methods | FACT |

## Notes

- FACT: This is the vault's first source reporting a genuinely measured, calibrated-power-meter-verified power-loss figure that includes a diode laser among the devices checked — but the 18–25% loss range is pooled across all 5 device types (CO2, KTP, Er:YAG, Nd:YAG, GaAlAs diode) and is not broken out per device, so it cannot be treated as a diode-isolated measured-power value. It partially, not fully, narrows the vault's standing "no source independently measures delivered diode output" gap (see [[04 Evidence/Power Output and Tissue Effect]]) — the measurement exists, but not at diode-specific resolution.
- FACT: The 3 W diode CW setting was the single slowest excision of all 9 tested wavelength/power combinations (764 s), and the 5 W diode setting produced the single largest combined (superficial+deep) thermal rise (~40 °C) of all 9 combinations. Per vault instruction and per this task's explicit constraint, excision time is recorded as-is and is NOT converted into an incision-speed (mm/s) value, and total thermal rise is not treated as a per-incision-speed-normalized figure.
- FACT: The source's own Discussion cites a different Romanos-authored source (Geminiani, Caton, Romanos 2011, its own reference 17: "Temperature change during non-contact diode laser irradiation of implant surfaces," *Lasers Med Sci*) as support for its statement that "Nd:YAG and diode lasers must be used with special care because of the higher penetration depth and the possible damage to the bone." This is Merigo et al.'s own citation of a separate 2011 Romanos-coauthored paper on implant-surface temperature (not itself processed in this vault pass) — it must not be conflated with [[02 Literature/Diode Laser Soft-Tissue Surgery_ Advancements Aimed at Consistent Cutting, Improved Clinical Outcomes|Romanos 2013 (Compendium)]], the single-author review processed separately in this same batch, nor with [[07 Data/Romanos et al 2022 - Initiated vs Non-Initiated Diode Laser Penetration Depth|Romanos et al. 2022]] already in this vault. All three "Romanos" sources are distinct and are not treated as interchangeable.
- FACT: This source's incision-quality scoring system (0–16, two blind examiners, ≥12 "good," 8–12 "mean," <8 "poor") is a different scale from this vault's other [[03 Concepts/Glossary/Margin Quality|margin/quality]] metrics (μm [[03 Concepts/Glossary/Thermal Damage|thermal-damage]] width, pathologist-graded 1–5 slide quality in Gundlapalle et al.) and is not directly poolable with them.
- Classification for this vault: **SUPPORTING** dental/soft-tissue-diode evidence — a real diode-laser arm (GaAlAs 808 nm, 3/5 W CW, 320 μm fiber, contact mode) with genuinely measured (though pooled, not diode-isolated) power-loss verification and quantified thermal/quality-score data, but ex vivo bovine tongue with no lesion and no diagnosis rendered, so it is not a core diagnostic-biopsy-pathway row. Relevant to [[04 Evidence/Power Output and Tissue Effect]] (partial, pooled power-loss data point), [[04 Evidence/Thermal Artifact]], and [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] (excision-time and thermal-rise data, not incision speed).
- METADATA CONVENTION: `measured_power: true` — the diode arm was independently checked with a calibrated power meter (Nova II, Ophir) before the protocol, per this vault's own prose above; `measured_power_value_reported: false` and `measured_power_w: null` because the resulting 18–25% loss figure is pooled across all 5 device types, not broken out for the diode specifically. This mirrors the Hanke et al. 2021 / Strakas et al. 2023 pattern — independent measurement occurred, but no diode-isolated numerical value is tabulated (see [[99 Templates/Study Metadata Schema]]).
