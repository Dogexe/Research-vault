---
classification: "SUPPORTING TECHNICAL"
oral_tissue: true
ex_vivo: false
human_tissue: false
diode_laser: true
wavelength_nm: [450, 980]
set_power_w: [1.3, 1.5, 2.0, 4.0, 7.0]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: "unknown"
cw_pw: "CW+PW"
fiber_diameter_um: 600
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
margin_quality: null
tissue_architecture: "Qualitative comparison of collagen-fiber-bundle organization/disorganization and fibrotic tissue (Masson's trichrome) between groups at day 0 and day 7; 450 nm group showed less collagen disorganization and more organized granulation tissue at day 7 than 980 nm group. This is a wound-healing/repair-organization judgment, not a diagnostic tissue-architecture-preservation score."
specimen_interpretability: null
diagnostic_outcome: false
biopsy_oriented: false
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

## Source

- Literature note: [[02 Literature/10.3390/jcm15103567|Mazzoni et al. 2026]]
- Source link: https://doi.org/10.3390/jcm15103567
- Source locator: Full text (PDF, `pdftotext`; Table 1 device-parameter table extracted with column-reflow artifacts, cross-checked against prose) — Abstract; §2.1–2.5 (Materials and Methods); §3.1–3.2 (Results); §4 (Discussion); §5 (Conclusions); Table 1; Table 2.

## Study-design flag: two phases, only one has histology

This study has an **ex vivo screening phase** (Phase 1, porcine tongue, thermal measurement only, no histology, used only to select instruments/parameters) and an **in vivo primary-outcome phase** (Phase 2, Wistar rat, thermal + histology, day 0 and day 7). The `ex_vivo` field above is set to `false` because the paper's histologic and headline comparative findings — the data this note exists to extract — come from the in vivo phase; the ex vivo phase's own thermal data (Table 2) is recorded separately below and should not be read as ex vivo histologic evidence, since none exists in that phase.

## Special check: incision speed (per user instruction — verify, do not infer)

