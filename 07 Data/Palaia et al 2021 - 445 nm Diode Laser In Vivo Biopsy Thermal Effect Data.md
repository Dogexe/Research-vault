---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 445
set_power_w: 2.5
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 320
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: real human diagnostic-biopsy pathway — a core biopsy-quality source, comparable in kind to Angiero et al. 2011, Romeo et al. 2014, and Gambino et al. 2026.**

## Source

- Citation: Palaia G, D'Alessandro L, Pergolini D, Carletti R, Di Gioia CRT, Romeo U. "In vivo clinical and histological thermal effect of a 445 nm diode laser on oral soft tissues during a biopsy." *J Oral Sci.* 2021;63(3):280-282. DOI: [10.2334/josnusd.20-0665](https://doi.org/10.2334/josnusd.20-0665)
- Literature note: [[02 Literature/10.2334/josnusd.20-0665]]
- Source type: Uncontrolled clinical trial (in vivo human excisional biopsies), single operator, single device/setting
- Source locator: Full text (Abstract; Introduction; Materials and Methods; Results; Table 1; Fig. 3; Discussion), retrieved from the attached PDF via the local Zotero library.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Blue diode laser (Eltech K-Laser srl, Treviso, Italy) | — | Materials and Methods | FACT |
| Manufacturer | Eltech K-Laser srl | — | Materials and Methods | FACT |
| Wavelength | 445 ± 5 | nm | Materials and Methods | FACT |
| Set power | 2.5 | W | Materials and Methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; "a power of 2.5 watts" is a set/console value only | — | — | UNKNOWN |
| Average power | UNKNOWN (CW, no distinct average-power field beyond the 2.5 W set value) | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) | — | Materials and Methods | FACT |
| Pulse duration | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Frequency | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Duty cycle | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Fluence | 3,100 | J/cm² | Materials and Methods | FACT |
| Fiber diameter | 320 | μm | Materials and Methods | FACT |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact / non-contact mode | UNKNOWN — not explicitly stated | — | — | UNKNOWN |
| Incision speed | UNKNOWN — not reported numerically | — | — | UNKNOWN |
| Excision protocol | Excisional biopsy; lesion tractioned with a suture, incision made around all sides of the lesion; no sutures applied post-excision | — | Materials and Methods | FACT |
| Specimen margin | UNKNOWN — no numeric margin/specimen-size value reported for the excisions performed in this study (a ≥0.5 mm additional margin is recommended in the Discussion for future suspicious-lesion cases, not the margin actually used here) | — | — | UNKNOWN (as used) / FACT (as a stated future recommendation only) |
| Tissue model | In vivo human oral soft tissue, real excisional biopsies of clinically benign lesions | — | Materials and Methods | FACT |
| Measurement method | Thermal alteration extent quantified separately for epithelium and connective tissue on H&E-stained sections (×100 magnification) using ImageScope software; mean and SD compared by Student's t-test | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN — no laser power-meter calibration protocol reported | — | — | UNKNOWN |
| Diagnostic yield | Definitive histological diagnosis obtained in all 42/42 (100%) excisional specimens (40 patients, 2 with two lesions each) | — | Results | FACT |
| Thermal-effect-evaluable specimens | 38 of 42 (4 specimens excluded from thermal-effect measurement only, due to incorrect orientation after processing — diagnosis was still obtained in all 42) | — | Results | FACT |
| Epithelial thermal effect, mean | 507.07 (Abstract) / 507.08 (Table 1 summary row) | μm | Abstract; Table 1 | FACT — two figures given by the source itself (507.07 vs. 507.08), preserved as reported, not reconciled |
| Epithelial thermal effect, SD | ±280 (Results text) / ±283.76 (Table 1 summary row) | μm | Results; Table 1 | FACT — internal discrepancy between the source's own Results narrative and its own Table 1 summary row; preserved verbatim, not resolved. NEEDS VERIFICATION. |
| Connective tissue thermal effect, mean | 320.39 | μm | Abstract; Results; Table 1 | FACT |
| Connective tissue thermal effect, SD | ±206.28 (Results text) / ±209.04 (Table 1 summary row) | μm | Results; Table 1 | FACT — same pattern of internal discrepancy as the epithelial SD above. NEEDS VERIFICATION. |
| Epithelial vs. connective tissue thermal effect, statistical comparison | Student's t-test, p=0.00085 (≤0.001); epithelial effect significantly greater than connective tissue effect | — | Results | FACT |
| Epithelial alteration >1 mm | 3 of 38 evaluable cases | — | Results; Table 1 | FACT |
| Per-case thermal effect range | Epithelial: 126.0–1,188.0 μm (evaluable cases); Connective tissue: 111.6–926.9 μm (evaluable cases) | μm | Table 1 | FACT |
| Coagulation zone | Not scored as an isolated variable; discussed qualitatively as the mechanism behind greater thermal effect in highly vascularized lesions (e.g., pyogenic granuloma) requiring more intraoperative photocoagulation | — | Discussion | FACT (qualitative mechanism description, not a measured finding) |
| Carbonization | Not scored; mentioned only as an advisory to use "correct fiber movements... to limit tissue carbonization" | — | Discussion | FACT (advisory only, not measured) |
| Complications | No intraoperative complications requiring intervention beyond routine hemostasis monitoring; no postoperative complications in any case; regular healing at 7-day, 1-month, and 3-month follow-up in all cases; no recurrence | — | Results | FACT |
| Sample | 42 excisional biopsies in 40 patients (53% male, 47% female); lesion types: focal fibrous hyperplasia (most common), squamous papilloma, pyogenic granuloma, peripheral giant cell granuloma, lymphoepithelial cyst, keratosis with no dysplasia, inflammatory focal fibrous hyperplasia, granulation tissue, mucocele, ectopic lymphoid tissue; most frequent site buccal mucosa | — | Materials and Methods; Results; Table 1 | FACT |

