---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: 808
set_power_w: [1.6, 2.7]
measured_power: false
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
needs_verification: false
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.1007/s10103-011-0900-7]]
- Source link: https://doi.org/10.1007/s10103-011-0900-7
- Source locator: Full text (Introduction; Materials and methods; Histopathology; Results; Discussion; Conclusions; Tables 1–5), retrieved from the attached PDF via the local Zotero library (zotero-key 946EPIDL). Upgraded from an earlier abstract-only extraction (no PMCID was available via PubMed's ID-conversion lookup).

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | 808 nm diode laser (DMT, Milan, Italy) | — | Materials and methods | FACT |
| Manufacturer | DMT, Milan, Italy | — | Materials and methods | FACT |
| Wavelength | 808 | nm | Materials and methods | FACT |
| Set power | 1.6–2.7 (range), average 2.5 | W | Materials and methods | FACT |
| Measured output power | UNKNOWN — no independent power-meter verification is reported; power values are set/console values | — | — | UNKNOWN |
| Average power | 2.5 (average of the 1.6–2.7 W range used across the series) | W | Materials and methods | FACT |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | Continuous wave (CW) | — | Materials and methods | FACT |
| Pulse duration | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Frequency | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Duty cycle | UNKNOWN (N/A, CW) | — | — | UNKNOWN |
| Fiber diameter | 320 | μm | Materials and methods | FACT |
| Tip type | UNKNOWN (optical fiber type/material not specified beyond diameter) | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN | — | — | UNKNOWN |
| Contact mode | UNKNOWN — not explicitly stated as contact or non-contact | — | — | UNKNOWN |
| Exposure duration | UNKNOWN as a per-incision time value; anesthesia protocol reported (topical or transmucosal local; 56.08% no anesthetic, 21.55% topical, 22.37% local) | — | Materials and methods | FACT (anesthesia only) / UNKNOWN (exposure time) |
| Measurement method | Histologic thermal-damage width measured as the distance from the specimen border to the end of visible thermal denaturation, at 100× magnification, on H&E-stained 4–5 μm sections; two pathologists evaluated separately, reaching agreement | — | Histopathology | FACT |
| Calibration method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable | — | — | UNKNOWN |
| Extent of thermal damage (width of modified tissue) | Range 260.7–321.4, mean 282.8 | μm | Results | FACT |
| Diagnostic yield — specimens 2 mm | 29/46 unreadable (63.63%) | % | Table 5 | FACT |
| Diagnostic yield — specimens 3 mm | 31/84 unreadable (37.71%) | % | Table 5 | FACT |
| Diagnostic yield — specimens 2–3 mm pooled | 60/130 unreadable (46.15%) — this is the source of the abstract's headline "46.15%" figure; the denominator (130 = 46 specimens sized 2 mm + 84 sized 3 mm) was not stated in the abstract and is resolved here from Table 5 | % | Table 5 | FACT |
| Diagnostic yield — specimens ≥4 mm | "A correct and reliable histopathological diagnosis was possible in all specimens of at least 4 mm in diameter" (0% unreadable) | — | Results | FACT |
| Unreadable specimens, whole series | 60 of 608 total (9.87%) | — | Table 2 (Histopathological diagnosis, "Unreadable specimen" row); cross-checked against Table 5's 60/130 for 2–3 mm specimens — consistent (all unreadable specimens fall within the 2–3 mm size classes) | FACT |
| Specimen size distribution | 2mm: 46 (7.57%); 3mm: 84 (13.81%); 4mm: 110 (18.10%); 5mm: 132 (21.72%); 6mm: 67 (11.02%); 7mm: 59 (9.70%); 8mm: 20 (3.30%); 9mm: 6 (0.98%); 10mm: 55 (9.04%); 11mm: 6 (0.98%); 12mm: 5 (0.82%); 13mm: 2 (0.33%); 15mm: 14 (2.30%); 26mm: 2 (0.33%) | mm / n / % | Table 4 | FACT |
| Recommended specimen size | ≥5 mm in vivo diameter (to allow for post-excision tissue shrinkage in addition to the ≥4 mm reliable-diagnosis threshold measured directly on paraffin-embedded specimens) | mm | Discussion | FACT |
| Connective tissue thermal-change descriptors | Carbonization; desiccation (expressed as dense eosinophilic layer) | — | Results | FACT |
| Vascular thermal-change descriptors | Intraluminal clotted erythrocytes; vascular stasis with gathered erythrocytes; thrombosed or collapsed blood/lymphatic vessels | — | Results | FACT |
| Epithelial thermal-change descriptors | Blisters, clefts, erosions, intraepithelial/subepithelial loss of attachment | — | Results | FACT |
| Biopsy technique criteria | Excisional biopsy when lesion benign or suspect but <5 mm diameter; incisional biopsy when lesion >5 mm or suspected malignant | — | Materials and methods | FACT |
| Sample | 608 surgical samples (269 men, 339 women; mean age 50.95 years), Department of Oral Pathology and Laser Therapy, Italian Stomatologic Institute, Milan, sent to S. Gerardo Hospital, Monza; Jan 2005–Apr 2010; one specimen per patient | — | Materials and methods; Table 1 | FACT |

## Notes

- FACT: The journal-issue year printed on the article header is 2012 (*Lasers Med Sci* 2012;27:383–388), while PubMed's indexed publication year is 2011 (online-first 9 March 2011). This vault continues to cite the source as "Angiero et al. 2011," consistent with prior references elsewhere in this vault and with PubMed's own indexed year; both years are preserved here rather than treated as an error.
- FACT: The abstract's "46.15%" figure, previously recorded as having an UNKNOWN denominator, is now resolved: it is 60 unreadable of 130 total specimens sized 2 mm or 3 mm combined (Table 5), not a threshold applied to "all specimens below 3 mm" as the abstract's phrasing might suggest in isolation. The full picture is size-graded: 63.63% unreadable at 2 mm, 37.71% at 3 mm, and 0% (fully readable) at ≥4 mm.
- FACT: The 60 "unreadable specimen" cases in the overall histopathological-diagnosis table (Table 2, out of 608) match exactly the 60 unreadable cases in the 2–3 mm size-stratified table (Table 5), confirming internal consistency — no unreadable specimens occurred at 4 mm or above.
- FACT: The source explicitly states that laser characteristics and settings — "power output, wavelength, emission modalities, type of optic fiber used, and affinity with target tissues" — can condition the width/severity of thermal damage, citing this as an established point in the literature (not a finding of the present study, which used one fixed protocol).
- INTERPRETATION (source's own): Reliable histological diagnosis for laser-excised specimens is a function of specimen size, not of the diode laser being fundamentally unsuitable for biopsy; the recommendation is to take a larger specimen (≥5 mm in vivo, accounting for shrinkage), not to avoid the diode laser.
- HYPOTHESIS: UNKNOWN.
- Classification for this vault: the largest-sample, now full-text-verified, direct dental-diode biopsy diagnostic-yield source in this vault; central to [[04 Evidence/Biopsy Specimen Quality]] and [[04 Evidence/Surgical Margins]]. Also the first vault source with a quantified thermal-damage-zone width (260.7–321.4 μm, mean 282.8 μm) paired with a real diagnostic-yield outcome — relevant to [[04 Evidence/Thermal Artifact]].
