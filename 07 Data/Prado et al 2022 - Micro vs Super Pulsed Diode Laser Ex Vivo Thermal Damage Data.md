---
classification: SUPPORTING TECHNICAL
oral_tissue: true
ex_vivo: true
human_tissue: false
diode_laser: true
wavelength_nm: 940
set_power_w:
  - 1.2
  - 1.8
measured_power: true
measured_power_value_reported: true
measured_power_w:
  - 1
  - 1.5
  - 3.2
power_meter: PM600 Power Meter (Molectron Detector Inc, Portland, OR, USA)
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
speed_varied: null
cw_pw: "CW+PW"
fiber_diameter_um:
  - 300
  - 400
tip_initiation: initiated
contact_mode: null
histology: true
thermal_damage: true
thermal_damage_measure: "quantified (thermal-damage area and depth; 606–1024 μm depth across groups)"
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

- Literature note: [[02 Literature/10.1002/cre2.670|Prado et al. 2022]]
- Source link: https://doi.org/10.1002/cre2.670
- Source locator: Full text (PDF, via `pdftotext` extraction cross-checked against the rendered PDF) — Abstract; Material and Methods; Table 1 (group distribution and diode laser parameters); Results §3.1–3.4; Tables 2–4; Discussion; Conclusion.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Devices | Epic X™ (micro pulsed diode laser, G2–G9) and Epic Pro™ (super pulsed diode laser, G10), both Biolase, Irvine, CA, USA | — | Material and Methods | FACT |
| Manufacturer | Biolase, Irvine, CA, USA | — | Material and Methods | FACT |
| Wavelength | 940 | nm | Material and Methods (both devices) | FACT |
| Power at display (console/set) — micro pulsed groups | 1.2 and 1.8 (each tested across CW, CP0, CP1, CP2 modes) | W | Table 1 | FACT |
| Power at display (console/set) — super pulsed group (G10) | n/a — no average-power console value is shown for this device; only a peak-power display value of 80 W is given (a different metric, see "Peak power" row) | W | Table 1 | FACT (n/a as reported) |
| Power measured (independently, via power meter) | G2/G4/G6/G8: 1.0; G3/G5/G7/G9: 1.5; G10: 3.2 | W | Table 1 | FACT |
| Power verification method | "The output power was checked before the start of each surgical procedure using a [[03 Concepts/Glossary/Power Meter\|power meter]] (PM600 Power Meter, Molectron Detector Inc, Portland, OR, USA)." — verification timing is per-procedure (before each surgical excision), not stated as per-incision within a single specimen | — | Material and Methods | FACT |
| Measurement location | UNKNOWN — no [[03 Concepts/Glossary/Measurement Location\|location]] (e.g., fiber tip / distal end) is stated for the power-meter check, only the timing ("before the start of each surgical procedure") | — | — | UNKNOWN |
| Power density (calculated) | 1415.4 (at 1 W measured); 2123.1 (at 1.5 W measured); 2547.7 (at 3.2 W measured) | W/cm² | Table 1 | FACT (derived by source from the measured, not display, power values) |
| Peak power at display | G2: 1.2; G3: 1.8; G4: 6; G5: 9; G6: 3.6; G7: 5.4; G8: 2.4; G9: 3.6; G10: 80 | W | Table 1 | FACT |
| Operating mode | CW (G2, G3); CP0/20% duty cycle (G4, G5); CP1/33% duty cycle (G6, G7); CP2/50% duty cycle (G8, G9); STP/super pulsed (G10) | — | Table 1; Material and Methods | FACT |
| Pulse duration / pulse interval | CP0: reported as "10 [unit]" / "40 [unit]"; CP1: "100 [unit]" / "200 [unit]"; CP2: 1 ms / 1 ms; G10 (STP): pulse width 10 μs–10 ms, pulse interval 0.01 ms–20 ms | ms or μs | Table 1; Material and Methods | FACT (ratios and CP2/G10 values) / **NEEDS VERIFICATION** — the ms/μs unit prefix for the CP0 and CP1 pulse-duration and pulse-interval values did not render cleanly in text extraction (the μ character was dropped in multiple places); the stated duty-cycle percentages (20%, 33%) are internally consistent with the numeric ratios either way, but the exact time unit for CP0/CP1 should be re-checked against the original PDF table before being used for anything beyond duty-cycle ratios |
| Duty cycle | 20% (CP0), 33% (CP1), 50% (CP2); CW and STP not expressed as a duty-cycle percentage | % | Table 1 | FACT |
| Fiber diameter / tip | 300 μm disposable-initiated surgical tip (micro pulsed, G2–G9); 400 μm disposable-initiated surgical tip (super pulsed, G10) | μm | Material and Methods | FACT |
| Tip initiation status | Both tips explicitly described as "disposable-initiated surgical tips" | — | Material and Methods | FACT |
| Contact / non-contact mode | UNKNOWN — not explicitly stated anywhere in the Methods or Figure captions | — | — | UNKNOWN |
| Incision / excision speed (mm/s or cm/s) | Not reported. The source records excision **time** (seconds, from laser application to complete sample removal), not a controlled or measured cutting speed; laser cutting was performed manually ("laser cutting of the tissue was done manually") with no target or measured speed value given | — | Material and Methods; Discussion (limitations) | FACT (that no speed value is reported; manual execution is stated) |
| Excision protocol | 100 standardized 8 mm-diameter specimens excised from the dorsal portion of fresh pig tongues, 10 groups of n=10 (G1 scalpel control, G2–G9 micro pulsed diode, G10 super pulsed diode); excisions at room temperature (22–24 °C) | — | Material and Methods | FACT |
| Specimen/tissue model | Fresh pig tongue (ex vivo, within 24 h of slaughter, stored 2–4 °C); standardized non-lesional 8 mm circular excisions, not real lesions | — | Material and Methods | FACT |
| Measurement method (thermal damage) | Standard histological processing (10% buffered formalin, paraffin-embedded, 4 μm serial sections, H&E stain); examined under light microscopy (Nikon Eclipse 80i) at 40× magnification; both total area (mm²) and depth (μm) of thermal damage measured per specimen | — | Material and Methods | FACT |
| Calibration method | UNKNOWN beyond "power meter (PM600...)" — no [[03 Concepts/Glossary/Calibration\|calibration]] certificate, traceability standard, or calibration schedule for the meter itself is reported | — | — | UNKNOWN |
| Statistical methods | Shapiro–Wilk normality test; Kruskal–Wallis nonparametric test across groups; Dunn's multiple-comparison test with Bonferroni correction; Spearman's rank correlation (area vs. depth); significance level 5% | — | Material and Methods | FACT |
| Total area of thermal damage (range across group medians) | 0.91–1.97 | mm² | Results §3.1; Table 2 | FACT |
| Depth of thermal damage (range across group medians/min–max) | 606–1024 (source's own summary figure); full group-level min–max range 317.6–1555.0 | μm | Results §3.3; Table 3 | FACT |
| Area of thermal damage — group comparison | G3 (CW, 1.5 W measured) significantly lower area than G7 (33% duty, 1.5 W measured) and G9 (50% duty, 1.5 W measured), p = .009 (Kruskal–Wallis); no other pairwise group differences reached significance | — | Results §3.1; Table 2 | FACT |
| Depth of thermal damage — group comparison | No statistically significant differences among laser groups G2–G10, p = .125 (Kruskal–Wallis) | — | Results §3.2; Table 3 | FACT |
| Area–depth correlation | Positive correlation between depth (μm) and area (mm²) of thermal damage (Spearman) | — | Results §3.3; Figure 4 | FACT |
| Excision time | Control (G1, scalpel) and super pulsed diode (G10) medians were significantly lower than all micro pulsed diode groups (G2–G9), p < .001; G10's median excision time was comparable to the scalpel control | s | Results §3.4; Table 4 | FACT |
| Diagnostic yield / diagnosis rendered | Not applicable — ex vivo, non-lesional standardized excisions; no diagnosis was rendered on any specimen | — | — | N/A (by design) |
| Margin recommendation | "A minimum of 1 mm perimeter of healthy margins is recommended for appropriate microscopic analysis of the tissue specimen," derived from the observed 606–1024 μm thermal-damage depth range, stated as consistent with Romeo et al.'s (2014) recommended 0.5–1 mm healthy-tissue halo | mm | Conclusion; Discussion | FACT |
| Carbonization | Discussed narratively via the [[03 Concepts/Glossary/Hot-tip Effect\|"hot tip effect"]] mechanism (carbonized build-up at the fiber tip affecting depth of penetration); not scored or quantified as its own numeric outcome | — | Discussion | FACT (qualitative mechanism) / UNKNOWN (no numeric score) |
| Coagulation zone | UNKNOWN — not scored or measured as a distinct variable | — | — | UNKNOWN |
| Sample size per analysis | Thermal-damage area/depth: n=10 per group except G8 and G10 (n=9); excision time: n=10 per group except G7, G8, G9 (n=9) — some specimens excluded, reason for exclusion not stated in the extracted text | — | Tables 2–4 | FACT (n as tabulated) / UNKNOWN (reason for n<10 in some groups) |

## Notes

- FACT: This source directly and cleanly demonstrates the vault's central set-vs-measured-power distinction: the [[03 Concepts/Glossary/Set Power|console/display]] average power (1.2 W, 1.8 W) is independently checked with a power meter (PM600) before each surgical procedure, and the **[[03 Concepts/Glossary/Measured Power|measured]]** average power is consistently lower than the displayed value at both settings (1.2 W display → 1.0 W measured; 1.8 W display → 1.5 W measured, both a ~17% under-delivery). This is one of the cleanest documented set-vs-measured power gaps in this vault's diode literature, and directly supports [[04 Evidence/Set Power vs Measured Output]].
- FACT: Despite the measured-power rigor, incision speed is explicitly **not** a controlled or reported variable in this study — cutting was performed manually, and only elapsed excision **time** (not a mm/s or cm/s speed) was recorded. The source's own Discussion (Limitations) states manual cutting "may have introduced the possibility of small random errors" in the area measurements. This means Prado et al. 2022 satisfies `measured_power = true` and `measured_power_value_reported = true`, but **not** `incision_speed_reported` — it therefore does **not** newly qualify for Table C of [[06 Synthesis/Study Dashboard]] (which additionally requires `incision_speed_reported = true`), even though it strengthens the measured-power evidence base.
- FACT / vault judgment call — `biopsy_oriented: false`: the paper's own language repeatedly frames this as simulating "excisional biopsy" (Figure 2 caption, Keywords: "oral biopsy," Discussion: "biopsied tissues," Conclusion: "surgical excisions adequate for histopathological evaluation") and its stated secondary aim is a clinical guideline for biopsy parameters. However, per this vault's operational definition (`biopsy_oriented` = excising/examining a **real lesion**, not a standardized incision/block on non-lesional tissue — see [[99 Templates/Study Metadata Schema]]), the 100 specimens here are standardized 8 mm circular excisions from **healthy, non-lesional** dorsal pig tongue, not real lesions. This is handled identically to [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data|Hanke et al. 2021]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data|Strakas et al. 2023]], and [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]] — all use biopsy-simulating language while excising non-lesional tissue, and all are `biopsy_oriented: false` under this vault's stricter operational test. Flagged here explicitly because a reader relying on the paper's own framing (rather than this field's definition) could reasonably disagree.
- FACT: The source's own margin recommendation (≥1 mm healthy margin) sits within the range already documented in this vault — narrower than the ≥5 mm figures from clinical/diagnostic-biopsy sources (Angiero 2011, Romeo 2014, Gambino 2026, Gundlapalle 2022) and close to Pergolini et al. 2025's ≥2 mm ex vivo recommendation — consistent with the vault's existing observation that ex vivo/technical sources tend to recommend smaller margins than clinical diagnostic-biopsy sources. See [[01 Projects/Diode Laser Biopsy]] §7, "Key unresolved assumptions" ("Margin-width recommendations differ between clinical and ex-vivo studies and are not treated as transferable standards").
- NEEDS VERIFICATION: Table 1's raw layout renders with misaligned columns in both the PDF viewer and `pdftotext` extraction (rows/values do not line up cleanly under their column headers). The group-by-group values used above (power at display, power measured, peak power, pulse settings) were reconstructed by cross-checking the internal arithmetic (peak = display power ÷ duty cycle; power density scaling with measured power) and the prose in Results/Discussion (which independently names G3 as "CW, 1.5 W," G7 as "1.5 W, 33% duty cycle," G9 as "1.5 W, 50% duty cycle," and G10 as "3.2 W" average / "80 W" peak) — all cross-checks were internally consistent, but a human should still visually re-confirm Table 1 against the original PDF given the extraction difficulty.
- NEEDS VERIFICATION: The exact time unit (ms vs. μs) for the CP0 and CP1 pulse-duration/pulse-interval values could not be confirmed from the extracted text (the μ character did not render). This does not affect the reported duty-cycle percentages (20%, 33%), which are stated directly, but affects only the raw pulse-duration/interval values in the extraction table above.
- FACT: No independent verification of the specimen excision boundary itself (margin readability, tissue-architecture preservation as a distinct score) is performed — the study's two outcome measures are thermal-damage area/depth and excision time only. This is consistent with this vault's existing observation (see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]) that no ex vivo diode source yet defines a formal margin-readability or tissue-architecture-preservation scoring instrument.
- Classification for this vault: SUPPORTING TECHNICAL — ex vivo, non-lesional, measured-power + thermal-damage/excision-time comparison of micro vs. super pulsed diode operating modes; strengthens the measured-power side of the novelty chain but does not report a controlled/measured incision speed and does not excise a real lesion. Relevant to [[04 Evidence/Set Power vs Measured Output]], [[04 Evidence/Power Output and Tissue Effect]], and [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]].

## Related notes

- Literature: [[02 Literature/10.1002/cre2.670]]
- Related: [[07 Data/Hanke et al 2021 - Eight-Wavelength Diode Cut Efficiency Data]], [[07 Data/Strakas et al 2023 - 940nm Diode Cutting Efficiency and Thermal Damage Data]], [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data]] (same measured-power-without-controlled-speed pattern), [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data]] (margin recommendation cited by this source)
- Synthesis: [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]], [[06 Synthesis/Study Dashboard]]
