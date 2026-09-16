---
classification: "SUPPORTING TECHNICAL"
oral_tissue: false
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 445
set_power_w: [2, 8]
measured_power: true
measured_power_value_reported: true
measured_power_w: [12.7, 34.5]
power_meter: "LabMax Top + PM10 power sensor (Coherent, Santa Clara, CA, USA)"
measurement_location: "distal end of the optical fiber"
incision_speed_reported: true
speed_mm_s: 3
speed_control: "mechanized"
cw_pw: "CW+PW"
fiber_diameter_um: 375
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
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

- Literature note: [[02 Literature/10.3390/app15031041|Liu et al. 2025]]
- Source link: https://doi.org/10.3390/app15031041
- Source locator: Full text (PDF, `pdftotext`, cross-checked against prose where table/figure regions extracted with column-reflow artifacts) — Abstract; §2.1–2.7 (Materials and Methods); §3.1–3.4 (Results); §4 (Discussion); §5 (Conclusions); Tables 1–2.

## Important tissue-type flag

**This is NOT an oral soft-tissue study.** §2.4 states explicitly: "Regarding the utilization and evaluation of this laser system in the field of otorhinolaryngology (ear, nose and throat (ENT) application), ear samples from freshly slaughtered pigs... were used." The tissue is porcine **ear** (skin/cartilage region), chosen for an ENT application context. Do not cite this note as oral-tissue evidence without this caveat.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Custom diode laser stack built from NDB7Y75 laser diode emitters (Nichia Corporation, Anan, Japan), driver electronics/optics/fiber coupling custom-made by A.R.C. Laser GmbH (Nuremberg, Germany) | — | §2.1 | FACT |
| Manufacturer | A.R.C. Laser GmbH, Nuremberg, Germany (system integration); Nichia Corporation (diode emitters) | — | §2.1 | FACT |
| Wavelength | 445 (individual emitters center at 455 nm; system/product wavelength stated throughout as 445) | nm | §2.1; Abstract | FACT |
| Set power (average, main cutting series) | 2.0–8.0, in 0.5 W increments (52 cuts); a second series at fixed pulse durations/duty-cycles of 25% and 15% ran 2 W up to the maximum achievable power in 1 W increments (24 more cuts) | W | §2.4; Table 2 | FACT |
| Measured output power (independent, reported value) | Maximum CW output measured: 12.7 W (vs. 13.5 W manufacturer/system nominal rating, ~0.8 W / ~6% below spec, cited as within IEC 60601-2-22's ±20% tolerance). Maximum peak power for 5 µs/10 µs pulses at 5–10% duty-cycle: up to 34.5 W | W | §3.1; Figures 6–8 | FACT |
| Average power | Same as set power for the tissue-cutting series (2–8 W); characterized independently across the full CW/pulsed power-vs-set-point-voltage curve (§3.1) | W | §2.4; §3.1 | FACT |
| Peak power | Up to 34.5 W (5 µs and 10 µs pulse durations, 5% and 10% duty-cycle) | W | §3.1; Figure 7 | FACT |
| Operating mode | CW and pulsed (duty-cycles 1% up to 40%, partially up to 90%; pulse durations from 1 µs to 900 ms per Table 1); tissue-cutting series specifically used CW plus 10 µs/100 µs/1 ms pulses at 50%, 25%, and 15% duty-cycle | — | §2.2–2.3; Table 1; §2.4 | FACT |
| Pulse duration | 1 µs to 900 ms achievable (Table 1, full characterization); tissue-cutting series used 10 µs, 100 µs, 1 ms, and CW | — | Table 1; §2.4 | FACT |
| Frequency | Pulse repetition rates from ~1 Hz to 300 kHz achievable depending on duty-cycle/pulse-duration combination (Table 1); pulse-train mode additionally tested at 2, 5, and 10 Hz train repetition | Hz | Table 1; §2.3 | FACT |
| Duty cycle | 1–90% achievable (Table 1); tissue-cutting series specifically used 50%, 25%, and 15% | % | Table 1; §2.4 | FACT |
| Fiber diameter | 375 core / 405 cladding | µm | §2.5 | FACT |
| Tip type | Bare step-index fiber (heracle GmbH, Jena, Germany), NA = 0.22; no initiation status stated | — | §2.2, §2.5 | FACT (fiber type) / UNKNOWN (initiation status not mentioned) |
| Tip initiation status | UNKNOWN — not described as initiated or non-initiated anywhere in the Methods | — | — | UNKNOWN |
| Contact mode | Contact mode, fiber distance to sample surface visually controlled in real time via an Elio-Microscope camera system | — | §2.5 | FACT |
| Exposure duration | Not given as a fixed time value; incisions are linear cuts of unspecified stated length at 3 mm/s cut speed (governs total exposure time per cut, not separately tabulated) | — | §2.5 | UNKNOWN (as a standalone value) |
| Measurement method | Output power measured with LabMax Top energy/power meter + PM10 sensor (Coherent); for high pulse-repetition-rate settings, power recorded over a 10 s window and averaged. Emitted power at the distal fiber end was checked against a calibration value before cutting; a new fiber-tip configuration was required if deviation exceeded 10% | — | §2.2; §2.5 | FACT |
| Calibration method | LabMax Top + PM10 used as the calibration/verification instrument; fiber-tip re-configuration triggered at >10% deviation from calibration value; no separate meter-calibration certificate/traceability standard reported | — | §2.5 | FACT (verification protocol) / UNKNOWN (meter's own calibration traceability) |
| Power loss / deviation | Measured max CW output (12.7 W) vs. system nominal rating (13.5 W): ~0.8 W (~6%) below spec — a device-rating-vs-measured-output gap, not a set-vs-measured comparison for a specific clinical parameter/preset | W | §3.1 | FACT |
| Incision / cutting speed | 3 mm/s, fixed and identical across every one of the 380 cuts; motion generated by a computer-controlled 3D micropositioner (VT-80, Micos, Eschbach, Germany) — the same device family used by [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] / [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] | mm/s | §2.5 | FACT — **speed is a fixed experimental control, never varied; this is not a speed-effect experiment** |
| Sample / tissue model | Porcine **ear** tissue (German landrace, 8 weeks old, 30–40 kg), ~1.5 × 2 cm blocks, full ear thickness, used within 2 h postmortem; NOT oral tissue | — | §2.4 | FACT |
| Measurement method (thermal damage) | Histological preparation and thermal-damage-zone evaluation procedure as previously described by the same group in Hanke et al. 2021 (ref. [20]); depth of cut also evaluated (newly, for this paper) | — | §2.6 | FACT |
| Cutting depth | Increases approximately linearly with average power; up to 1 mm depth achieved with 100 µs pulses (various duty-cycles) and in CW mode; no significant difference in cut depth found between different pulse-duration/duty-cycle regimes and CW at the sample sizes tested | mm | §3.4; Figure 12; Table 3 | FACT |
| Thermal damage zone width | 200–350 µm across all tested settings; a non-statistically-confirmed trend toward a steeper (deeper) increase for CW vs. pulsed modes at average power > 4 W, flagged by the authors as needing further investigation given limited sample size | µm | Abstract; §3.4; Figure 13 | FACT |
| Diagnostic biopsy outcome | Not applicable — non-lesional ear-tissue blocks, no diagnosis rendered, purely a technical cutting/thermal characterization | — | — | N/A (by design) |
| Carbonization | Not scored or discussed as a distinct outcome | — | — | UNKNOWN |
| Coagulation zone | Not scored or discussed as a distinct outcome (only "thermal damage zone" width, from the cited Hanke 2021 histological protocol) | — | — | UNKNOWN |
| Sample size | 380 cuts total (52 in the main power series + 24 in the fixed-duty-cycle series, ×5 repeats each — arithmetic in the source's own text) | — | §2.4 | FACT |

## Notes

- FACT: This paper shares its power-measurement instrument (LabMax Top + PM10, Coherent) and its histological thermal-damage-zone evaluation protocol directly with this vault's existing direct prior art, [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]] (cited in this paper as reference [20]) and [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]] — same senior author (J. Meister), same 3D micropositioner family (VT-80, Micos). This paper extends that lineage's power/pulse-duration characterization to the 445 nm wavelength and the microsecond pulse regime, but on a different tissue model.
- FACT: **The tissue is porcine ear, not oral tissue** — chosen explicitly for an ENT/otorhinolaryngology application context (§2.4). This is a deliberate scope departure from Hanke/Strakas's oral (gingival) tissue model and must not be conflated with it when this note is cited.
- FACT: Cut speed (3 mm/s) is fixed and mechanized across every single condition in this study. Per user instruction, this is recorded as `incision_speed_reported: true` / `speed_control: mechanized` (a numeric, mechanized speed value **is** reported), but this must not be read as a speed-effect experiment — speed is a standardized control variable, not an independent variable under test. No comparison across different speeds exists anywhere in this paper.
- FACT: The measured-vs-nominal power gap here (12.7 W measured vs. 13.5 W system rating, ~6% under) is a **device-rating-vs-measured-maximum-output** comparison, not a set-power-vs-measured-output comparison for a specific clinical dial setting or manufacturer preset. It should not be pooled with this vault's existing set-vs-measured evidence (Parker 2022, Xue 2022, Kim 2020, Zegaib 2011, Prado 2022 — see [[04 Evidence/Set Power vs Measured Output]]) without noting this distinction; those studies compare a console-dialed value against its measured delivery, while this paper compares a system's rated maximum capability against its measured maximum capability.
- FACT: No manufacturer-named clinical preset is tested, referenced, or implied anywhere in this paper. All tested power/pulse-duration/duty-cycle combinations are researcher-selected bench parameters for system characterization, not a recalled device preset — do not cite this paper as preset-reliability evidence.
- INTERPRETATION: None drawn beyond the source's own reported cutting-depth/thermal-damage-zone findings.
- HYPOTHESIS: The authors themselves flag, as an open question requiring further investigation (not a confirmed finding), that CW mode might produce a deeper thermal-damage zone than pulsed modes at average power > 4 W, given a limited sample size per condition.
- NEEDS VERIFICATION: Several passages of the source PDF (particularly Figures 6–13 captions and the associated Results prose) extracted with column-reflow/character-duplication artifacts under automated text extraction (both `-layout` and plain modes). Numeric values used in this table were cross-checked against the Abstract, Discussion, and unambiguous prose sentences elsewhere in the document, but a human should visually re-confirm Tables 1–3 and Figures 6, 7, 8, 12, and 13 against the original PDF before using any value not already stated plainly in running text.
- Classification for this vault: SUPPORTING TECHNICAL — a rigorous, independently power-verified diode-laser characterization sharing this vault's Hanke/Strakas measurement lineage, but on non-oral tissue, at a fixed (not varied) cut speed, with no preset or biopsy-oriented outcome. Relevant only as general parameter-characterization/methodological context for [[04 Evidence/Power Output and Tissue Effect]] and [[04 Evidence/Set Power vs Measured Output]] — not as oral-tissue, speed-effect, or preset evidence.

## Related notes

- Literature: [[02 Literature/10.3390/app15031041]]
- Related (shared measurement/protocol lineage): [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data]]
- Evidence: [[04 Evidence/Power Output and Tissue Effect]], [[04 Evidence/Set Power vs Measured Output]]
