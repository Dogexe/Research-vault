---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 980
set_power_w: 2
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "CW"
fiber_diameter_um: 300
tip_initiation: "initiated"
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: "qualitative (well-defined margins, minimal connective-tissue disruption; no distance measured)"
tissue_architecture: "qualitative (described as clearer/more intact than scalpel group)"
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.1007/s41547-025-00309-w]]
- Source link: https://doi.org/10.1007/s41547-025-00309-w
- Source locator: Full text retrieved from the local Zotero PDF-text cache (`.zotero-ft-cache`, zotero-key B4PC58LYg6669922). Shnawa AA, Taher HJ, Khalil AA. "Minimally invasive excision of oral fibromas: a clinical and histological comparison between diode laser and scalpel techniques." *Lasers Dent Sci.* 2025;9:34. Received 23 Jul 2025, accepted 26 Aug 2025, published online 4 Sep 2025.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Quicklase 12 W Dual Plus 6″ (dual-wavelength 810+980 nm device; 980 nm selected for this study) | — | Materials and methods | FACT |
| Manufacturer | UNKNOWN (brand "Quicklase" only; country of origin stated as England, UK; manufacturer company name not given) | — | Materials and methods | UNKNOWN |
| Wavelength | 980 (device also offers 810 nm, not used for excision in this study) | nm | Materials and methods | FACT |
| Set power | 2 | W | Materials and methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification reported; set/console value only | — | — | UNKNOWN |
| Average power | UNKNOWN | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) | — | Materials and methods | FACT |
| Pulse duration | N/A (CW) | — | — | N/A |
| Frequency | N/A (CW) | — | — | N/A |
| Duty cycle | N/A (CW) | — | — | N/A |
| Fiber diameter | 300 | μm | Materials and methods | FACT |
| Tip type | UNKNOWN (fiber-optic tip, no model/type name given beyond "300-micron fiber optic tip") | — | — | UNKNOWN |
| Tip initiation status | Initiated — "the fiber tip was initiated by gently pressing it against articulating paper to enhance energy absorption and heat retention," stated by the source to optimize cutting efficiency, minimize lateral thermal damage, and improve beam precision | — | Materials and methods | FACT |
| Contact mode | Contact | — | Materials and methods | FACT |
| Exposure duration | UNKNOWN as a per-incision value; not reported at all (unlike some other vault sources, no total procedure-time figure is given either) | — | — | UNKNOWN |
| Thermal-management protocol (non-outcome, procedural) | High-volume evacuation of vapor plume; continuous sweeping motion with minimal contact pressure; intermittent cold saline irrigation; fiber tip regularly cleaned "to avoid carbonization and excessive tissue charring" | — | Materials and methods | FACT (protocol description, not a measured outcome) |
| Measurement method — histology | H&E, paraffin-embedded, light microscopy (Olympus CX21) at 4×/10×/40×, 5MP CMOS camera; qualified pathologist | — | Histopathological examination | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Thermal damage (quantified) | UNKNOWN — no μm-scale thermal-damage-zone or margin-alteration measurement reported for either group. | — | — | UNKNOWN |
| Thermal damage (qualitative) | "Ballooning degeneration" observed in laser-treated specimens (highlighted in Fig. 4), attributed to thermal effects of the laser; overall tissue architecture nonetheless described as clearer/more intact than the scalpel group, attributed by the source to reduced bleeding rather than absence of thermal effect. | — | Results — "Histopathological assessment" | FACT (qualitative) |
| Carbonization | Not reported as an observed histologic finding in either group (the protocol describes tip-cleaning specifically to *avoid* carbonization, but no carbonization is reported as having occurred or been scored). | — | Materials and methods (prevention protocol only) | UNKNOWN (as an outcome) |
| Coagulation zone | Not scored or measured as an isolated histologic variable; hemostasis/coagulation is discussed only as a clinical outcome (bleeding-index score), not a histologic measurement. | — | — | UNKNOWN (as histologic finding) |
| Margin quality | Qualitative only: laser group described as showing "uniform epithelial layer, well-defined margins, and minimal disruption of the underlying connective tissue" (Fig. 3a); scalpel group described as showing "broader epithelial and connective tissue disruption, with obscured details likely due to bleeding and mechanical trauma." No margin distance (mm/μm) is reported for either group. | — | Results — "Histopathological assessment" | FACT (qualitative) |
| Diagnostic quality | No quantified diagnostic-yield percentage is reported for either group. Qualitative statement only: "laser-excised specimens were more favorable for histological interpretation compared to those obtained by scalpel surgery... likely due to reduced bleeding," and the Discussion states "concerns regarding thermal artifacts compromising histopathological analysis were not observed in this study, as tissue integrity was well maintained in all laser-excised specimens." All excised lesions from both groups were sent for histopathological analysis to confirm the clinical diagnosis (fibroma), but a numeric per-group diagnostic-success count/percentage is not stated in the retrieved text. | — | Results / Discussion | FACT (qualitative statement only) / UNKNOWN (quantified yield) |
| Lesion size | Representative cases shown are approximately 0.5 cm diameter (Figs. 1–2); no size range or distribution across the full n=24 laser-group sample is reported. | cm | Figures 1–2 (representative cases only) | FACT (representative cases only, not sample-wide) |
| Sample | 48 patients (24 laser, 24 scalpel), age 22–65, oral fibroma, Basra Teaching Hospital, Nov 2024–Jul 2025; groups determined by a priori power analysis | — | Materials and methods | FACT |
| Clinical outcomes (for context, not histologic) | Laser group had significantly less intraoperative bleeding, postoperative edema, and functional interference (p<0.005); lower mucosal scar index at weeks 2 and 4 (p=0.0001); reduced pain days 1–3 (p≤0.0008); 100% "excellent" satisfaction (laser) vs. 41.6% (scalpel), p=0.0001. | — | Results, Tables 2–4 | FACT |

