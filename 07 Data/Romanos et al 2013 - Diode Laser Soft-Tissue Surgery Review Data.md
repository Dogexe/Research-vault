---
classification: "BACKGROUND"
oral_tissue: null
ex_vivo: null
human_tissue: null
diode_laser: true
wavelength_nm: null
set_power_w: 3
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: true
speed_mm_s: [12.5, 6.0, 3.0, 1.0, 0.0]
speed_control: mechanized
cw_pw: "CW"
fiber_diameter_um: null
tip_initiation: null
contact_mode: "contact"
histology: true
thermal_damage: true
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

- Literature note: [[02 Literature/Diode Laser Soft-Tissue Surgery_ Advancements Aimed at Consistent Cutting, Improved Clinical Outcomes]]
- Source link: UNKNOWN (no DOI given in the retrieved text; journal is *Compendium of Continuing Education in Dentistry*, published by AEGIS Communications)
- Source locator: Full text retrieved from the local Zotero PDF-text cache (`.zotero-ft-cache`, zotero-key EHPY3MPVg6669922). Romanos GE. "Diode Laser Soft-Tissue Surgery: Advancements Aimed at Consistent Cutting, Improved Clinical Outcomes." *Compendium of Continuing Education in Dentistry.* November/December 2013;34(10):752-758. Course validity stated in the source itself as "12/3/2013 to 12/31/2016."

## NEEDS VERIFICATION — naming discrepancy

The task that requested this extraction referred to this paper as "Romanos 2014." The retrieved full text is explicitly dated and paginated as the **November/December 2013** issue of *Compendium* (Volume 34, Number 10), with a CE-course validity window of "12/3/2013 to 12/31/2016," and the Zotero-attached PDF filename is "Romanos - 2013 - Diode Laser Soft-Tissue Surgery...". No 2014 publication date appears anywhere in the retrieved text. Per this vault's rule against inventing or assuming bibliographic data, this note and its literature-note counterpart use **2013**, the year stated by the source itself, and this discrepancy is flagged rather than silently resolved. This is a single-author continuing-education (CE) review article, not a primary study — it must not be confused with [[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data|Romeo et al. 2014]] (a different, multi-author primary study on KTP/diode oral biopsy already processed in this vault), nor with [[07 Data/Romanos et al 2022 - Initiated vs Non-Initiated Diode Laser Penetration Depth|Romanos et al. 2022]] (a different paper by an overlapping author, already in this vault).

## Scope note

This is a single-author CE review/perspective article on diode-laser soft-tissue surgery mechanisms, contrasted with a proprietary "Thermo-Optically Powered" (TOP) surgery technology. It is not a controlled primary study: no patient sample, no stated n, and no inferential statistics are reported anywhere in the retrieved text. Two illustrative comparisons with numeric values are presented (Figs. 5–6 and Figs. 7–8), but the source does not state a sample size, repetition count, or significance test for either. These are extracted below as the source's own reported values, explicitly flagged as illustrative/non-inferential.

## Extraction