**No numeric incision speed, movement rate, or dwell time is stated anywhere in this paper, in either phase.** The Methods describe incision dimensions only ("The incision dimensions were standardized to approximately 1 mm in diameter and 1 mm in depth," §2.3) — a size, not a rate of movement. No mm/s, cm/s, or exposure-duration-in-seconds value is given for the incision itself. This is a confirmed absence from a full-text read, not an unresolved gap: `incision_speed_reported: false`.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Devices (final, in vivo) | Thera Lase Surgery™ (980 nm, DMC, São Carlos, Brazil); Thera BLU™ (450 nm, DMC, São Carlos, Brazil) | — | §2.1, §2.3 | FACT |
| Devices (ex vivo screening only, not carried to Phase 2) | D-Storm™ high-power infrared diode laser (Light Instruments) at multiple modes (2.0 W CW; 7.0 W long-pulse; 4 W/8 Hz superpulse); LiteTouch™ Er:YAG (Light Instruments), with and without air-water cooling; electrocautery; electric scalpel; Iris surgical scissors (control) | — | §2.2; Table 1; Table 2 | FACT |
| Manufacturer | DMC (São Carlos, Brazil) — final in vivo devices; Light Instruments (Yokneam, Israel) — Er:YAG and D-Storm ex vivo comparators | — | §2.1–2.2 | FACT |
| Wavelength | 450 (blue) and 980 (infrared), final in vivo arms; Er:YAG comparator 2940 nm (ex vivo only, excluded from in vivo phase) | nm | §2.1, §2.3; Table 1 | FACT |
| Set power (final, in vivo) | 980 nm: 1.3 W, pulsed, 20 Hz. 450 nm: 1.5 W, pulsed, 20 Hz | W | §2.1, §2.3 | FACT |
| Set power (ex vivo screening, additional diode arms not carried forward) | Thera Lase 980 nm CW: 2.0 W. D-Storm 980 nm CW: 2.0 W; long-pulse: 7.0 W; superpulse: 4 W/8 Hz. Thera BLU 450 nm CW: 1.5 W | W | Table 1; Table 2 | FACT |
| Measured output power (independent, reported value) | **NOT reported.** The Methods fully describe device settings (manufacturer/console W and Hz values) without describing any independent power-meter verification step anywhere in either phase. Per this vault's schema convention (a complete, fully-read Methods section that never mentions verification is recorded as `false`, not `null`), this is `measured_power: false` | — | §2.1–2.3 (absence, full-text read) | FACT (confirmed absence) |
| Average power | Same as set power (pulsed devices; average power not separately distinguished from the stated console value) | W | §2.1, §2.3 | FACT |
| Peak power | UNKNOWN — not reported for the diode devices | — | — | UNKNOWN |
| Operating mode | Pulsed, 20 Hz, for both final in vivo diode arms; ex vivo screening additionally tested CW, long-pulse, and superpulse modes for some diode devices (see above) | — | §2.1, §2.3; Table 1 | FACT |
| Pulse duration | UNKNOWN — not stated numerically for the final in vivo devices; Table 1 lists some duration/interval fields for other ex vivo instruments (e.g., Er:YAG 100–1000 ms range) that did not extract cleanly for the diode rows | — | Table 1 (partial, unclear) | UNKNOWN (diode pulse duration) |
| Frequency | 20 Hz, both final in vivo diode arms | Hz | §2.1, §2.3 | FACT |
| Duty cycle | UNKNOWN — not reported | — | — | UNKNOWN |
| Fiber diameter | 600 (Thera Lase and Thera BLU tips, per Table 1) | µm | Table 1 | FACT |
| Tip type | UNKNOWN beyond fiber diameter; no initiation status stated | — | — | UNKNOWN |
| Tip initiation status | UNKNOWN — not mentioned anywhere in the Methods | — | — | UNKNOWN |
| Contact mode | Contact mode, both final in vivo diode devices (per Table 1: "Contact mode" listed for Thera Lase and Thera BLU rows) | — | Table 1 | FACT |
| Exposure duration | UNKNOWN as a stand-alone value — incision described only by final dimensions (~1 mm diameter × 1 mm depth), not by time or rate | — | §2.3 | UNKNOWN |
| Incision / movement speed | **Not reported anywhere, in either phase.** No mm/s, cm/s, or any rate-of-movement value is given for any instrument. Incisions are static-dimension descriptions ("standardized to approximately 1 mm in diameter and 1 mm in depth"), not timed/rate-based | — | §2.3 (absence, full-text read) | FACT (confirmed absence) — **not a speed-effect study; speed is neither reported nor controlled as a variable** |
| Measurement method | Thermal: infrared thermography (Teledyne FLIR C5, with MSX technology), standardized camera distance and tray position. Histology (in vivo only): 10% formalin fixation, H&E staining (inflammatory infiltrate) and Masson's trichrome staining (collagen organization/fibrosis), examined at 40×/100×/400× total magnification (Opticam 0300S microscope), blinded examiner | — | §2.2–2.4 | FACT |
| Calibration method | UNKNOWN — no power-meter or thermography-camera calibration protocol described | — | — | UNKNOWN |
| Power loss / deviation | Not applicable — no independent power measurement was performed, so no set-vs-measured comparison exists | — | — | N/A |
| Sample / tissue model (Phase 1) | 60 ex vivo porcine tongues, lingual-frenulum-region incisions, 12 instrument/parameter groups | — | §2.1–2.2 | FACT |
| Sample / tissue model (Phase 2) | 30 prepubescent Wistar rats (22–30 days old, both sexes), lingual frenulum, 3 groups of n=10 (scissors, 980 nm diode, 450 nm diode); 5 animals/group euthanized at day 0, 5 at day 7 | — | §2.1, §2.3 | FACT |
| Thermal outcome (Phase 1, ex vivo screening) | Median temperature rise: scissors 5.9 °C (lowest); electrosurgical instruments 11.4–11.9 °C; diode lasers 8.4–14.0 °C (980 nm and 450 nm devices at the higher end). No instrument/setting exceeded the 40–42 °C threshold the authors cite as the onset of protein denaturation/irreversible thermal damage | °C | §3.1; Table 2 | FACT |
| Thermal outcome (Phase 2, in vivo) | Both 980 nm and 450 nm diode lasers caused significantly greater temperature increase than scissors; 450 nm showed a higher initial peak but faster cooling than 980 nm | °C | §3.2 | FACT |
| Histologic outcome, day 0 | 450 nm group: larger immediate zone of thermal coagulation near the incision, more structural damage (protein denaturation, collagen compaction). 980 nm group: smaller, more limited thermal-damage area with clearer preservation of nearby structures. Scissors group: hemorrhagic area, no thermal coagulation | — | §3.2 | FACT |
| Histologic outcome, day 7 | 450 nm group: less collagen-fiber disorganization, larger and more organized granulation-tissue healing area, described as closer to the scissors-control healing pattern. 980 nm group: smaller, more concentrated healing area, denser collagen deposition, thicker fibrotic scar | — | §3.2 | FACT |
| Macroscopic / clinical outcome | Both diode wavelengths achieved effective incision with adequate frenulum release and hemostasis; one animal had controlled bleeding in the 980 nm group. Scissors group had excessive intraoperative bleeding in 4/10 animals and no hemostatic effect | — | §3.2 | FACT |
| Diagnostic biopsy outcome | Not applicable — therapeutic ankyloglossia-release incision model, no lesion excised, no diagnosis rendered | — | — | N/A (by design) |
| Carbonization | Discussed narratively as a general risk in the Introduction ("excessive temperature increases leading to local tissue carbonization") but not scored or reported as an observed outcome in either phase | — | Introduction | UNKNOWN (as an observed outcome) |
| Coagulation zone | "Thermal coagulation" area described qualitatively at day 0 (larger for 450 nm, smaller for 980 nm) — not given a numeric measurement | — | §3.2 | FACT (qualitative) / UNKNOWN (no numeric value) |

