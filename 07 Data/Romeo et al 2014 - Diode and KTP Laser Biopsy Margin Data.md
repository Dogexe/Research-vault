# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/Romeo et al 2014 - Biopsy of Oral Soft Tissue Lesions by KTP and Diode Laser]]
- Source link: https://doi.org/10.1155/2014/761704
- Source locator: Materials and Methods; Results; Discussion

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | Diode laser (SOL, DenMat Italia, Italy); KTP laser (SmartLite, DEKA, Italy) | — | Materials and Methods | FACT |
| Manufacturer | DenMat Italia (diode); DEKA (KTP) | — | Materials and Methods | FACT |
| Wavelength | Diode: 808; KTP: 532 | nm | Materials and Methods | FACT |
| Set power | Diode: 2 W CW; KTP: 1.5 W PW | W | Materials and Methods | FACT |
| Measured output power | UNKNOWN — set/console values only; no independent power-meter verification reported | — | — | UNKNOWN |
| Average power | UNKNOWN (fluence reported instead — see below) | — | — | UNKNOWN |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Diode: continuous wave (CW); KTP: pulsed wave (PW) | — | Materials and Methods | FACT |
| Pulse duration | UNKNOWN | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fluence | Diode: 2400 J/cm²; KTP: 212 J/cm² | J/cm² | Materials and Methods | FACT |
| Fiber diameter (spot size) | Diode: 320; KTP: 300 | μm | Materials and Methods | FACT |
| Tip type | UNKNOWN | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN (not mentioned) | — | — | UNKNOWN |
| Contact mode | UNKNOWN — not explicitly stated as contact or non-contact in the retrieved text | — | — | UNKNOWN |
| Exposure duration | UNKNOWN as a per-incision value; overall surgical intervention constrained to ≤5 minutes for patient compliance | sec/min | Materials and Methods | FACT (procedure-level only) / UNKNOWN (per-incision) |
| Measurement method | Histologic margin alteration measured in mm on H&E-stained sections, optical microscope (LEICA DM 2000, 5x/10x magnification), quantified with Leica Application Suite v3.4 software; single-blind pathologist evaluation | — | Materials and Methods | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Diagnostic yield | Certainty diagnosis achieved in 17/17 specimens (100%) | — | Results | FACT |
| Margin damage — mucocele | 0.245 ± 0.162 (n=3: 2 diode + 1 KTP, pooled) | mm | Results | FACT |
| Margin damage — fibroma | 0.382 ± 0.149 (n=5, diode only) | mm | Results | FACT |
| Margin damage — hyperkeratosis / squamous hyperplasia | 0.336 ± 0.106 (n=4: 3 diode + 1 KTP, pooled) | mm | Results | FACT |
| Margin damage — oral lichen planus | 0.473 ± 0.105 (n=3, diode only) | mm | Results | FACT |
| Margin damage — giant cell granuloma | 0.182 (n=1, diode only; SD not reported) | mm | Results | FACT |
| Margin damage — melanotic macula | 0.149 (n=1, diode 808 nm explicitly stated; SD not reported) | mm | Results | FACT |
| Sample | 17 patients (8F/9M); lesion size 0.5–1 cm diameter; mostly excisional biopsies, some incisional depending on lesion site/size | — | Materials and Methods | FACT |

## Notes

- FACT: Except for melanotic macula (explicitly attributed to the 808 nm diode), the mucocele and hyperkeratosis/squamous-hyperplasia margin-damage values are pooled across whichever device (diode or KTP) treated that lesion type — the source's Methods states 2 mucoceles by diode + 1 by KTP, and 3 hyperkeratosis lesions by diode + 1 by KTP — so these two rows are not a clean single-device measurement. Fibroma, oral lichen planus, giant cell granuloma, and melanotic macula were diode-only per the Methods.
- FACT: Greater inflammation/cellularity of the excised lesion (e.g., oral lichen planus, an inflammatory lesion) was associated with higher margin thermal-damage values than less-inflamed lesions (mucocele, melanotic macula), per the source's own interpretation — independent of device type per se.
- FACT: The source states many artifacts found on the samples were attributable to standard fixation/sectioning/staining processing, not to the laser itself.
- FACT: The source's own Discussion independently cites Angiero et al. 2011's 608-case retrospective (808 nm diode, 1.6–2.7 W CW, 320 μm fiber), reproducing the same "46.15%... not achievable" figure below 3 mm specimen size and the ≥5 mm specimen-size recommendation that this vault separately retrieved from Angiero et al.'s own abstract (see [[07 Data/Angiero et al 2011 - Diode Laser Biopsy Specimen Size and Diagnostic Yield]]). This is Romeo et al.'s own citation of Angiero et al., not independent vault verification of Angiero et al.'s primary data — but the two independently sourced figures match, which increases confidence in this vault's Angiero extraction.
- FACT: The Discussion also cites a different, earlier study by a different Romeo et al. group (not the present 2014 paper), comparing Er:YAG, Nd:YAG, Er,Cr:YSGG, and two diode wavelengths (808/980 nm) on pig tongue, reporting best results (<1 mm damage) with 808 nm diode in pulsed mode and higher-power Er,Cr:YSGG. This earlier study is not independently verified by this vault and must not be conflated with the present Romeo et al. 2014 paper.
- Classification for this vault: direct dental-diode biopsy diagnostic-yield and specimen-margin evidence — this vault's first source with an actual pathologist-rendered diagnosis outcome in a real human biopsy pathway. Relevant to [[04 Evidence/Biopsy Specimen Quality]] and [[04 Evidence/Surgical Margins]].
