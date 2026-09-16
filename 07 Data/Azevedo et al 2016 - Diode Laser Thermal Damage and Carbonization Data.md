---
classification: SUPPORTING TECHNICAL
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 980
set_power_w: 3.5
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
speed_varied: null
cw_pw: PW
fiber_diameter_um: null
tip_initiation: null
contact_mode: contact
histology: true
thermal_damage: true
thermal_damage_measure: "quantified (ETTD: 456.15 μm at 3.5 W PW; 626.82 μm at 3.5 W Boost PW; carbonization scored 0–4)"
margin_quality: null
tissue_architecture: "ordinal histologic tissue-change and incision-regularity scores; not a biopsy-architecture-preservation outcome"
specimen_interpretability: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.4317/jced.52830]]
- Source link: https://doi.org/10.4317/jced.52830
- Source locator: Full text (Material and Methods; Results; Discussion; Tables 1–4), retrieved from the attached PDF via the local Zotero library (zotero-key HNES2DYV). Upgraded from an earlier PMC-API extraction — Table 1, Table 2/4, and the incision-regularity table's diode-specific cell values, previously UNKNOWN, are now available.

## Extraction

Scope note: this study is a six-instrument ex vivo comparison (Er:YAG, CO2, diode, Nd:YAG, electroscalpel, cold scalpel). Only the diode-laser rows are extracted here, per this vault's scope; comparator-instrument values are reported in the source but not extracted into this table.

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Diode laser, LITEMEDICS® | — | Material and Methods | FACT |
| Manufacturer | LITEMEDICS® (city/country not stated) | — | Material and Methods | FACT (name only) |
| Wavelength | 980 | nm | Material and Methods | FACT |
| Set power | 3.5 (two arms: "3.5 W PW" and "3.5 W Boost PW"; "Boost" is not further defined beyond being a distinct pulsed setting at the same nominal 3.5 W label) | W | Material and Methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification; set/console value only | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Pulsed wave (PW), two sub-settings ("PW" and "Boost PW"); no CW arm tested for the diode laser | — | Material and Methods | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN (not stated for the diode; comparators report Hz, e.g., Nd:YAG 40Hz, Er:YAG 10Hz, CO2 50Hz) | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | UNKNOWN (not stated for the diode; only the Nd:YAG arm's fiber diameter, 300 μm, is given) | — | — | UNKNOWN |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | Contact mode ("the diode laser... was used in contact mode for two different applications") | — | Material and Methods | FACT |
| Exposure duration | UNKNOWN (single-pass incision per sample; no fixed time duration reported) | — | — | UNKNOWN |
| Measurement method — thermal damage | Extent of Thermal Tissue Damage (ETTD): greatest distance (μm) from the incision edge to the end of histologically visible thermal damage, measured on 3 μm sections stained with H&E and Masson Trichrome, scored by two blinded pathologists reaching consensus (ZEISS Axio® microscope, Axiovision® software) | — | Material and Methods | FACT |
| Measurement method — carbonization | Macroscopic carbonization scored 0–4 (Cercadillo-Ibarguren et al. criteria: 0 = no color, 1 = brownish surface, 2 = brown in depth, 3 = black surface, 4 = black in depth) | — | Material and Methods | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| ETTD, diode 3.5 W PW | 456.15 (min 234, max 597, SD 108.513) | μm | Table 3 | FACT |
| ETTD, diode 3.5 W Boost PW | 626.82 (min 431, max 1113, SD 220.292) | μm | Table 3 | FACT |
| Carbonization degree, diode 3.5 W PW | 2.50 (n=10, min 1, max 3, SD 0.707) | 0–4 scale | Table 1 | FACT |
| Carbonization degree, diode 3.5 W Boost PW | 1.80 (n=10, min 1, max 3, SD 0.919) | 0–4 scale | Table 1 | FACT |
| Nuclear change score, diode 3.5 W PW | 2.00 (SD 0.000) | 0–4 scale | Table 2 | FACT |
| Nuclear change score, diode 3.5 W Boost PW | 2.20 (SD 0.632) | 0–4 scale | Table 2 | FACT |
| Cytoplasm change score, diode 3.5 W PW | 1.70 (SD 0.483) | 0–4 scale | Table 2 | FACT |
| Cytoplasm change score, diode 3.5 W Boost PW | 1.70 (SD 0.675) | 0–4 scale | Table 2 | FACT |
| Connective (conjunctive) change score, diode 3.5 W PW | 2.00 (SD 0.000) | 0–4 scale | Table 2 | FACT |
| Connective (conjunctive) change score, diode 3.5 W Boost PW | 2.00 (SD 0.000) | 0–4 scale | Table 2 | FACT |
| Incision regularity, diode 3.5 W PW | 2/10 (20%) regular, 8/10 (80%) irregular; mean score 1.0 (SD 0.667) on the 0–4 regularity scale | — | Table 4 | FACT |
| Incision regularity, diode 3.5 W Boost PW | 2/10 (20%) regular, 8/10 (80%) irregular; mean score 0.9 (SD 0.738) | — | Table 4 | FACT |
| ETTD–Carbonization Degree correlation (all instruments pooled) | r = 0.789, p = 0.01 | — | Results | FACT |
| ETTD–Incision Regularity correlation (all instruments pooled) | r = −0.299, p = 0.01 | — | Results | FACT |
| Sample | 10 pig cadaver tongues, 24 h post-slaughter; 120 total incisions across 6 instrument groups; diode n=20 (16.7% of total, 10 per power setting) | — | Material and Methods | FACT |

## Notes

- FACT (correction of an earlier UNKNOWN, now resolved with the real table values): the diode laser's carbonization degree was *lower* at the higher-ETTD "Boost" setting (1.80) than at the standard PW setting (2.50), even though Boost produced *more* thermal-damage extent (626.82 μm vs. 456.15 μm). This is the opposite of what this vault's earlier note speculated (that the higher-ETTD setting would also show higher carbonization) — the pooled cross-instrument correlation (r=0.789) holds across the six instrument types generally, but does not hold as a simple within-device, across-setting pattern for the diode arm specifically. This distinction is preserved here rather than smoothed over.
- FACT: Diode incisions were irregular (score <2) in 80% of cases at both settings, the second-worst regularity in the study after Nd:YAG (0% regular); the best regularity was CO2 at 3.5 W PW (90% regular).
- FACT: Diode nuclear/cytoplasm/connective change scores were similar between the two settings (2.00 vs. 2.20 nuclear; 1.70 vs. 1.70 cytoplasm; 2.00 vs. 2.00 connective), despite the ETTD difference — the tissue-change *scores* were roughly stable while the *linear extent* (ETTD) of damage increased at the Boost setting.
- INTERPRETATION (source's own): the diode's comparatively high ETTD (second-highest of 8 groups, after Nd:YAG) is attributed in the Discussion to its wavelength being poorly absorbed by water but more absorbed by hemoglobin/melanin, giving deeper tissue penetration than CO2 or Er:YAG.
- HYPOTHESIS: UNKNOWN — no formal hypothesis regarding the diode specifically is proposed.
- Classification for this vault: direct dental-diode thermal-damage/carbonization/incision-regularity evidence — ex vivo, not a diagnostic-biopsy outcome (no diagnosis rendered) and not measured-output evidence (set power only, no calibration protocol reported). Relevant to [[04 Evidence/Thermal Artifact]] and [[04 Evidence/Surgical Margins]].
