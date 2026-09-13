---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: false
human_tissue: false
diode_laser: true
wavelength_nm: null
set_power_w: 3
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: true
speed_mm_s: 1
speed_control: unknown
cw_pw: "PW"
fiber_diameter_um: 300
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: "qualitative (incision less regular than Er:YAG; more carbonization and deeper apoptotic damage than Er:YAG)"
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: SUPPORTING dental evidence.** Diode-specific and oral-mucosa-specific, but an animal (mouse) wound-excision model, not a diagnostic biopsy — no lesion is present, no specimen is submitted for pathologist diagnosis, and no diagnostic yield is assessed. Contributes a genuine numeric diode tip-movement speed (a first for this vault's *core-diode* literature, alongside the already-vault Goharkhay et al. 1999 value from a different device/species) and a qualitative carbonization finding.

## Source

- Citation: Li H, Liu Y, Li X, Du J, Guo L, Liu Y. "A histological evaluation of the mice oral mucosal tissue wounds excised with diode laser, Er:YAG laser, and cold scalpel." *Lasers Med Sci.* 2022;37(6):2707-2715. DOI: [10.1007/s10103-022-03544-w](https://doi.org/10.1007/s10103-022-03544-w)
- Literature note: [[02 Literature/10.1007/s10103-022-03544-w]]
- Source type: Controlled animal (mouse) experimental study, three parallel groups (diode, Er:YAG, cold scalpel), n=12 animals/group
- Source locator: Full text (Abstract; Materials and Methods; Results; Figs. 1–8; Discussion), retrieved from the attached PDF via the local Zotero library.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Diode laser (Fotona, Ljubljana, Slovenia); comparator Er:YAG laser (Fotona); comparator cold scalpel (15c blade) | — | Materials and Methods | FACT |
| Manufacturer | Fotona (diode and Er:YAG) | — | Materials and Methods | FACT |
| Wavelength | UNKNOWN — not stated for this specific device in the Methods; the Introduction states diode lasers used in periodontal surgery generally span 800–980 nm, but this is a general literature statement, not this study's own device specification | — | Introduction (general statement only) | UNKNOWN (device-specific value) |
| Set power | 3.0 | W | Materials and Methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; 3.0 W is a console/panel value | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Pulsed — 200 Hz, duty setting reported as "1/2" (device-specific notation, not independently decoded by this vault) | — | Materials and Methods | FACT (that it is pulsed, not CW) / UNKNOWN (exact duty-cycle percentage) |
| Pulse duration | UNKNOWN (not separately given; only frequency and the "1/2" notation are reported) | — | — | UNKNOWN |
| Frequency | 200 | Hz | Materials and Methods | FACT |
| Duty cycle | UNKNOWN — "1/2" is reported verbatim but not defined by the source as a percentage | — | Materials and Methods | FACT (verbatim notation) / UNKNOWN (interpreted value) |
| Fiber diameter | 300 | μm | Materials and Methods | FACT |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact / non-contact mode | UNKNOWN — not explicitly stated | — | — | UNKNOWN |
| Incision speed (tip movement speed) | 1 | mm/s | Materials and Methods ("The tip movement speed in both Er:YAG and diode groups was 1 mm/s") | FACT |
| Wound length | 2 | mm | Materials and Methods | FACT |
| Wound establishment (irradiation) time | 2 | s | Materials and Methods | FACT — consistent with the stated 1 mm/s speed over a 2 mm wound, but this vault does not use this consistency to derive speed independently; the source states the speed value directly |
| Excision protocol | Coronal incision in the mouse tongue dorsum, standardized wound model (not a lesion excision) | — | Materials and Methods | FACT |
| Specimen margin | N/A — not an excised diagnostic specimen; wound evaluated in situ by serial histologic sectioning of the tongue | — | — | N/A |
| Tissue model | In vivo mouse (C57BL/6J, male), tongue dorsum mucosa; comparator groups Er:YAG (400 μm, 1.2 W, 60 mJ, 20 Hz, water 2/air 2) and cold scalpel (15c blade, one-time cut per wound, new blade each time) | — | Materials and Methods | FACT |
| Measurement method | H&E histology (5 μm sections) at 40× for wound width/depth and inflammatory infiltrate, scored by a pathologist blinded to instrument type; immunofluorescence (Ly-6G, CD11b, CD86) for neutrophil/macrophage chemotaxis; TUNEL staining for local apoptosis | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN — no laser power-meter calibration protocol reported | — | — | UNKNOWN |
| Wound depth vs. cold scalpel | Diode and Er:YAG wounds significantly shallower than cold-scalpel wounds (P<0.01); exact μm/mm values shown only in bar-graph form (Fig. 1A), not tabulated as numbers in text — not extracted here to avoid reading precise figures off a bar chart | — | Results; Fig. 1A | FACT (direction, significance) / UNKNOWN (exact magnitude) |
| Wound width vs. cold scalpel | Diode and Er:YAG wounds significantly wider than cold-scalpel wounds (P<0.01); exact values graph-only, not extracted | — | Results; Fig. 1B | FACT (direction, significance) / UNKNOWN (exact magnitude) |
| Incision regularity | Er:YAG produced the most regular incision, followed by diode, then cold scalpel (qualitative histologic assessment, not scored numerically) | — | Results; Fig. 2A | FACT (qualitative ranking only) |
| Carbonization | Diode laser caused an "obvious carbonization layer," described as more tissue damage than Er:YAG, visible on both gross and histologic examination; not scored on a numeric scale | — | Results; Fig. 2A, B | FACT (qualitative finding) |
| Thermal/apoptotic damage depth (TUNEL) | Diode group showed more apoptotic cells, located relatively deeper, than Er:YAG (superficial, fewer); cold scalpel showed minimal/no TUNEL-positive cells | — | Results; Fig. 3 | FACT |
| Wound healing time | Diode healing speed significantly slower than both Er:YAG and cold scalpel (P<0.05); cold scalpel healing rate faster than Er:YAG but not significantly (P>0.05); exact day values graph-only (Fig. 1C), not extracted numerically here | — | Results; Fig. 1C | FACT (direction, significance) / UNKNOWN (exact magnitude) |
| Inflammatory cell infiltration | Diode group showed the largest number of local inflammatory cells on post-op day 1, followed by Er:YAG then cold scalpel; both lasers showed more infiltration than cold scalpel throughout the 3-day observation | — | Results; Figs. 4–6 | FACT |
| Neutrophil/macrophage chemotaxis | Both lasers increased Ly-6G+ neutrophil and CD11b+CD86+ macrophage chemotaxis versus cold scalpel; diode produced the most pronounced promotion of both | — | Results; Figs. 7–8 | FACT |
| Coagulation zone | Not scored or measured in this study's own data; the Discussion cites another paper's finding that "diode laser showed good coagulation capacity" as background, not as this study's own measured result | — | Discussion | FACT (that it is a cited claim, not a finding of this study) |
| Diagnostic yield | N/A — no lesion, no diagnosis rendered; this is a standardized wound-healing model, not a diagnostic-biopsy pathway | — | — | N/A |
| Sample | n=12 mice per group (diode, Er:YAG, cold scalpel), 36 total; histologic sections taken daily (n=3/group/day) through day 3 | — | Materials and Methods | FACT |

## Notes

- FACT: This is the first source in this vault's *core-diode* biopsy-adjacent literature (as opposed to the previously-noted Goharkhay et al. 1999, a different device and species) to report an explicit numeric tip-movement/incision speed for a diode laser: 1 mm/s. This speed was held fixed across both laser arms (diode and Er:YAG), not varied as an independent variable, so it cannot answer whether incision speed itself affects thermal damage or specimen quality — it only establishes that a second, independent numeric incision-speed value now exists in this vault's wider diode literature.
- FACT: The 1 mm/s value cannot be compared to or reconciled with Goharkhay et al. 1999's 10 mm/s value — different device (Fotona vs. Dentek LD 15), different species (mouse vs. pig), different tissue context (in vivo tongue dorsum vs. ex vivo mandible mucosa), and different wavelength (UNKNOWN here vs. 810 nm there). Per vault rule, this is preserved as two independent, non-transferable data points, not averaged or used to estimate a "typical" speed.
- FACT: The diode laser produced more carbonization and deeper/more apoptotic thermal damage than Er:YAG at its own tested settings (3.0 W pulsed vs. 1.2 W/60 mJ/20 Hz) — consistent in direction with this vault's existing [[04 Evidence/Thermal Artifact]] finding that Al-Ani et al. measured a higher mean temperature rise with a 2.5 W diode setting than a comparator Er,Cr:YSGG setting. This is a second independent source, using an entirely different laser-type comparator (Er:YAG rather than Er,Cr:YSGG) and a different species, corroborating that this vault's diode sources tend to show more thermal effect than non-diode comparators tested alongside them.
- FACT: Diode laser incisions were regular, but less regular than Er:YAG — this is a new, if qualitative, incision-regularity ranking not previously present in this vault's diode literature (existing sources report thermal-damage width/carbonization but not a laser-vs-laser incision-regularity ranking).
- INTERPRETATION: The combination of more carbonization, deeper apoptosis, and slower healing in the diode group, all at once in the same model, is internally consistent — it supports (without independently proving beyond this one animal model) the general expectation that greater acute thermal/carbonization injury is associated with delayed healing. This is not a specimen-diagnostic-quality finding, so it cannot be used to update [[04 Evidence/Biopsy Specimen Quality]] or [[04 Evidence/Surgical Margins]].
- HYPOTHESIS: UNKNOWN — no formal hypothesis beyond the study's own comparative aim.
- Limitations (source-stated and vault-noted): mouse tongue dorsum wound-healing model, not a human or ex vivo diagnostic-biopsy pathway; no lesion excised and no diagnosis rendered; set power only, no independent power-meter verification; wavelength of the diode device used is not stated; exact numeric wound-morphology and healing-time values are presented only as bar graphs in the source, not as text/table numbers, so several FACTs above are qualitative (direction + significance) rather than quantitative.
- Classification for this vault: SUPPORTING dental evidence — diode-specific, oral-mucosa-specific, but a non-diagnostic animal wound-excision model. Relevant to [[04 Evidence/Thermal Artifact]] and [[03 Concepts/Glossary/Incision Speed]]; not relevant to [[04 Evidence/Biopsy Specimen Quality]] or [[04 Evidence/Surgical Margins]] (no excised diagnostic specimen).

## Related notes

- Evidence: [[04 Evidence/Thermal Artifact]]
- Concepts: [[03 Concepts/Glossary/Incision Speed]], [[03 Concepts/Glossary/Carbonization]], [[03 Concepts/Glossary/Thermal Damage]]
- Project: [[01 Projects/Diode Laser Biopsy]]
