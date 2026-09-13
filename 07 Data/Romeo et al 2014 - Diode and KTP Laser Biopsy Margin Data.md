---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 808
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
fiber_diameter_um: 320
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: "quantified (histologic margin damage, mm, per lesion type; diode-only values 0.149-0.623 mm)"
tissue_architecture: null
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/Biopsy of Different Oral Soft Tissues Lesions by KTP and Diode Laser_ Histological Evaluation - Romeo - 2014 - The Scientific World Journal - Wiley Online Library]]
- Source link: https://doi.org/10.1155/2014/761704
- Source locator: Full text (Introduction; Materials and Methods; Results; Discussion; Tables 1–4), retrieved from the Wiley Online Library page via the local Zotero library (zotero-key 464BCCSL). Upgraded from an earlier PMC-API extraction with per-patient device attribution now available.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Diode laser (SOL, DenMat Italia, Italy); KTP laser (SmartLite, DEKA, Italy) | — | Materials and Methods | FACT |
| Manufacturer | DenMat Italia (diode); DEKA (KTP) | — | Materials and Methods | FACT |
| Wavelength | Diode: 808; KTP: 532 | nm | Materials and Methods | FACT |
| Set power | Diode: 2 W CW; KTP: 1.5 W PW | W | Materials and Methods | FACT |
| Measured output power | UNKNOWN — set/console values only, no independent power-meter verification reported | — | — | UNKNOWN |
| Average power | UNKNOWN (fluence reported instead — see below) | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Diode: continuous wave (CW); KTP: pulsed wave (PW) | — | Materials and Methods | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fluence | Diode: 2400 J/cm²; KTP: 212 J/cm² | J/cm² | Materials and Methods | FACT |
| Fiber diameter (spot size) | Diode: 320; KTP: 300 | μm | Materials and Methods | FACT |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | UNKNOWN — not explicitly stated as contact or non-contact | — | — | UNKNOWN |
| Exposure duration | UNKNOWN as a per-incision value; overall surgical intervention constrained to ≤5 minutes for patient compliance; local anesthesia 1.8 mL mepivacaine (no vasoconstrictor), injected 0.5 cm from lesion margin | — | Materials and Methods | FACT (procedure-level) / UNKNOWN (per-incision) |
| Measurement method | Histologic margin alteration measured in mm on H&E-stained sections, optical microscope (LEICA DM 2000, 5×/10×), quantified with Leica Application Suite v3.4 software; single-blind pathologist evaluation | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Diagnostic yield | Certainty diagnosis achieved in 17/17 specimens (100%); follow-up at 7 and 21 days showed complete wound recovery, no complications or pain | — | Results | FACT |
| Margin damage — mucocele, pooled (2 diode + 1 KTP) | 0.245 ± 0.162 | mm | Results (Table 1) | FACT |
| Margin damage — mucocele, diode-only (n=2: 0.442 mm, 0.102 mm) | 0.272 (mean of the 2 diode cases; individual values, not source-computed) | mm | Table 1 (per-patient) | FACT (individual values) / INTERPRETATION (diode-only mean, computed in this vault from the two individual diode values) |
| Margin damage — fibroma (5 diode, all diode) | 0.382 ± 0.149 (individual: 0.411, 0.357, 0.267, 0.623, 0.252 mm) | mm | Results (Table 2) | FACT |
| Margin damage — hyperkeratosis/squamous hyperplasia, pooled (3 diode + 1 KTP) | 0.336 ± 0.106 | mm | Results (Table 3) | FACT |
| Margin damage — hyperkeratosis, diode-only (n=3: 0.319, 0.446, 0.383 mm) | 0.383 (mean of the 3 diode cases; individual values, not source-computed) | mm | Table 3 (per-patient) | FACT (individual values) / INTERPRETATION (diode-only mean, computed in this vault) |
| Margin damage — oral lichen planus (3 diode, all diode) | 0.473 ± 0.105 (individual: 0.504, 0.356, 0.561 mm) | mm | Results (Table 4) | FACT |
| Margin damage — giant cell granuloma (1 diode) | 0.182 (SD not reported) | mm | Results | FACT |
| Margin damage — melanotic macula (1, diode 808 nm explicitly stated) | 0.149 (SD not reported) | mm | Results | FACT |
| Sample | 17 patients (8F/9M); lesion size 0.5–1 cm diameter; mostly excisional biopsies, some incisional depending on lesion site/size; device-per-lesion breakdown: mucocele 2 diode+1 KTP, fibroma 5 diode, hyperkeratosis 3 diode+1 KTP, oral lichen planus 3 diode, giant cell granuloma 1 diode, melanotic macula 1 diode | — | Materials and Methods | FACT |

## Notes

- FACT: Per-patient tables (Tables 1–4 of the source) give individual damage values with device attribution, allowing diode-only figures to be isolated for mucocele and hyperkeratosis (the two lesion types that mixed diode and KTP cases); this vault's mean-of-individual-values for those two diode-only subsets is an arithmetic computation performed here, not a value the source itself reports, and is flagged INTERPRETATION accordingly. Fibroma and oral lichen planus were diode-only in the source's own design, so their pooled means (0.382 mm, 0.473 mm) are already pure diode figures without recomputation.
- FACT: Greater inflammation/cellularity of the excised lesion (e.g., oral lichen planus, an inflammatory lesion) was associated with higher margin [[03 Concepts/Glossary/Thermal Damage|thermal-damage]] values than less-inflamed lesions (mucocele, melanotic macula), per the source's own interpretation — independent of device type per se.
- FACT: The source states many artifacts found on the samples were attributable to standard fixation/sectioning/staining processing, not to the laser itself.
- FACT: The source's own Discussion independently cites Angiero et al.'s 608-case retrospective (808 nm diode, 1.6–2.7 W CW, 320 μm fiber), reproducing the same "46.15%... in vivo diameter of at least 5 mm" figures now directly confirmed by this vault's own full-text extraction of Angiero et al. — see [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]]. This is Romeo et al.'s own citation of Angiero et al., not independent vault verification, but both sources now being full-text-processed in this vault increases confidence in both extractions.
- FACT: The Discussion also cites a different, earlier study by a different Romeo et al. group (not the present 2014 paper) — "Romeo et al. [13]" and "[14]" in this source's own reference list — comparing Er:YAG, Nd:YAG, Er-Cr:YSGG, and two diode wavelengths (808/980 nm) on pig tongue, reporting best results (<1 mm damage) with 808 nm diode in pulsed mode and higher-power Er,Cr:YSGG. This earlier study is not independently verified by this vault and must not be conflated with the present Romeo et al. 2014 paper.
- Classification for this vault: direct dental-diode biopsy diagnostic-yield and specimen-margin evidence — this vault's first source with an actual pathologist-rendered [[03 Concepts/Glossary/Diagnostic Quality|diagnosis]] outcome in a real human biopsy pathway, now with per-patient granularity. Relevant to [[04 Evidence/Biopsy Specimen Quality]] and [[04 Evidence/Surgical Margins]].
