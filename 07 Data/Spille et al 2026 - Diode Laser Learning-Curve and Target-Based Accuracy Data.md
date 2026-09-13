# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.1007/s10103-026-05011-2]]
- Source link: https://doi.org/10.1007/s10103-026-05011-2
- Source locator: Full text retrieved from the local Zotero PDF-text cache (`.zotero-ft-cache`, zotero-key YDDBBYEKg6669922). Spille D, Lymperopoulos S, Wagner J, Mohr C, Lorich F, Kalsberger T, Wiltfang J, Spille J. "Learning curve and target-based accuracy of diode laser versus scalpel incisions in a porcine skin model: a preclinical feasibility study with undergraduate dental students." *Lasers Med Sci.* 2026;41:204. Received 10 Jul 2026, accepted 24 Aug 2026.

## Scope note

This is a preclinical training/feasibility study, not a diagnostic-biopsy pathway: 22 undergraduate dental students made standardized linear incisions on ex vivo porcine skin at three weekly sessions, comparing four diode-laser settings against a scalpel reference. No lesion was excised and no pathologist diagnosis was rendered; histology was descriptive only (thermal-margin presence/absence), not quantified. The study's primary outcomes are target-based incision-length/depth/width accuracy, operative time, and NASA-TLX workload — extracted below because they directly address this vault's "cutting accuracy/efficiency" question, not because this is a biopsy-diagnostic source.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | SiroLaser Blue | — | Materials and methods — "Laser system" | FACT |
| Manufacturer | Dentsply Sirona, Bensheim, Germany | — | Materials and methods | FACT |
| Wavelength | 445 (blue preset selected; device also offers 660 and 970 nm, not used here) | nm | Materials and methods | FACT |
| Set power | 1 W and 3 W (each crossed with pulsed and continuous mode = 4 laser settings); device total power range 0–3 W | W | Materials and methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; set/console values only | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Pulsed and continuous wave (CW), both tested at both power levels (4-condition factorial: 1 W pulsed, 3 W pulsed, 1 W CW, 3 W CW) | — | Materials and methods | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | 320 | μm | Materials and methods | FACT |
| Fiber/tip type | Sterile single-use flexible quartz-glass fiber (EasyTips), pre-angled to approximately 30° with the manufacturer's bending tool before each session | — | Materials and methods | FACT |
| Tip initiation status | UNKNOWN — pre-angling of the tip is described; initiation (carbonized-tip creation) is not mentioned | — | — | UNKNOWN |
| Contact mode | Contact (methods define incision start as "initial contact between the laser fiber... and the tissue") | — | Materials and methods — "Operative time" | FACT |
| Exposure duration / operative time (mean ± SD, per incision, per method, T1→T3) | Laser 1 W pulsed: 87.9±65.7 s → 65.9±30.6 s → 50.0±26.3 s (p=0.003, T1 vs T3). Laser 3 W pulsed: 39.8±30.7 → 29.7±18.3 → 23.3±11.8 s (p=0.013). Laser 1 W continuous: 41.8±28.7 → 37.8±17.5 → 30.9±14.1 s (p=0.152, ns). Laser 3 W continuous: 22.2±12.2 → 20.9±13.6 → 18.2±9.9 s (p=0.179, ns). Scalpel: 23.5±12.1 → 18.2±8.7 → 17.5±10.5 s (p=0.266, ns). Total per session: 215.3±119.8 → 172.6±74.5 → 139.8±62.5 s (p=0.006). Per vault instruction, incision speed (mm/s) is NOT computed from these operative-time values even though the target incision length (10 mm) is fixed and known. | s | Results, Table 1 | FACT |
| Target incision dimensions | Length 10 mm; depth 2 mm; width minimal (no numeric target) | mm | Materials and methods | FACT |
| Measurement method — dimensions | Micro-CT (70 kVp, 114 μA, 8 W, Cu 0.1 mm filter, 48.5 μm voxel size) on formalin-fixed specimens; custom Python surface-mapping/curve-fitting (Mexican-hat function for laser incisions, Gaussian for scalpel); intra-/inter-rater reliability not formally assessed — source itself describes the method as "feasible and potentially objective rather than formally validated." | — | Materials and methods — "Micro-CT analysis" | FACT |
| Measurement method — histology | HE-stained, 3 μm sections; descriptive only, no quantitative thermal-damage measurement performed | — | Materials and methods — "Histological analysis" | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable — no measured-vs-set comparison performed | — | — | UNKNOWN |
| Incision length error, mm (T1 → T3, mean±SD) | 1 W pulsed: 2.47±1.79 → 1.03±0.59 (p=0.011). 3 W pulsed: 2.38±1.77 → 1.01±0.81 (p=0.012). 1 W CW: 2.40±1.62 → 1.28±0.96 (p=0.026). 3 W CW: 2.25±1.73 → 1.06±0.89 (p=0.026). Scalpel: 2.35±1.50 → 1.30±1.05 (p=0.017). All five methods improved significantly and comparably; repeated-measures ANOVA: significant time effect (p<0.001, η²G=0.144), no significant method effect (p=0.370) or method×time interaction (p=0.444). | mm | Results, Tables 2–3 | FACT |
| Incision depth error, mm (T1 → T3, mean±SD) | 1 W pulsed: 1.43±0.16 → 1.20±0.26 (p=0.009, only setting reaching significance). 3 W pulsed: 1.11±0.47 → 0.97±0.31 (p=0.578, ns). 1 W CW: 1.15±0.36 → 1.01±0.33 (p=0.578, ns). 3 W CW: 0.94±0.49 → 0.78±0.34 (p=0.578, ns). Scalpel: 0.70±0.58 → 0.60±0.38 (p=0.578, ns). ANOVA: strong method effect (p<0.001, η²G=0.268 — laser incisions systematically shallower than scalpel), small but significant time effect (p=0.010, η²G=0.042), no interaction (p=0.600). | mm | Results, Tables 2–3 | FACT |
| Incision width, raw mm (T1 → T3, mean±SD; target = minimal, not a fixed number) | 1 W pulsed: 0.91±0.34 → 0.88±0.27 (p=0.670, ns). 3 W pulsed: 0.94±0.25 → 0.88±0.21 (p=0.633, ns). 1 W CW: 0.97±0.27 → 0.88±0.24 (p=0.633, ns). 3 W CW: 1.03±0.23 → 1.14±0.25 (p=0.408, ns; only setting to widen over time). Scalpel: 0.67±0.30 → 0.79±0.26 (p=0.408, ns). Laser incisions were significantly wider than scalpel at T1 and T2 (all p≤0.001, large effect); at T3 this held only for 3 W CW vs. scalpel (p<0.001, Cohen's d=1.37). ANOVA: strong method effect (p<0.001, η²G=0.195), no time effect (p=0.600), significant method×time interaction (p=0.011, η²G=0.046). | mm | Results, Tables 2–3 | FACT |
| Thermal damage (quantified) | UNKNOWN — histology was descriptive only; no μm-scale thermal-margin measurement was performed for any setting. | — | Results — "Histological findings" | UNKNOWN |
| Thermal damage (qualitative) | HE sections of all laser settings (pooled, not split by setting) showed coagulation necrosis (loss of nuclear staining, increased eosinophilia) and focal carbonization at incision margins; scalpel incisions showed sharply demarcated margins with no thermal alteration. Source explicitly states these descriptive findings "do not support comparative claims regarding the extent of thermal damage among the individual laser settings." | — | Results — "Histological findings" | FACT (qualitative, not setting-specific) |
| Carbonization | Present, qualitative only, pooled across laser settings ("focal carbonization appearing as dark brown to black areas"); not scored or quantified, not split by power/mode. | — | Results — "Histological findings" | FACT (qualitative) |
| Coagulation zone | Present, qualitative only, pooled across laser settings ("coagulation necrosis" at margins); not scored or quantified, not split by power/mode. | — | Results — "Histological findings" | FACT (qualitative) |
| Margin quality (numeric) | UNKNOWN in μm; margin condition described only qualitatively (see thermal damage row above). | — | — | UNKNOWN |
| Diagnostic quality | N/A — no lesion, no pathologist diagnosis; this is a skills-training feasibility study on healthy porcine skin, not a diagnostic-biopsy pathway. | — | — | N/A |
| Subjective workload (NASA-TLX, T1 → T3, mean) | Mental demand: 8.00 → 4.77 (p<0.001). Physical demand: 6.18 → 3.82 (p=0.013). Goal achievement: 11.9 → 6.23 (p<0.001). Frustration: 6.95 → 3.86 (p=0.012). Temporal demand: ns (p=0.764). Effort: ns (p=0.068). | score (0–20 per subscale) | Results — "Subjective workload" | FACT |
| Sample | 22 undergraduate dental students (12F/10M, mean age 25.9y), no prior laser experience, prior scalpel training; porcine skin (~0.8 cm thick, epidermis+dermis+subcutis), 3 sessions at weekly intervals, 5 incisions/session (4 laser settings + 1 scalpel, fixed order) | — | Materials and methods | FACT |

## Notes

- FACT: This is the vault's first source to report a controlled, target-based (known fixed target length of 10 mm) accuracy comparison between diode-laser settings and scalpel, with formal repeated-measures statistics across three practice sessions — directly relevant to this vault's "cutting accuracy/efficiency" question, though as a skills-training feasibility study, not a diagnostic-biopsy pathway.
- FACT: Per this task's explicit instruction, incision speed (mm/s) is NOT computed from the reported operative-time values, even though the target length (10 mm) is known and fixed — operative time is recorded here strictly as reported (seconds per incision), not converted or reinterpreted as a rate.
- FACT: Laser incisions were consistently wider than scalpel incisions and, unlike length accuracy, width did not improve significantly with practice for any laser setting — the source's own Discussion attributes this to the physical nature of laser cutting (thermal ablation plus a coagulation zone inherently widening the cut), not to operator skill, and explicitly cautions that the narrowing width gap at T3 "should not be interpreted as convergence or equivalence."
- FACT: Depth was the least well-controlled dimension for every laser setting (only 1 W pulsed reached significance) and all laser settings remained systematically shallower than the 2 mm target relative to the scalpel — the source attributes this to the non-contact laser's lack of tactile feedback and to a "visual endpoint" (a visible groove) substituting for depth control.
- FACT: No numeric thermal-damage width is reported for any of the four laser settings; the source explicitly disclaims any comparative ranking among its own laser settings from the purely descriptive histology, which limits this source's usefulness for the vault's thermal-damage-magnitude questions even though it directly addresses accuracy/efficiency.
- Classification for this vault: **SUPPORTING** dental-diode evidence — a real dental diode device (SiroLaser Blue, 445 nm) with a formally controlled, target-based accuracy/efficiency design and genuine operative-time data, but a porcine-skin training model (not human oral mucosa), no lesion, and no diagnosis, so it is not a core diagnostic-biopsy-pathway row. Relevant to [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] (accuracy/efficiency theme) and [[04 Evidence/Thermal Artifact]] (qualitative-only corroboration of margin thermal alteration).