## Notes

- FACT: This is a new, large (n=42, the second-largest in-vivo diagnostic-yield sample in this vault after Angiero et al.'s n=608) 100% diagnostic-yield data point, at a single fixed CW setting (2.5 W, 445 nm, 320 μm fiber) — directly comparable in kind to [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield|Angiero et al. 2011]], [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]], and [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data|Gambino et al. 2026]].
- FACT, directly relevant to whether wavelength modifies thermal damage: this source's own Discussion explicitly compares its 445 nm result to [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]] (already in this vault), stating that Romeo et al.'s 808 nm diode and 532 nm KTP lasers both showed a *lower* extent of thermal effect in vivo than the present 445 nm device, though the source itself notes Romeo et al.'s sample size was smaller. This is the source's own cross-study comparison, not independently re-derived here, but it is directly checkable against this vault's own Romeo et al. extraction: Romeo et al.'s diode-only margin damage ranged 0.149–0.473 mm (149–473 μm) across lesion types, versus Palaia et al.'s 445 nm mean epithelial effect of 507.07 μm — Palaia et al.'s mean value is numerically above the top of Romeo et al.'s 808 nm diode range, consistent in direction with the source's own claim, though the two studies use different measurement methods and lesion-type mixes, so this is not a controlled wavelength comparison.
- FACT: Epithelial thermal effect (507.07 μm) was significantly *greater* than connective-tissue thermal effect (320.39 μm) in this 445 nm study (p=0.00085) — the *opposite* compartment pattern from [[07 Data/Gambino et al 2026 - Diode Laser OCT and Histologic Thermal Damage Data|Gambino et al. 2026]]'s 980 nm result, where connective-tissue damage (430.3 μm) exceeded epithelial damage (288.9 μm). This is a genuine cross-source difference in *which tissue compartment* shows greater thermal alteration, co-occurring with a wavelength difference (445 nm vs. 980 nm) — INTERPRETATION, not established as causal by any single vault source, since device, power, fluence, and patient population also differ between the two studies.
- INTERPRETATION (source's own): the source attributes the epithelium > connective-tissue pattern to selective photothermolysis — energy absorbed by hemoglobin in vascularized connective tissue is carried away from the immediate surgical site, "reducing alteration of the surrounding tissue," while highly vascularized lesions (pyogenic granuloma) needing more intraoperative photocoagulation showed the largest thermal effects of any lesion type in this series.
- FACT: The source's own Discussion cites a companion ex vivo study using the same laser device (Palaia et al. 2020, *Int J Environ Res Public Health*, not itself processed in this vault) at 2 W and 3 W CW, noting that in vivo epithelial thermal effect was *greater* than the ex vivo result at the same device, while connective-tissue effect was *smaller* in vivo — attributed by the source to the absence of vascular perfusion in the ex vivo (deceased pig tongue) model. This is the source's own citation of a non-vault-processed paper, not independent vault verification, but it is consistent in direction with [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]]'s own discussion of ex vivo thermal effects likely being underestimated relative to in vivo due to reduced vascularization.
- FACT: The source's own Discussion recommends widening excisional margins by "at least 0.5 mm" for potentially malignant lesions to compensate for thermal alteration — this matches, independently, [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]]'s own ~0.5 mm compensatory-margin recommendation (a different metric from the ≥5 mm/≥2 mm *total specimen/margin size* recommendations discussed in [[06 Synthesis/Contradictions in Diode Laser Biopsy Evidence]] — this vault does not treat "additional margin to compensate for thermal alteration" and "total minimum specimen/margin size for reliable diagnosis" as the same metric).
- NEEDS VERIFICATION: the source's own Abstract/Results-text SD values (±280 μm epithelial; ±206.28 μm connective) do not exactly match its own Table 1 summary-row SD values (±283.76 μm; ±209.04 μm), and the mean epithelial value itself differs trivially between Abstract (507.07) and Table 1 (507.08). Both figures are preserved verbatim; this vault does not reconcile the discrepancy.
- HYPOTHESIS: UNKNOWN — no formal hypothesis beyond the study's own stated aim and its forward-looking margin-widening suggestion (explicitly flagged by the source itself as needing future confirmation).
- Limitations (source-stated and vault-noted): uncontrolled trial (no comparator arm within this study); single operator; single fixed device/setting (no power or mode variation); specimen size/margin not reported numerically; tip-initiation and contact-mode status not reported; no independent power-meter verification of the 2.5 W set value.
- Classification for this vault: direct dental-diode biopsy diagnostic-yield and thermal-effect evidence, real human in vivo pathway, single fixed CW setting. Relevant to [[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Thermal Artifact]], and [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]].
