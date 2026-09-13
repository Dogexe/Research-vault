---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: null
set_power_w: 5.12
measured_power: null
measured_power_value_reported: null
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: null
speed_mm_s: null
speed_control: unknown
cw_pw: "PW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: null
diagnostic_outcome: null
biopsy_oriented: true
full_text: false
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: ABSTRACT-LEVEL ONLY.** No full-text PDF/HTML is cached in this vault's local Zotero library for this source (the literature note has no attached-file link, unlike Goharkhay et al. 1999 and Palaia et al. 2021), and no PMCID is available for this PMID via PubMed's ID-conversion lookup — no free full text exists on PubMed Central. A web search for an open-access copy did not locate one. This extraction is therefore built entirely from the structured abstract retrieved via PubMed, per the same convention already used in this vault for Capodiferro et al. 2008. Most methodological parameters below are UNKNOWN because the abstract does not report them; this is a genuine reporting gap in what is available to this vault, not a claim that the full paper omits them.

According to PubMed, the following is drawn from: Suter VGA, Altermatt HJ, Sendi P, Mettraux G, Bornstein MM. "CO2 and diode laser for excisional biopsies of oral mucosal lesions. A pilot study evaluating clinical and histopathological parameters." *Schweiz Monatsschr Zahnmed.* 2010;120(8):664-671. PMID: 21038754. No DOI is available in PubMed's record for this article (PII: smfz-2010-08-01).

## Source

- Literature note: [[02 Literature/CO2 and diode laser for excisional biopsies of oral mucosal lesions. A pilot study evaluating clinical and histopathological parameters]]
- Source link: https://pubmed.ncbi.nlm.nih.gov/21038754/
- Source locator: PubMed structured abstract only (retrieved via `get_article_metadata`), no full text available in this vault.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Unnamed CO2 laser and unnamed diode laser (make/model not given in the abstract) | — | Abstract | UNKNOWN (device names) / FACT (laser types used) |
| Manufacturer | UNKNOWN | — | — | UNKNOWN |
| Wavelength | UNKNOWN — not stated for either laser in the abstract | — | — | UNKNOWN |
| Set power — CO2, continuous-wave (cw) group | 5 | W | Abstract | FACT |
| Set power — CO2, pulsed "char-free" (cf) group | UNKNOWN — labeled only as a distinct pulsed setting, no wattage given in the abstract | — | Abstract | UNKNOWN |
| Set power — diode group | 5.12 | W | Abstract | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification is mentioned in the abstract; all values presented are instrument/panel settings | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | CO2: continuous wave (cw) and a distinct pulsed "char-free" (cf) mode (two CO2 arms); Diode: pulsed mode only (one arm, 5.12 W) | — | Abstract | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | UNKNOWN | — | — | UNKNOWN |
| Tip type / tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact / non-contact mode | UNKNOWN | — | — | UNKNOWN |
| Incision speed | UNKNOWN | — | — | UNKNOWN |
| Excision protocol | Excisional biopsy of fibrous hyperplasia in the buccal mucosa | — | Abstract | FACT |
| Specimen margin / size | UNKNOWN | — | — | UNKNOWN |
| Tissue model | In vivo human, randomized pilot trial (real excisional biopsies) | — | Abstract | FACT |
| Measurement method | Thermal damage zone assessed both in μm and via an unnamed "histopathological index" score; exact histologic technique (staining, magnification, blinding) UNKNOWN from the abstract | — | Abstract | FACT (that both a μm and an index measure were used) / UNKNOWN (technique detail) |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Thermal damage zone — CO2 (both settings) vs. diode | Significantly smaller with the CO2 laser for both settings tested, compared to the diode laser, "regarding values in μm or histopathological index scores" — exact numeric values not given in the abstract | — | Abstract | FACT (direction and significance) / UNKNOWN (exact magnitude) |
| Diagnostic yield | UNKNOWN — not addressed in the abstract; the study's stated focus is thermal-damage-zone extent and peri-operative complications, not diagnostic readability or yield | — | — | UNKNOWN |
| Coagulation zone | UNKNOWN — not mentioned in the abstract | — | — | UNKNOWN |
| Carbonization | UNKNOWN — not mentioned in the abstract | — | — | UNKNOWN |
| Complications | Bleeding was the only intraoperative complication encountered (group not specified in the abstract), controlled with electrocauterization; no postoperative complications in any of the three groups | — | Abstract | FACT |
| Sample | 15 patients with fibrous hyperplasia, randomized to one diode group or two CO2-laser groups (exact per-group n not given in the abstract) | — | Abstract | FACT (total n and randomization) / UNKNOWN (per-group n) |

