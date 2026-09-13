---
classification: "BACKGROUND"
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: false
wavelength_nm: null
set_power_w: null
measured_power: true
measured_power_value_reported: true
measured_power_w: [1, 4, 12]
power_meter: "PRJ-M (Gentec)"
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: "non-contact"
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

**Vault classification: BACKGROUND methodological evidence.** This source uses three CO2 lasers, not a diode laser — it does not add diode-specific evidence to any core biopsy claim. It is retained because it independently measures delivered power with a calibrated power meter and pairs that measurement with histologic thermal-damage/incision data in oral mucosa, which is the measurement design this vault's diode literature currently lacks. Its power-meter methodology cannot be transferred to any diode source in this vault.

## Source

- Citation: Wilder-Smith P, Arrastia AM, Liaw LH, Berns M. "Incision properties and thermal effects of three CO2 lasers in soft tissue." *Oral Surg Oral Med Oral Pathol Oral Radiol Endod.* 1995;79(6):685-691. DOI: [10.1016/S1079-2104(05)80300-2](https://doi.org/10.1016/S1079-2104(05)80300-2)
- Literature note: [[02 Literature/10.1016/S1079-2104(05)80300-2]]
- Source type: Controlled ex vivo laboratory study, three parallel laser devices, standardized incisions
- Source locator: Full text (Abstract; Material and Methods; Results; Figs. 1–9; Discussion), retrieved from the attached PDF via the local Zotero library.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Three CO2 lasers: Laser A (Medical Optics Inc., Carlsbad, Calif.), Laser B (Sharplan Lasers, Inc., Allendale, N.J.), Laser C (Luxar Corp., Bothell, Wash.) — **not diode lasers** | — | Materials and Methods | FACT |
| Manufacturer | Medical Optics Inc. (A); Sharplan Lasers, Inc. (B); Luxar Corp. (C) | — | Materials and Methods | FACT |
| Wavelength | Laser A: 9.3 μm; Lasers B and C: 10.6 μm | — | Materials and Methods | FACT |
| Set power (console/panel) | UNKNOWN — the source does not separately report a console dial value distinct from the power-meter-confirmed value below | — | — | UNKNOWN |
| Measured output power | 1, 4, and 12 | W ("actual power levels") | Materials and Methods | FACT — measured directly before each incision with a PRJ-M power meter (Gentec); explicitly described as "actual power levels emitted," distinct from a nominal/panel value |
| Average power | Same as measured output power above (CW mode; no separate average/peak distinction made) | W | Materials and Methods | FACT |
| Peak power | N/A (CW mode) | — | — | N/A |
| Operating mode | Continuous wave (CW) — "All lasers were set to the continuous wave mode" | — | Materials and Methods | FACT |
| Pulse duration | N/A (CW) | — | — | N/A |
| Frequency | N/A (CW) | — | — | N/A |
| Duty cycle | N/A (CW) | — | — | N/A |
| Beam delivery / spot size | Laser A: coherent hollow waveguide, 250 μm spot; Laser B: articulated arm, 220 μm spot; Laser C: incoherent hollow fiber waveguide, 300 μm spot | — | Materials and Methods | FACT |
| Fiber diameter | N/A in the diode-fiber sense — CO2 delivery via hollow waveguide or articulated arm, not a silica fiber; spot sizes given above | — | — | N/A |
| Tip type / tip initiation status | N/A — not applicable to CO2 waveguide/articulated-arm delivery | — | — | N/A |
| Contact / non-contact mode | Non-contact (focusing handpiece, standardized distance via a jig) | — | Materials and Methods | FACT |
| Incision speed | UNKNOWN — not reported and not calculated by the authors. The source reports a fixed irradiation duration (4 seconds per incision, timed with a stopwatch) and a fixed incision length (3 cm), but does not itself state or compute a speed value; per this vault's rule, speed is not inferred from duration and length here. | — | — | UNKNOWN |
| Exposure duration | 4 | s (per incision, timed with a stopwatch) | Materials and Methods | FACT |
| Incision length (standardized) | 3 | cm | Materials and Methods | FACT |
| Excision protocol | Standardized 3 cm incisions in pig mandible oral mucosa, parallel to the mandibular border, 5 mm below the gingival margin; not a lesion excision | — | Materials and Methods | FACT |
| Specimen margin | Incisions dissected with a margin exceeding 5 mm; not a diagnostic biopsy specimen | mm | Materials and Methods | FACT |
| Tissue model | Ex vivo pig mandible oral mucosa (9 fresh mandibles, used within 6 hours of death); 30 total incisions, minimum 3 per laser/power combination | — | Materials and Methods | FACT |
| Measurement method | Thermocouple (copper-constantan, 0.25 mm diameter, 7 ms response time) placed ~1 mm + half spot-size lateral to the incision, recording temperature at 3/6/10/30 s of irradiation; histologic sections (6 μm, serius red stain) measured by a single blinded investigator for incision depth/width and vertical/horizontal tissue-damage extent (Fig. 1 depicts measurement sites) | — | Materials and Methods | FACT |
| Calibration method | Beam characteristics for each laser calibrated by one laser engineer to manufacturer specifications immediately before the study; spot sizes verified with photographic paper before each irradiation; power confirmed with a PRJ-M (Gentec) power meter directly before each incision | — | Materials and Methods | FACT |
| Thermal events during irradiation | No significant temperature rise for Lasers A or B at any power/time point (p<0.05, i.e., not significant); Laser C showed significant temperature increases at 1 W (after 6, 10, 30 s), 4 W (after 6, 10, 30 s), and 12 W (after 3, 6, 10, 30 s); at 12 W, Laser C reached an almost immediate rise of up to 20°C | °C | Results; Figs. 2–5 | FACT |
| Incision depth/width | For Lasers A and B, depth/width did not differ significantly at 4 and 12 W; at 1 W, Laser B produced no clear incision at all. Laser C produced significantly smaller incision depth and significantly greater incision width than A/B at all comparable power settings (p<0.0001). Exact μm values are presented only in bar-graph form (Figs. 6–7), not tabulated as text numbers, and are not extracted numerically here. | — | Results; Figs. 6–7 | FACT (direction, significance) / UNKNOWN (exact magnitude) |
| Vertical/horizontal tissue damage | Lasers A and B did not differ significantly at 4 and 12 W; both produced significantly greater tissue-damage zones than Laser C (p<0.0001) at matched power. A trend of greater lateral tissue damage at higher power was observed within the constant-wave mode. Exact μm values are graph-only (Figs. 8–9), not extracted numerically here. | — | Results; Discussion; Figs. 8–9 | FACT (direction, significance) / UNKNOWN (exact magnitude) |
| Coagulation zone | Discussed conceptually (a coagulated tissue layer along laser incision walls, distinct from the scalpel-cut comparison), not scored as its own numeric variable in this study | — | Introduction; Discussion | FACT (conceptual discussion only) |
| Carbonization | Discussed conceptually as a possible outcome of marginal thermal interaction (alongside protein denaturation and water evaporation), not scored or measured as its own variable in this study's results | — | Introduction | FACT (conceptual discussion only) |
| Diagnostic yield | N/A — no lesion excised, no diagnosis rendered; this is a mechanistic incision/thermal-effect study, not a diagnostic-biopsy pathway | — | — | N/A |
| Sample | 30 incisions total across 9 pig mandibles; minimum 3 incisions per laser × power combination; 81 wax blocks, 10 slides per incision site (30 slides per laser/power parameter) | — | Materials and Methods | FACT |

## Notes

- FACT: This is the only source identified by this project's literature search that pairs a genuinely power-meter-measured (not console/set) laser power value with both thermocouple-measured thermal events and histologic incision/damage measurements, in oral mucosa. This is exactly the measurement design that [[04 Evidence/Power Output and Tissue Effect]] identifies as absent from this vault's dental-diode literature — but this source cannot fill that gap, because it uses CO2 lasers, not a diode laser, and its devices (Medical Optics Inc., Sharplan, Luxar CO2 systems) do not overlap with any device in this vault's diode-specific evidence base.
- FACT: The study's own stated conclusion is that thermal and histologic results were "related to parameters and beam characteristics rather than wavelength" — i.e., at matched actual power, differences in incision depth/width and thermal damage between lasers B and C (same 10.6 μm wavelength) were attributed to differences in beam coherence, spot size, and delivery system (articulated arm vs. incoherent hollow waveguide), not wavelength itself.
- INTERPRETATION: This finding — that device/beam characteristics can matter as much as or more than the power value itself — is directionally consistent with this vault's existing diode-literature pattern in which power level alone does not reliably predict thermal-damage-zone width (see [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]] and [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]], both finding no significant power-dependence of thermal-damage width). This is a cross-laser-type methodological parallel, not diode-specific evidence, and is not used to alter any diode-specific claim in [[04 Evidence/Thermal Artifact]].
- FACT: Per this vault's explicit instruction, incision speed is not inferred from the reported 3 cm incision length and 4 s exposure duration, because the authors themselves do not state or compute a speed value from these figures.
- Limitations (source-stated and vault-noted): ex vivo porcine tissue, not human; CO2 laser only, no diode comparator; nonpulsed/CW settings only, by the authors' own design choice, explicitly stated as a simplification for this first study in a planned series; thermocouple placement precision is noted by the authors themselves as imperfect; exact histologic and thermal magnitude values are presented graphically, not as text/table numbers.
- Classification for this vault: BACKGROUND methodological evidence — non-diode, but relevant as a measurement-design precedent (independently measured power + thermal + histologic outcome, in oral mucosa) for what a closing study in [[04 Evidence/Power Output and Tissue Effect]] would need to look like. Not cited as diode-specific evidence in any CORE biopsy evidence note.
- METADATA CONVENTION: `diode_laser: false` — this source uses three CO2 lasers, explicitly not diode. `measured_power: true` and `measured_power_value_reported: true` (`measured_power_w: [1, 4, 12]`, PRJ-M/Gentec meter, actual power confirmed before every incision) are genuinely and cleanly reported, but this is CO2 data, not diode-laser prior art. This note previously appeared in [[06 Synthesis/Study Dashboard]] Table B despite being non-diode, because the original queries filtered on `measured_power`/`incision_speed_reported`/`histology` only. As of schema v1.1, Tables B and C add `diode_laser = true AND classification != "BACKGROUND"`, so this row no longer appears in either table — it remains correctly tagged here (measured power was genuinely, independently verified) but is excluded from the diode-technical-precedent tables by design, not by omission.

## Related notes

- Evidence: [[04 Evidence/Power Output and Tissue Effect]], [[04 Evidence/Thermal Artifact]]
- Project: [[01 Projects/Diode Laser Biopsy]]
