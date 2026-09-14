---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: false
wavelength_nm: 1064
set_power_w: [3.5, 5]
measured_power: false
measured_power_value_reported: false
measured_power_w: null
power_meter: null
measurement_location: null
incision_speed_reported: false
speed_mm_s: null
speed_control: unknown
cw_pw: "PW"
fiber_diameter_um: 320
tip_initiation: null
contact_mode: null
histology: true
thermal_damage: true
margin_quality: "quantified (overall width of tissue injury, μm, by compartment and group) + ordinal incision-quality score (0–4, 4=best); Group 1 (3.5W/60Hz): epithelial 305.8, stromal 376.6, vascular 151.6 μm, incision score 1.5. Group 2 (5W/30Hz): epithelial 399.8, stromal 521, vascular 183.5 μm, incision score 1.4. Scalpel: 0 μm all compartments, incision score 4"
tissue_architecture: "categorical presence/absence (nuclear changes, cytoplasmic changes, loss of attachment, carbonization, desiccation, vascular thrombosis/stasis), by group, with a stated 10% cut-off threshold for the whole resection margin"
specimen_interpretability: null
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: CORE BIOPSY — NOT a diode laser.** Nd:YAG is a solid-state laser; `diode_laser: false` is deliberate and confirmed. This is the **source paper whose histologic evaluation criteria were explicitly adopted by [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data|Monteiro et al. 2019]]** (confirmed by Monteiro's own text: "evaluated... according the criteria established by Vescovi et al."). Its central finding — that small specimens (<7 mm) show markedly greater thermal artifact regardless of laser settings — is the strongest specimen-size precedent in this vault outside Angiero et al. 2011.

## Source

- Literature note: [[02 Literature/10.1007/s10103-010-0770-4]]
- Source link: https://doi.org/10.1007/s10103-010-0770-4
- Source locator: Full text (cached plain-text extraction, `.zotero-ft-cache`) — Abstract; Introduction; Material and methods; Figs. 1–6; Tables 1–6; Results; Discussion; Conclusions.

## Extraction

| Parameter | Group 1 (Nd:YAG, 3.5W/60Hz) | Group 2 (Nd:YAG, 5W/30Hz) | Group 3 (Bard-Parker scalpel #15c) | Evidence status |
| --- | --- | --- | --- | --- |
| n | 6 | 9 | 11 | FACT |
| Wavelength | 1064 nm | 1064 nm | N/A | FACT |
| Output power | 3.5 W | 5 W | N/A | FACT |
| Frequency | 60 Hz | 30 Hz | N/A | FACT |
| Power density | 488,281 W/cm² | 300,000 W/cm² | N/A | FACT |
| Fiber diameter | 320 μm | 320 μm | N/A | FACT |
| Pulse width | 100 μs ("very short pulse," VSP) — device-level, applies to both groups | (same) | N/A | FACT |
| Device basis | Flashlamp-pumped | (same) | N/A | FACT |
| Contact mode | UNKNOWN — not explicitly stated for either laser group | UNKNOWN | N/A | UNKNOWN |
| Tip initiation status | UNKNOWN — not addressed | UNKNOWN | N/A | UNKNOWN |
| Independently measured power | NO — output power/frequency are reported as the device operating settings; no power meter or independent verification instrument is described anywhere in Methods | NO | N/A | FACT (absence confirmed) |
| Incision speed | NOT REPORTED — no mm/s value or control description for either group | NOT REPORTED | N/A | UNKNOWN |
| Sample / lesion | Benign fibro-epithelial oral lesions (denture-induced fibrous hyperplasia, fibroma, fibropapilloma), cheek/buccal mucosa; mean specimen size 10.5 mm | (same lesion types) mean specimen size 8.12 mm | (same lesion types) mean specimen size 8 mm | FACT |
| Nuclear changes (Yes/No) | 6/0 | 8/0 | 0/11 | FACT |
| Cytoplasm changes (Yes/No) | 5/1 | 7/1 | 0/11 | FACT |
| Loss of attachment (Yes/No) | 5/1 | 5/3 | 0/11 | FACT |
| Overall epithelial changes present | 6/6 | 9/9 | 0/11 | FACT |
| Stromal (connective-tissue) changes present | 6/6 | 8/8 (of the 8 with data reported — see source Table 3) | 0/11 | FACT |
| Vascular thrombosis (Yes/No) | 4/2 | 4/4 | 0/11 | FACT |
| Vascular stasis (Yes/No) | 2/4 | 3/5 | 1/10 | FACT |
| Incision regularity (Yes/No) | Not separately tabulated as Yes/No for group 1/2 in the extracted text; incision **quality score** is the operative metric (below) | — | — | FACT (score) |
| Incision quality score (0–4, 4=highest) | 1.5 | 1.4 | 4 | FACT — "an overall quality score (ranging 0–4) was assigned to each incision, score '4' representing the highest quality" |
| Epithelial width of injury (μm) | 305.8 | 399.8 | 0 | FACT |
| Stromal (connective) width of injury (μm) | 376.6 | 521 | 0 | FACT |
| Vascular width of injury (μm) | 151.6 | 183.5 | 0 | FACT |
| Epithelial changes, samples <7mm | / (group 1 had no <7mm samples reported) | 567.5 μm | 0 | FACT |
| Epithelial changes, samples >7mm | 305.8 μm | 232.5 μm | 0 | FACT |
| Histological diagnosis affected | No, for any group — "thermal artifacts did not limit the histologic diagnosis and accuracy of resection margins evaluation" | No | No | FACT |

## Study design (per task's Section A)

- Human, in vivo, prospective (Unit of Oral Pathology and Oral Laser-assisted Surgery, University of Parma, Italy; May 2007–May 2008). NOT ex vivo.
- **True diagnostic/excisional biopsy pathway**: real benign fibro-epithelial lesions, histopathological diagnosis rendered per case.
- Comparator groups: 2 Nd:YAG arms (differing power/frequency) + 1 cold-scalpel arm. **This is a small, explicitly "preliminary" study** (title: "A preliminary histological analysis").
- Sample size: n=26 total (6/9/11) — the smallest per-arm sample size of the four sources processed in this phase.
- Tissue/site: cheek and buccal mucosa only (both same subsite across all groups, a deliberate control for anatomic-site variability).
- Specimen size range 3–14 mm (mean 8.58 mm); explicit **<7mm vs. ≥7mm** size stratification is the paper's own analytic variable.

## Histopathology methodology (per task's Section C)

- Fixation: 10% buffered formalin; paraffin-embedded; 5 μm sections, H&E stain.
- **Pathologist involvement: one pathologist**, explicitly stated **"unaware of the excision method"** (i.e., blinded).
- **Number of assessors: 1.** NOT a multi-pathologist consensus design.
- **Consensus process: N/A** (single assessor).
- **Inter-rater reliability: NOT REPORTED.**
- Magnification: 40× and 100× (low- and high-power light microscopy, Nikon Labophot); tissue-injury width measured with an ocular micrometer (Olympus BX 51).
- Explicit measurement protocol: epithelial changes evaluated "from the edge of the margin to a depth of 1,000 μm," connective-tissue changes likewise to 1,000 μm depth, with a stated **10% cut-off** threshold of altered tissue in the whole resection margin used to call a compartment "affected."

## Outcome terminology (author's exact wording, per task's Section D)

- **"Epithelial changes"**, **"connective tissue modifications"** (also called "stromal changes" in Results/Tables — the paper itself uses both terms interchangeably for the same construct; this vault preserves both as the source's own wording rather than picking one), **"vascular modifications."**
- **"Incision morphology"**, subclassified regular/irregular, and an **"overall quality score (0–4)"**, "4" = highest quality.
- **"Overall width of tissue modifications"** — the paper's own phrase for the μm measurement (not given a named abbreviation, unlike Monteiro's "TDE").
- No "pseudodysplastic" or artifact-specific terminology is used in this paper (contrast with Seoane 2013/González-Mosquera 2011's vocabulary) — the paper frames its findings purely as "thermal artifacts" / "tissue modifications," not as dysplasia-mimicking artifacts specifically.

## Outcome type (per task's Section E)

| Outcome | Type | Unit/range | Epithelial component? | CT component? | Margin-specific? | Architecture-specific? | Diagnosis affected? | Adequacy/readability judgment? |
|---|---|---|---|---|---|---|---|---|
| Width of tissue injury | Quantitative continuous | μm, by compartment (epithelial/stromal/vascular) and group | Yes | Yes | Yes | No | No | No |
| Nuclear/cytoplasmic/attachment-loss, carbonization/desiccation, vascular thrombosis/stasis | Binary (presence/absence, 10% cut-off rule) | Yes/No, per sub-item, per group | Yes | Yes | No | Yes | No | No |
| Incision quality score | Ordinal | 0–4, 4=best | No | No | Yes (edge regularity) | No | No | Yes (incision-quality proxy) |
| "No limitation of diagnosis / accuracy of resection margin evaluation" | Binary, whole-cohort conclusion | Yes/No | — | — | — | — | Yes | Yes |

## Score/grading details (per task's Section F)

- **Incision quality score (0–4, 4=highest)**: created in this paper. This is the paper Monteiro et al. 2019 later reused (as its own "regularity of incision" 0–4 score) and that the Tenore et al. 2023 systematic review (already known to this vault, secondary source) calls the "incision damage morphology score" shared across several of its 28 included studies. **This paper is therefore the likely origin point of that cross-study score**, though this vault has not independently verified an even-earlier original source — flagged NEEDS VERIFICATION.
- Validation status: NOT stated as validated; no inter-rater reliability given (single, blinded assessor).
- Blinded scoring: YES (one pathologist, unaware of excision method).
- Number of scorers: 1.
- Reliability statistic: NOT REPORTED.

## Specimen size effect (task's specific focus for this source)

- FACT: **"Epithelial and stromal changes were significantly more frequent in specimens with a mean size less than 7 mm (p<0.0001)"** — the paper's own headline size-effect finding, independent of laser power/frequency settings used.
- FACT: "The Nd:YAG laser induces serious thermal effects in small specimens (mean size less than 7 mm) independently from the frequency and power employed" — explicitly generalized across both laser arms.
- FACT: Vascular-change differences by size were only "quite significant" (Fisher's exact p=0.0827; Chi-square p=0.0832) — weaker than the epithelial/stromal effect, and explicitly reported as such rather than rounded up to "significant."
- INTERPRETATION (the paper's own, not this vault's addition): the authors distinguish thermal-artifact magnitude from diagnostic adequacy — despite the strong size-dependent thermal-artifact effect, the Conclusions state "thermal artifacts did not limit the histopathological diagnosis in any case," i.e., **greater measured thermal damage in small specimens did not, in this study, translate into a diagnosis-affected outcome.** This is the same dissociation-between-constructs pattern independently observed in Gobbo et al. 2017 (this phase) and already present in this vault's Gambino et al. 2026 extraction.

## Notes

- FACT: This is the vault's **source-of-record for the "criteria established by Vescovi et al."** cited verbatim by Monteiro et al. 2019 — a confirmed, not inferred, methodological lineage between two of this phase's four primary extractions.
- FACT: Smallest per-arm sample size of this phase's four new sources (n=6/9/11) — explicitly self-described as "preliminary."
- FACT: Independently measures no power and reports no incision speed — does not close this project's core measured-power + speed gap; strengthens only the specimen-size / outcome-methodology side.
- NEEDS VERIFICATION flagged in YAML: (1) `set_power_w: [3.5, 5]` records the two tested discrete Nd:YAG settings as a list, per schema convention for "discrete list only where the source itself enumerates fixed variants"; (2) `contact_mode: null` and `tip_initiation: null` — neither is addressed anywhere in the text for either Nd:YAG group, confirmed absence rather than oversight; (3) the origin-point claim for the 0–4 incision-quality score (i.e., whether this paper itself is the first published use, or itself reused it from an earlier uncited source) is NOT independently verified — this vault only confirms that Monteiro 2019 explicitly reused *this* paper's criteria, not that this paper is the ultimate origin.
- Classification for this vault: CORE BIOPSY, non-diode. Strengthens the specimen-size and cross-study methodological-lineage precedent materially; does not touch the diode-specific, measured-power, or incision-speed axes.

## สรุปภาษาไทย

- การศึกษานี้เปรียบเทียบเลเซอร์ Nd:YAG (2 ค่ากำลัง/ความถี่) กับใบมีดผ่าตัดในผู้ป่วยจริง 26 ราย (รอยโรค fibro-epithelial hyperplasia) มีพยาธิแพทย์ 1 คนที่ไม่ทราบวิธีตัด (blinded) ประเมินผล
- **พบว่าชิ้นเนื้อขนาดเล็กกว่า 7 มม. มีการเปลี่ยนแปลงทางเยื่อบุผิวและชั้นใต้เยื่อบุผิวมากกว่าอย่างมีนัยสำคัญ (p<0.0001) โดยไม่ขึ้นกับค่ากำลัง/ความถี่ที่ใช้**
- แม้จะพบความเสียหายจากความร้อนที่ชัดเจนในชิ้นเนื้อเล็ก แต่**ไม่มีกรณีใดที่การวินิจฉัยทางพยาธิวิทยาถูกจำกัดจากความเสียหายนี้**
- บทความนี้เป็น**ต้นแบบของเกณฑ์การประเมินทางจุลพยาธิวิทยา**ที่ Monteiro et al. 2019 นำไปใช้ต่อโดยตรง (ยืนยันจากข้อความในบทความของ Monteiro เอง)
- ไม่มีการวัดกำลังขาออกจริง และไม่มีการรายงานความเร็วตัด

## Related notes

- Literature: [[02 Literature/10.1007/s10103-010-0770-4]]
- Data: [[07 Data/Monteiro et al 2019 - Multi-Instrument Oral Fibro-Epithelial Margin Histology Data]] (directly reuses this paper's evaluation criteria)
- Evidence: [[04 Evidence/Biopsy Specimen Quality]]
- Synthesis: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
- Project: [[01 Projects/Diode Laser Biopsy]]