## Notes

- FACT: The abstract's own stated conclusion is that the CO2 laser offers a smaller collateral [[03 Concepts/Glossary/Thermal Damage|thermal-damage zone]] than the diode laser at the settings tested (CO2 5 W cw and an unspecified-wattage pulsed char-free mode, vs. diode 5.12 W pulsed) — this is a cross-laser-type comparison (CO2 vs. diode), not a CW-vs-PW comparison within the diode laser itself, since the diode arm here uses only one mode (pulsed).
- FACT: This source cannot be used as CW-vs-PW evidence for the diode laser specifically, because only one diode setting (5.12 W pulsed) was tested — there is no diode CW arm in this study to compare against.
- FACT: This is the highest diode set-power value (5.12 W) reported anywhere in this vault's biopsy-adjacent literature to date — outside the 1.6–2.7 W range associated with the vault's other quantified-diagnostic-yield sources, and outside the 2–4 W range tested by [[07 Data/Pergolini et al 2025 - Dual-Wavelength Diode Laser Ex Vivo Thermal Damage Data|Pergolini et al. 2025]]. Because this source reports greater diode thermal damage than CO2 at this higher power, but does not report a diagnostic-yield outcome or a same-laser lower-power comparator, it cannot by itself be used to extend or contradict the vault's evidence-supported CW power range — it is simply a different, higher power point with no diagnostic-outcome data attached.
- NEEDS VERIFICATION: Whether the diode laser's wavelength, fiber, contact mode, and calibration status materially affected the reported CO2-vs-diode difference cannot be assessed from the abstract alone. Full-text access is needed before this source can contribute more than a single high-power, abstract-level data point.
- Limitations (source-stated, from the abstract): pilot scale (n=15, unevenly split across three groups); the authors' own stated conclusion calls for more study participants to resolve differences between the two CO2 settings, implying the study is likely underpowered even for its own primary comparison.
- HYPOTHESIS: UNKNOWN — no formal hypothesis stated beyond the pilot study's own aim.
- Classification for this vault: abstract-level-only cross-laser-type (CO2 vs. diode) thermal-damage comparison; contributes one additional, higher-power diode data point but cannot be integrated into the vault's within-diode CW-vs-PW or power-range analysis without full-text access. Relevant to [[04 Evidence/Thermal Artifact]] and [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]].
- METADATA CONVENTION — abstract-only null cascade: `measured_power`, `measured_power_value_reported`, `incision_speed_reported`, and `diagnostic_outcome` are all recorded as `null`, not `false`, per the schema's explicit abstract-only exception (see [[99 Templates/Study Metadata Schema]], "The meaning of true/false/null") — this source's abstract does not mention these properties, but with `full_text: false` there is no complete Methods/Results section to confirm the full paper is actually silent on them, so `false` would overstate what this vault can confirm. `histology`, `thermal_damage`, and `cw_pw` are populated (not null) because the abstract itself directly and explicitly states them (a μm/histopathological-index thermal-damage comparison, and "diode: pulsed mode only"). `classification: CORE BIOPSY` is retained because the abstract explicitly states "excisional biopsies of oral mucosal lesions" — a directly-reported fact, not dependent on the missing full text.