## Notes

- FACT: This is a two-phase design where only the in vivo (rat) phase includes histology; the ex vivo (porcine) phase is thermal-screening only. Citing this source for "ex vivo oral histologic evidence" would be incorrect — the histology is in vivo (animal), not ex vivo.
- FACT, confirmed by full-text read per user instruction: **no incision speed, movement rate, or dwell time is reported anywhere in this paper.** This is a genuine absence, not an extraction gap — the incision is described only by final dimensions. Do not treat this source as speed-effect evidence in either direction, and do not infer a "slow"/"fast" incision technique from the absence of a stated rate.
- FACT: No independent power-meter verification is described for any instrument in either phase — all power/frequency values used in the Extraction table are device console/set values. Per the vault schema's convention for a fully-read, complete Methods section, this is recorded as `measured_power: false`.
- FACT: The paper's own safety framing is explicit and directly relevant to general parameter-safety context: none of the tested ex vivo instrument/power combinations raised local tissue temperature above the cited 40–42 °C injury threshold. This is a useful general safety data point but is not tied to any manufacturer preset, and does not by itself establish anything about this vault's specific preset-reliability question.
- FACT: The histologic outcome measured (inflammatory infiltrate, collagen organization/fibrosis, tracked to day 7) is a **wound-healing/tissue-repair** outcome, not this vault's biopsy-oriented **specimen-quality** outcome (margin readability, tissue-architecture preservation for diagnostic interpretation). Per user instruction, this note does not describe the thermal-damage or histology findings here as "specimen quality" — `specimen_interpretability` and `margin_quality` are both `null`, and `tissue_architecture` is populated with an explicit caveat distinguishing a healing-organization judgment from a diagnostic-architecture-preservation score.
- FACT: Reference [38] in this paper is Matys, Flieger & Dominiak 2017, "Effect of Diode Lasers with Wavelength of 445 and 980 nm on a Temperature Rise When Uncovering Implants for Second Stage Surgery: An Ex-Vivo Study in Pigs" — already in this vault as the acem/68943 source (cited in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] and the vault's dental-laser-safety search results). This paper cites that source in its Discussion as supporting context for wavelength-dependent thermal behavior.
- INTERPRETATION: None drawn beyond the source's own reported thermal/histologic comparisons.
- HYPOTHESIS: UNKNOWN — the authors state only that "further clinical studies are warranted to establish safe and effective parameters," not a specific testable hypothesis beyond the study's own comparative aim.
- NEEDS VERIFICATION: Table 1 (instrument parameter table) extracted from the source PDF with substantial column-reflow/merging artifacts; values used above were cross-checked against unambiguous prose statements in §2.1, §2.3, and §3.1–3.2 wherever possible, but a human should visually re-confirm Table 1 and Table 2 against the original PDF, particularly for the ex vivo-only instrument arms not carried into Phase 2.
- Classification for this vault: SUPPORTING TECHNICAL — oral-tissue, wavelength-controlled, in vivo (animal) thermal-and-healing comparison with an explicit safety-threshold framing, but no independently measured power, no incision speed reported at all, and a wound-healing (not biopsy-specimen-quality) histologic outcome. Relevant as general oral-tissue parameter-safety context for [[04 Evidence/Power Output and Tissue Effect]]; does not close this vault's incision-speed or biopsy-oriented-outcome gaps.

## Related notes

- Literature: [[02 Literature/10.3390/jcm15103567]]
- Distinct from (same first author, different paper, different devices — this paper uses Thera Lase/Thera BLU by DMC, not the [[05 Devices/Gemini Evo|Gemini Evo]] device): [[07 Data/Mazzoni et al 2026 - Neonatal Frenulum Laser Parameters]]
- Evidence: [[04 Evidence/Power Output and Tissue Effect]]