| Parameter | Reported value | Unit | Source locator | Evidence status |
| --- | --- | --- | --- | --- |
| Device | "Standard diode laser" (fixed power, generic, unnamed) contrasted with "Thermo-Optically Powered (TOP) surgery" (a named proprietary technology; specific commercial product/manufacturer not stated in the retrieved text) | — | Throughout | FACT |
| Manufacturer | UNKNOWN (neither the generic diode comparator nor the TOP system is attributed to a named manufacturer in the retrieved text) | — | — | UNKNOWN |
| Wavelength | General near-infrared diode range stated as 800–1,100 nm; the TOP system's own source laser is described only as "a computer-controlled semiconductor laser," with no numeric wavelength value stated for it specifically in the retrieved text (elsewhere in the text, the tip's converted thermal-radiation output is stated to span 1,400–11,000 nm, which is a different, tip-emitted wavelength range, not the source laser's wavelength) | nm | Throughout | FACT (range only, not device-specific) |
| Set power | "Typically in the range of 2 W to 7 W" for commercially available diode dental lasers (a general statement, not a specific study setting); the Fig. 5/6 comparison specifies "fixed power (3 W CW)" for the conventional-diode arm; the TOP arm's own power value is not stated numerically (it is described as "automatic power control," varying to hold a preset tip temperature) | W | Throughout; Fig. 6 caption | FACT (general range + one specific fixed-power comparator value) |
| Measured output power | UNKNOWN — no power-meter-verified output value is reported anywhere in this source | — | — | UNKNOWN |
| Average power | Minimum average power needed for direct tissue cutting by light absorption alone, with a 400 μm tip, calculated/stated as approximately 25 W — far above the 2–7 W typical of commercial dental diode lasers, which the source uses to argue that standard diodes cannot cut by direct light absorption and instead rely on the [[03 Concepts/Glossary/Hot-tip Effect\|"hot-tip effect"]] (thermo-mechanical cutting via a carbonized, light-absorbing deposit at the fiber tip) | W | "Diode Laser Limitations" section | FACT (source's own stated calculation, not independently verified in this vault) |
| Peak power | UNKNOWN | — | — | UNKNOWN |
| Operating mode | CW implied for the "fixed power (3 W CW)" comparator in Figs. 5–6; TOP system uses automatic/variable power control rather than a fixed CW or pulsed setting | — | Fig. 6 caption | FACT |
| Pulse duration / frequency / duty cycle | UNKNOWN — not applicable to the CW comparator shown; not stated for any pulsed diode setting (this source does not test a pulsed diode arm) | — | — | UNKNOWN |
| Tip temperature (TOP system) | 500 °C to 900 °C, user-selectable within this range or via pre-programmed procedure-specific presets; illustrative images shown at 700 °C (Figs. 2–4) | °C | "Advances in Surgical Techniques" | FACT |
| Fiber diameter | 400 μm cited specifically in the "minimum average power for direct cutting" calculation above; not otherwise specified for the Fig. 5–8 comparisons | μm | "Diode Laser Limitations" | FACT (one specific citation only) |
| Tip type | TOP tip described as a quartz-glass fiber with sintered particles/ions integrated into the glass structure, engineered to convert monochromatic laser light into broadband thermal (polychromatic) radiation at the tip; average absorption coefficient of the tip's emitted radiation stated as 700–850 cm⁻¹, compared by the source to a CO2 laser's 630 cm⁻¹ | cm⁻¹ | "Advances in Surgical Techniques" | FACT |
| Tip initiation status | For **standard/conventional diode lasers** (not the TOP system): the source states manufacturers "now suggest initiating laser fibers using cork or articulating paper," but explicitly characterizes these as "non-standardized techniques" that "do not guarantee consistent initiation, nor does the initiation last longer than a few seconds while cutting tissue" — i.e., initiation is described as inherently unreliable for standard diodes, not as a fixed device state. The TOP system instead uses "a computer-controlled tip initiation process" described as "reproducibly" creating a defined 3-D tip shape, in-office, via a built-in initiation module — a categorically different, source-claimed-more-consistent initiation method. | — | "Diode Laser Limitations"; "Advances in Surgical Techniques" | FACT (source's own claims for both technologies; TOP's "reproducible" claim is not independently tested in this article with a stated method or data) |
| Contact mode | Contact (near-infrared diode/TOP systems both described as contact-cutting instruments, contrasted throughout with non-contact CO2/erbium lasers) | — | "Issues Regarding Non-Contact Vs. Contact Cutting" | FACT |
| [[03 Concepts/Glossary/Incision Speed\|Incision/advancement speed]] tested (Figs. 7–8 comparison) | 12.5, 6.0, 3.0, 1.0, and 0.0 mm/s (stop for several seconds; one 0.0 mm/s condition held for t=3 s specifically), applied to both a "traditional diode laser using fixed power" and "TOP surgery with automatic power control," using a translation stage with programmable speed and controlled vertical force | mm/s | "Connection Between Cutting Depth, Collateral Tissue Damage, and Speed of Cutting"; Figs. 7–8 | FACT |
| [[03 Concepts/Glossary/Incision Depth\|Cutting depth]] (Fig. 5–6 comparison, single illustrative example, no stated n) | TOP with automatic power control: 2.3 mm. Fixed power (3 W CW) conventional diode: 0.85 mm. | mm | Figs. 5–6 captions | FACT (single illustrative figure pair; no sample size or statistics given) |
| Coagulation depth (same Fig. 5–6 comparison) | TOP with automatic power control: 0.23 mm. Fixed power (3 W CW) conventional diode: 0.31 mm. | mm | Figs. 5–6 captions | FACT (single illustrative figure pair; no sample size or statistics given) |
| Thermal damage vs. speed (Figs. 7–8, NBTC viability staining) | Qualitative only, no μm values given in the retrieved text: "when the speed decreases, the cutting depth and level of collateral tissue damage and carbonization increase sharply for diode lasers, but they remain essentially the same with the new [TOP] laser technology." Method: nitro blue tetrazolium chloride (NBTC) viability staining (stained = live cells, white = dead cells), described by the source as "a standard tool to visualize tissue thermal damage in laser surgery." | — | "Connection Between Cutting Depth, Collateral Tissue Damage, and Speed of Cutting" | FACT (qualitative direction only; no numeric thermal-damage values reported for either technology at any tested speed) |
| Carbonization | Central mechanistic claim (not a measured outcome in this source): standard diode-laser cutting depends entirely on the "hot-tip effect" — an uninitiated or intermittently-initiated fiber tip carbonizes tissue protein at the point of contact, and this black carbonized deposit is what actually absorbs laser energy and heats the tip (to several hundred degrees), producing thermo-mechanical cutting; this deposit is continuously scraped away during cutting, causing fluctuating cutting/coagulation power. Per the Figs. 7–8 finding above, carbonization is stated to increase sharply with decreasing (standard diode) cutting speed. | — | "Diode Laser Limitations" | FACT (source's own mechanistic description; not independently quantified in this vault) |
| Coagulation zone | For standard heat-based contact cutting generally (electrosurgery, diode, CO2): described as occurring to "a depth of more than 200 μm," sealing blood/lymphatic vessels; hemostasis itself is stated to require "no more than 200 μm to 500 μm," so the source states that ≥1 mm of tissue coagulation (which it attributes to low cutting speed with snag/drag) constitutes "significant over-treatment." | μm | "Surgical Technique Challenges" | FACT (general/qualitative threshold statement, not a study-specific measured value) |
| Margin quality / diagnostic quality | N/A — this is a mechanism/technology review, not an oral-biopsy or specimen-diagnosis study; no lesion, no specimen, no pathologist diagnosis anywhere in the source | — | — | N/A |
| Measurement method | NBTC viability staining (Figs. 7–8, qualitative); no histologic thermal-damage quantification method with stated units is described for the Fig. 5–6 cutting/coagulation-depth comparison. | — | Various | FACT |
| [[03 Concepts/Glossary/Calibration\|Calibration]] method | UNKNOWN | — | — | UNKNOWN |
| Power loss / deviation | UNKNOWN / not applicable — no power-loss or set-vs-measured comparison is made anywhere in this source | — | — | UNKNOWN |

## Notes

- FACT: This source's central claim — "for standard diode lasers with fixed power, collateral tissue damage greatly depends on the speed of cutting... with low speed caused by a snag or drag, the extent of collateral damage can exceed 1 mm" (the snag/drag mechanism described is this vault's [[03 Concepts/Glossary/Hot-tip Effect|hot-tip effect]]) — is the most direct, explicit statement anywhere in this vault's processed literature that incision speed governs collateral [[03 Concepts/Glossary/Thermal Damage|thermal damage]] for a standard (non-proprietary) diode laser. It is presented with a supporting illustrative experiment (Figs. 7–8, five tested speeds from 12.5 to 0.0 mm/s), but the finding at those speeds is reported only qualitatively ("increase sharply"), with no numeric thermal-damage-width values, no stated sample size, and no significance test. This does **not** close this vault's standing incision-speed evidence gap (see [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]] §8) for oral-biopsy specimens — no lesion, no diagnosis, and no quantified damage value are reported — but it is the strongest *directional/mechanistic* statement on this exact question found in this vault's literature so far, and it directly corroborates, without quantifying, the general power/speed-dependent-damage pattern already noted qualitatively elsewhere in this vault.
- FACT: The Fig. 5–6 cutting-depth/coagulation-depth comparison (TOP: 2.3 mm cut / 0.23 mm coagulation vs. fixed-power diode: 0.85 mm cut / 0.31 mm coagulation) is a single illustrative example with no stated sample size or statistical test — it is recorded here as the source's own reported figures, not as validated comparative data, and should not be pooled with any of this vault's other margin/thermal-damage figures (which come from replicated, if still ex vivo or small-n, designs).
- FACT: This source explicitly discloses "no affiliation with any products mentioned in this article," but the entire article is structured around describing and favorably contrasting a single named proprietary technology (TOP surgery) against generic "standard diode lasers" — this is noted as a methodological/framing limitation, not as evidence the technical claims are false.
- FACT: The source's own reference list (ref. 2) cites Goharkhay K, Moritz A, Wilder-Smith P, et al. 1999 — the same [[07 Data/Goharkhay et al 1999 - Diode Laser Incision Depth and Collateral Damage Data|Goharkhay et al. 1999]] paper already independently processed in this vault. This is Romanos's own citation, not new corroboration performed by this vault, but it confirms both sources draw on the same foundational diode-tissue-interaction dataset.
- Classification for this vault: **BACKGROUND** — a non-empirical (or minimally empirical, illustrative-only) single-author CE review explaining diode-laser cutting mechanisms and a proprietary alternative technology; not an oral-biopsy study, not diode-specific primary data with a stated sample size, and not a source that can be pooled with this vault's quantified thermal-damage or diagnostic-yield figures. Relevant only as directional/mechanistic context for [[06 Synthesis/Diode Laser Biopsy Pre-setting Map]]'s incision-speed discussion and for [[03 Concepts/Glossary/Incision Speed]] and [[03 Concepts/Glossary/Initiated Tip]] / [[03 Concepts/Glossary/Non-initiated Tip]].
- METADATA CONVENTION / BOUNDARY CASES: `oral_tissue`, `ex_vivo`, and `human_tissue` are recorded `null`, not `false` — this is a review with no stated tissue sample, species, or n for its illustrative Figs. 5–8 comparisons, so these properties are genuinely indeterminate rather than confirmed absent. `fiber_diameter_um` and `tip_initiation` are `null` for the same reason: a 400 μm fiber and standard-diode initiation practices are discussed elsewhere in the review's general background, but neither is confirmed to be the specific setup used for the Figs. 5–8/7–8 illustrative comparisons. `speed_mm_s: [12.5, 6.0, 3.0, 1.0, 0.0]` — the source explicitly reports this 5-point tested speed sweep via a programmable translation stage (hence `speed_control: mechanized`); recorded as a list per the schema v1.1 widening of `speed_mm_s` to accept a list of discrete tested values, matching its sibling numeric fields (see [[99 Templates/Study Metadata Schema]]). **This remains illustrative data from a single-author review, not primary-study evidence** — no stated sample size, repetition count, or significance test accompanies the sweep (see the Scope note above); the list captures the reported values faithfully, it does not upgrade their evidentiary weight.