## Notes

- FACT: This is the vault's first **CORE-tier** biopsy-adjacent source to explicitly report [[03 Concepts/Glossary/Initiated Tip|tip-initiation]] status as a described, real protocol step (pressing the fiber tip against articulating paper) rather than leaving it UNKNOWN — closing, for this one source, a gap previously open in seven of eight core biopsy sources per [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] §5.
- FACT, cross-source link: The exact initiation method reported here (articulating paper) is one of the two non-standardized techniques explicitly named and cautioned against by [[07 Data/Romanos et al 2013 - Diode Laser Soft-Tissue Surgery Review Data|Romanos 2013 (Compendium)]], processed in this same batch: "Diode laser manufacturers have noted this issue and now suggest initiating laser fibers using cork or articulating paper. These non-standardized techniques do not guarantee consistent initiation, nor does the initiation last longer than a few seconds while cutting tissue." This is Romanos's own general caution about the technique class, not a claim about Shnawa et al.'s specific device or outcome — it is recorded here as a directly relevant caveat on how much confidence to place in "initiated" as a fixed, verified device state for the duration of Shnawa et al.'s procedure, not as evidence that Shnawa et al.'s initiation failed.
- FACT: No numeric diagnostic-yield percentage, thermal-damage width, or margin distance is reported for either group — this source strengthens the CORE evidence base's clinical/qualitative-histologic picture (diode preserves tissue architecture despite minor thermal artifact) but does not add a new quantified data point to the vault's ≥4–5 mm margin threshold, its μm-scale [[03 Concepts/Glossary/Thermal Damage|thermal-damage]] range, or its diagnostic-yield-percentage table column.
- FACT: This source's own citation list (ref. 30–31) cites de Oliveira Andriola et al. 2018 and Lopes-Santos et al. 2022 on diode-laser histologic artifact risk in inflammatory fibrous hyperplasia and cytological artifacts respectively — these are the source's own citations, not independently verified by this vault, and are distinct from [[07 Data/Lopes-Santos et al 2023 - High-Power Laser Oral Biopsy Histology Systematic Review Data|Lopes-Santos et al. 2023]] already processed in this vault (a different, later Lopes-Santos publication).
- Classification for this vault: **CORE** biopsy evidence — a real human diode oral-soft-tissue excisional-biopsy pathway (n=24 laser-treated, RCT-style comparator design) with device, wavelength, set power, mode, fiber diameter, contact mode, and tip-initiation status all explicitly reported, and histopathological confirmation of diagnosis performed — but no quantified thermal-damage width, margin distance, or diagnostic-yield percentage. Relevant to [[04 Evidence/Biopsy Specimen Quality]], [[04 Evidence/Surgical Margins]], [[04 Evidence/Thermal Artifact]], and the tip-initiation gap in [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] §5.
