# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/Phenomenon of laser power loss during curettage of infected periodontal pockets|Zegaib et al. 2011]]
- Source link: https://doi.org/10.1089/pho.2010.2911
- Source locator: Abstract; Materials and Methods; Figure 3; Table 1; Table 2; Table 3; Results; Discussion; Conclusions

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | 810-nm diode laser, Biolase, Irvine, CA; specific model number not given | — | Materials and Methods (Study group) | FACT |
| Manufacturer | Biolase (Irvine, CA) | — | Materials and Methods | FACT |
| Semiconductor composition | UNKNOWN for this specific unit (Discussion lists GaAlAs as typical of 810-nm diode lasers generally, but does not attribute this to the study device) | — | Discussion | UNKNOWN |
| Wavelength | 810 | nm | Abstract; Materials and Methods | FACT |
| Set power — treatment/irradiation | 1.7 | W CW | Abstract; Materials and Methods | FACT |
| Set power — standardized measurement setting | 1.0 | W CW | Abstract; Materials and Methods | FACT |
| Operating mode | Continuous wave (CW) | — | Abstract; Materials and Methods | FACT |
| Measured output power (absolute, at fiber tip, panel set to 1 W) | Study group (contact): 1st 0.91 W (SD 0.05, range 0.80–1.05); 2nd 0.72 W (SD 0.11, range 0.48–0.88); 3rd 0.63 W (SD 0.15, range 0.39–0.95); 4th 0.54 W (SD 0.14, range 0.33–0.76). Control group (non-contact): 1st 0.89 W (SD 0.07); 2nd 0.89 W (SD 0.07); 3rd 0.88 W (SD 0.07); 4th 0.88 W (SD 0.07) | W | Table 1 | FACT |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Pulse duration | UNKNOWN (device operated in CW mode) | — | — | UNKNOWN |
| Frequency | UNKNOWN | — | — | UNKNOWN |
| Duty cycle | UNKNOWN | — | — | UNKNOWN |
| Fiber diameter | 400 (study group, silica-glass fiber); control group fiber diameter not explicitly restated in text | μm | Materials and Methods | FACT (study group only) |
| Tip type | Silica-glass optical fiber; freshly cleaved tip; cleavage quality checked visually via aiming-beam spot shape (uniform circular spot = good cleavage) | — | Materials and Methods | FACT |
| Tip initiation status | UNKNOWN (paper does not use "initiated"/"non-initiated" terminology) | — | — | UNKNOWN |
| Contact mode | Study group: contact mode, fiber inserted into pocket 1 mm less than pocket depth. Control group: non-contact mode, no contact with teeth or gingival tissue | — | Materials and Methods | FACT |
| Exposure duration | 10 sec (anterior teeth) to 15 sec (posterior teeth) per application site; 40–60 sec total per tooth across 4 applications | sec | Materials and Methods | FACT |
| Cleaning/cleaving protocol | Study group: fiber tip cleaned of debris with saline-moistened gauze before each of the 4 PO measurements per tooth; freshly cleaved once per tooth, immediately after all 4 applications were completed. Control group: tip cleaved before each of the 28 irradiations (i.e., every irradiation) | — | Materials and Methods | FACT |
| Measurement method | Power meter (Molectron, Coherent Inc., Santa Clara, CA) measured PO at the fiber tip immediately prior to each laser application; panel reset to 1.0 W CW before each measurement, then raised to 1.7 W CW for the subsequent irradiation | — | Materials and Methods; Fig. 3 | FACT |
| Calibration method | UNKNOWN — power meter make/model is reported, but no calibration protocol, certificate, or traceability is described | — | — | UNKNOWN |
| Power loss — fiber transmission only, pre-contact | Mean 9% (control-panel 1.0 W setting vs. measured PO at 1st application, study group, before the tip touched tissue) | % | Discussion | FACT |
| Power loss — contact-induced, progressive (relative to 1st application) | Study group: 20.89% (1st→2nd), 30.39% (1st→3rd), 40.26% (1st→4th). Control group (non-contact): 0.14%, 0.54%, 1.58% respectively | % | Table 2; Abstract; Results | FACT |
| Power loss — panel setting vs. 4th-application tip PO, as stated by source | Source states "a mean PO loss of 54%... was found between the laser power set at the control panel and the PO measured at the fiber tip after the fourth laser application" | % | Results; Conclusions | FACT (verbatim source claim — see Notes for internal inconsistency) |
| Energy intensity (irradiance) | 0.724–1.2 | kW/cm² | Materials and Methods | FACT |
| Sample | 12 patients, 28 teeth (secondary analysis of a clinical trial originally enrolling 32 patients); 110 total PO measurements in study group (one tooth had only 2 measurements recorded); 112 total PO measurements in control group (28 irradiations × 4) | — | Materials and Methods | FACT |

## Notes

- FACT: The apparent 1.7 W vs. 1.0 W discrepancy is resolved by the full Methods text. These are not competing treatment powers: for each application, the control panel was set to 1.0 W CW immediately before the PO measurement at the fiber tip ("to facilitate mathematical analysis"), then raised to 1.7 W CW for the actual periodontal-pocket irradiation. The 1.0 W value is a standardized measurement reference, not the clinical treatment power.
- FACT / internal inconsistency flagged, not resolved: the source's own Results and Conclusions state a "mean PO loss of 54%" between the control-panel setting and the measured PO after the 4th application. Table 1 reports the mean measured PO at the 4th application (study group) as 0.54 W against the 1.0 W panel reference used for measurement, which arithmetically is a 46% loss (54% of power remaining), not a 54% loss. This vault preserves the source's stated figure verbatim rather than silently correcting it; the arithmetic mismatch is recorded as NEEDS VERIFICATION.
- INTERPRETATION (the source's own framing, not independently re-derived here): the small pre-contact fiber-transmission loss (9%) versus the much larger progressive loss with repeated contact applications (up to 40.26%) is attributed by the authors to tip fouling/debris from gingival tissue contact during curettage, not to intrinsic fiber transmission loss.
- HYPOTHESIS: UNKNOWN — the source proposes no formal hypothesis; it recommends frequent tip cleaving and rotation of application sites as practical mitigation (Conclusions/Summary), stated as a recommendation rather than a hypothesis to be tested.
- FACT: This is a secondary analysis of a previously conducted clinical trial (32 patients), using a 12-patient/28-tooth subset for the power-loss measurements reported here.
