# Tenore et al. 2023 — Laser Thermal Effect on Oral Soft Tissue Biopsy Histology: Systematic Review Data

**SECONDARY SOURCE ONLY — NOT a primary study. No schema v1.1 YAML is applied to this note**, per [[99 Templates/Study Metadata Schema]] (schema fields describe primary-study extractions) and per explicit instruction for this phase. This note follows the same secondary-source convention already established in this vault by [[07 Data/Lopes-Santos et al 2023 - High-Power Laser Oral Biopsy Histology Systematic Review Data|Lopes-Santos et al. 2023]] (also untagged). Record values exactly as reported by the review; do not promote its summary claims into primary-study metadata for any individual included study.

## Source

- Literature note: [[02 Literature/10.3390/dj11020028]]
- Citation: Tenore G, et al. "The Impact of Laser Thermal Effect on Histological Evaluation of Oral Soft Tissue Biopsy: Systematic Review." *Dent J (Basel)*. 2023;11(2):28. [DOI](https://doi.org/10.3390/dj11020028)
- Source locator: Full text, open access, PMC9955047 — Introduction; Materials and Methods; Results (§3.1 Animal studies, §3.2 Clinical studies, §3.3 Laser parameters); Discussion; Conclusions.

## Review-level extraction

| Parameter | Reported value | Evidence status |
| --- | --- | --- |
| Review type | Systematic review (narrative synthesis; no meta-analysis performed) | FACT |
| Reporting standard | PRISMA | FACT |
| Registration | PROSPERO CRD42022385059 | FACT |
| Focus question | "What is the impact of the thermal effect of different laser wavelengths on the histological evaluation of laser-collected oral biopsy?" | FACT |
| Databases searched | PubMed, Scopus | FACT |
| Search date range | July 2020 – November 2022 | FACT |
| Screening | Two independent reviewers (A.M., A.N.), two stages (title/abstract, then full text); third reviewer (G.T.) arbitrated disagreements | FACT |
| Risk-of-bias tools | SYRCLE (animal studies); MINORS (clinical studies) | FACT |
| Studies identified | PubMed 119, Scopus 1433 (1987–2022) → 152 after dedup → 28 included (23 from database search + 5 from manual reference/citation-list search) | FACT |
| Included study split | 14 animal studies, 14 clinical studies | FACT |
| Total animal samples | 607 | FACT |
| Total clinical specimens | 1117 (941 with histopathological diagnosis explicitly reported; 176 not clearly identified in 4 studies) | FACT |
| Wavelengths considered (review's own inclusion scope) | KTP 532 nm; diode 445, 808, 940–980 nm; Nd:YAG 1064 nm; Er,Cr:YSGG 2780 nm; Er:YAG 2940 nm; CO2 | FACT |
| Most-studied laser | CO2 (12 studies: 5 animal + 7 clinical), followed by diode 940–980 nm (8 studies) | FACT |
| Least-studied laser | KTP (3 studies) | FACT |

## Outcome terminology and scoring systems named in the review (citation-mined, not vault-original)

Preserved exactly as the review attributes them — **none of these attributions has been independently verified against the cited paper's own full text by this vault except where a dedicated primary 07 Data note already exists** (marked below).

| Named metric/score | Attributed source (per review) | Definition (per review) | Already a primary 07 Data note in this vault? |
| --- | --- | --- | --- |
| Thermal Damage Score (TDS) | Romeo et al. | Ordinal 0–3 (0 "no damage," 1 "little damage," 2 "moderate damage," 3 "severe damage") | Romeo et al. 2014 is in vault ([[07 Data/Romeo et al 2014 - Diode and KTP Laser Biopsy Margin Data]]) — whether that note's own extraction independently confirms the "TDS" name/definition has NOT been re-verified in this phase; flagged for a future check, not silently assumed |
| Cut-quality score (0–5, 5=highest, cold-blade reference) | Fornaini et al. | 0–5 ordinal | NOT in vault as a primary source |
| Cercadillo-Ibarguren macroscopic grading scale (0–4) | Cercadillo-Ibarguren et al. | Macroscopic hyalinization/coagulation grading | NOT in vault as a primary source (identified as a retrieval-priority candidate in Phase 4) |
| Maximum Denaturation Depth (MDD) / Denaturation Area (DA) | Braun et al. | Quantitative μm/mm² | NOT in vault as a primary source |
| Thermal Damage Depth (TDD) / Thermal Damage Area (TDA) | Prado et al. | Quantitative μm/mm²; TDA = total specimen area minus thermal-damage area | **Already in vault**, [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data]] — this review's citation is consistent with, and cross-confirms, that note's own extracted terminology |
| Thermal Damage Zone (TDZ), max/min/mean/median | Suter et al.; Gill et al. | Quantitative μm | Suter et al. 2010 is in vault at abstract-level only ([[07 Data/Suter et al 2010 - CO2 vs Diode Laser Biopsy Thermal Damage Data (Abstract-Level)]]); the review's own text distinguishes at least three separate Suter et al. papers (2010, 2014, 2017 per its reference list context) — **this vault's existing Suter 2010 note should not be assumed to be the same "Suter et al." cited for TDZ without a direct check**, flagged as an unresolved ambiguity (see Step 12 below) |
| "Distance from edges of specimen to thermal artifacts" | Matsumoto et al. | Quantitative μm | NOT in vault as a primary source |
| Maximum thermal damage along cutting margin | Gobbo et al. | Quantitative μm | **Now in vault**, this phase — [[07 Data/Gobbo et al 2017 - Blue vs Infrared Diode Laser Biopsy Thermal Damage Data]]. This review's own text ("Gobbo et al. quantified the maximum thermal damage along the cutting margin") matches this vault's independent full-text extraction of the same paper exactly — a genuine cross-confirmation. |

## Wavelength-specific synthesis (review's own narrative, preserved as reported)

- **808 nm diode** (6 studies: 3 clinical + 3 animal): tested power 1–3 W; reported thermal effect range 17.92–473 μm (clinical, similar parameters); "all the studies suggested that the 808 nm laser can be considered an affordable tool and confirm the possibility of having a clear histological diagnosis," but margin extension was also recommended; one study recommended lesions >3 mm diameter, reporting diagnosis "not achievable" in 46.15% of smaller specimens — **this specific 46.15% figure and its source study were NOT independently identified or verified by this vault in this phase** (the review's own in-text citation markers were stripped in the full-text extraction available to this vault); flagged as an unresolved ambiguity, not attributed to any specific vault-known study (see Step 12).
- **940–980 nm diode** (8 studies): thermal effect range 100–1198.54 μm across 5 studies reporting it; "all the studies stated that diode laser 940–980 nm laser did not hinder the histological evaluation."
- **445 nm diode** (6 studies): "all the included six studies... reported the best quality of cut and minimal thermal effect in comparison with others."
- **Nd:YAG** (6 studies): tested power 1–6 W, all pulsed; "the extent of the thermal effect with Nd:YAG was the highest when compared to other lasers," and cites Vescovi et al.'s finding of serious thermal effects in specimens <7 mm — **this is the review's own independent citation of the same Vescovi et al. 2010 finding this vault extracted directly from the primary paper this phase** ([[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data]]), a genuine cross-confirmation.
- **Er,Cr:YSGG** (4 studies): "the reported extent of thermal effect was quite small with all tested powers."
- **KTP** (3 studies): "demonstrated a low thermal effect on soft tissues."
- **Er:YAG** (6 studies): "almost all of them showed that it is a conservative tool"; least thermal effect of all compared lasers where head-to-head comparisons existed.
- **CO2** (12 studies, most-studied): "all the studies confirmed that it is a reliable tool"; one study "reported produced epithelial damage for both low- and high-tested powers (3 W to 12 W) similar to light dysplasia features that could cause erroneous therapy" — a direct match to the "pseudodysplastic artifact" construct this vault newly extracted this phase from Seoane et al. 2013 and González-Mosquera et al. 2011 (neither is named explicitly in this review's visible text, but the underlying concept — CO2-induced pseudodysplasia-mimicking artifact — is the same one Seoane 2013 and Monteiro 2019 both cite via Eversole 1997 and Seoane 2010).

## Statements about diagnostic interference (review's own synthesis)

- Verbatim (Discussion): "Despite the differences and heterogeneity among the included studies, almost all of them showed that the different tested laser wavelengths did not have a thermal effect that may hinder the histological diagnosis."
- Verbatim (Discussion): "...what should be done is to minimize [the thermal effect] by better adjusting the laser parameters. The extension of margins during the collection of laser oral biopsies and the use of laser only in non-suspicious lesions are recommended because of the difficulty of the histopathologist to assess the extension and grade of dysplasia at the surgical margins."
- INTERPRETATION (this vault's own, not the review's): this review's overall conclusion — thermal effect occurs and varies by wavelength/parameters, but rarely prevents diagnosis outright, with the recurring caveat about margin extension near suspected dysplastic/malignant lesions specifically — is directionally consistent with every primary source processed in this vault to date (including all four processed this phase), none of which reports a diagnosis actually being prevented by thermal artifact.

## Specimen size effects (review's own synthesis)

- The review does not perform its own pooled specimen-size analysis; it reports the 808 nm study's >3mm recommendation and, separately, cites Vescovi et al.'s <7mm finding (both summarized above) as two independent, non-reconciled specimen-size observations from two different included studies at two different laser wavelengths. The review does not attempt to unify these into one threshold.

## Methodological limitations identified by the review (verbatim/paraphrased)

- "The allocation concealment domain in the selection bias and the blinding domain in the performance bias were awarded unclear or high [risk] in almost all the included animal studies."
- Meta-analysis was not possible: "Heterogeneousness of the data was observed among the included studies concerning the study design, laser parameters, sample type, histological evaluation methods, and reported thermal effect that hindered the authors from carrying out the meta-analysis."
- Selection bias acknowledged: English-language only, PubMed/Scopus only.
- "Some studies reported the extent of the thermal effect of the tested laser in a confusing way that hindered the comparison process."
- Recommendation for future studies: "it should be more advisable to include the micrometric measurements of both epithelial and CT thermal effects" — directly relevant to this project, since Gobbo et al. 2017 (processed this phase) is itself an example of a study that does *not* separate epithelial/CT compartments, a gap this review's own recommendation independently flags.

## Key primary studies named in this review not yet in this vault

Per Step 7/12 of this phase's task — **do not promote these into primary metadata; list only as retrieval candidates**, consistent with the Phase 4 report:

- Fornaini et al. (cut-quality score, 0–5) — not yet retrieved.
- Braun et al. (MDD/DA) — not yet retrieved.
- Cercadillo-Ibarguren et al. 2010 — full citation identified in Phase 4 (PMID 20526250), not yet processed into a primary 07 Data note.
- Kawamura et al. — not yet retrieved; mentioned only for "histological and histometric analysis of the coagulated and thermally affected layers at the ablation bottom."
- Rizoiu et al. — full citation identified in Phase 4 (PMID 8899775), not yet processed into a primary 07 Data note.
- Matsumoto et al. — full citation identified in Phase 4 (PMID 19025408), not yet processed into a primary 07 Data note.

## Notes

- This review's search window (July 2020–November 2022) **predates** several sources already in this vault (e.g., Shnawa et al. 2025, Gambino et al. 2026, Al-Ani et al. 2023/2024, Pergolini et al. 2025) and postdates none of the four sources processed as primary studies this phase (Monteiro 2019, Seoane 2013, Gobbo 2017, Vescovi 2010) — all four should, in principle, have been eligible for this review's inclusion criteria (thermal-effect measurement + named wavelength). This vault has **not verified** whether all four were actually screened/included versus missed by the review's own search strategy; Gobbo 2017 and Vescovi 2010's findings are explicitly cross-confirmed present in the review's text (see tables above), but Monteiro 2019 and Seoane 2013 were **not** identified by name anywhere in the review's visible full text extracted by this vault — this is flagged as an open ambiguity (see Step 12 of the phase report), not resolved here.
- This review is **broader in scope** (28 studies, no scalpel-comparator requirement) than this vault's other existing systematic-review extraction, [[07 Data/Lopes-Santos et al 2023 - High-Power Laser Oral Biopsy Histology Systematic Review Data|Lopes-Santos et al. 2023]] (7 studies, scalpel-comparator required). The two reviews are **not merged** in this vault — they are tracked as two independent secondary sources with different inclusion criteria and partially overlapping but not identical study sets.
- No primary-study claim from this review has been used anywhere in this vault's Evidence/Synthesis updates (this phase) without independent primary-source verification, per this phase's explicit instruction.

## Related notes

- Literature: [[02 Literature/10.3390/dj11020028]]
- Secondary source (companion): [[07 Data/Lopes-Santos et al 2023 - High-Power Laser Oral Biopsy Histology Systematic Review Data]]
- Primary sources cross-confirmed by this review: [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data]], [[07 Data/Gobbo et al 2017 - Blue vs Infrared Diode Laser Biopsy Thermal Damage Data]], [[07 Data/Vescovi et al 2010 - Nd YAG Laser vs Scalpel Specimen Size Histology Data]]
- Evidence: [[04 Evidence/Biopsy Specimen Quality]]
- Synthesis: [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
- Project: [[01 Projects/Diode Laser Biopsy]]
