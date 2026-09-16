---
classification: "CORE BIOPSY"
oral_tissue: true
ex_vivo: false
human_tissue: true
diode_laser: true
wavelength_nm: [445, 970]
set_power_w: [1.4, 2.0]
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
thermal_damage_measure: "maximum thermal damage along cutting margin (μm): BLUE (445 nm) 71.3±51.8 (n=24), IR (970 nm) 186.8±82.7 (n=24), non-laser QMR comparator 111.4±55.4 (n=25); 20/93 specimens (21.5%) had thermal damage that was not measurable"
margin_quality: null
tissue_architecture: null
specimen_interpretability: "20/93 specimens (21.5%) had thermal damage that could not be measured (not evaluable in smaller lesions, not recognizable in larger ones); despite this, 'all the techniques allowed correct histological sampling' and diagnosis was not impaired in any case."
diagnostic_outcome: true
biopsy_oriented: true
full_text: true
needs_verification: true
---

# Laser Operating Parameters

Record values exactly as reported. Use `UNKNOWN` when a value is not reported; do not infer missing parameters.

**Vault classification: CORE BIOPSY — real human excisional biopsies (n=93), two diode wavelengths (445 nm "BLUE" vs 970 nm "IR") plus a non-laser electrosurgical comparator (QMR scalpel), single blind pathologist quantifying thermal damage along the cutting margin.** This is the strongest diode-specific blinded-pathologist precedent found in the Phase 4 search — see [[04 Evidence/Biopsy Specimen Quality]].

**YAML scoping note**: `wavelength_nm` and `set_power_w` are two-element lists in paired order [BLUE (445 nm), IR (970 nm)] per this vault's dual-arm convention (matching [[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters|Al-Ani et al. 2023]]/[[07 Data/Al-Ani et al 2024 - Dual-Wavelength Diode vs Er,Cr YSGG Biopsy Margin Histology Data|2024]]). `set_power_w` records each arm's stated **average** power (1.4 W BLUE, 2.0 W IR); each arm's **peak** power (2.0 W BLUE, 6.0 W IR) is preserved in the Extraction table below since the schema has no dedicated peak-power field. The third study arm (QMR electrosurgical scalpel) is not a laser and is excluded from all diode-scoped YAML fields but retained in the Extraction table and Notes as a comparator.

## Source

- Literature note: [[02 Literature/10.1117/1.JBO.22.12.121602]]
- Source link: https://doi.org/10.1117/1.JBO.22.12.121602
- Source locator: Full text (cached plain-text extraction, `.zotero-ft-cache`) — Abstract; Materials and Methods; Statistical Analysis; Tables 1–4; Results; Discussion; Conclusion.

## Extraction

| Parameter | BLUE group (diode) | IR group (diode) | QMR group (non-laser comparator) | Evidence status |
| --- | --- | --- | --- | --- |
| Device | InGaN diode laser, K-Laser Blue (class IV), Eltech S.r.l., Treviso, Italy | Diode laser, K-Laser K-Series (class IV), Eltech S.r.l., Treviso, Italy | QMR electroscalpel, VESALIUS (Telea Electronic Engineering S.r.l.) | FACT |
| Wavelength | 445 nm | 970 nm | N/A (electrosurgical, not optical) | FACT |
| Peak power | 2.0 W | 6.0 W | N/A | FACT |
| Average power | 1.4 W | 2.0 W | N/A | FACT |
| Pulse parameters | t-on 20 ms, t-off 8 ms | Pulsed modality, 33% duty cycle, 10 Hz frequency | N/A | FACT |
| Fiber diameter | 320 μm | 320 μm | N/A (thin, straight electrode) | FACT |
| Operating mode | Pulsed (t-on/t-off cycling stated explicitly) | Pulsed (explicitly stated "pulsed modality") | "Cut and coagulate" modality | FACT |
| Contact mode | UNKNOWN — not explicitly stated | UNKNOWN — not explicitly stated | UNKNOWN — not explicitly stated | UNKNOWN (absence confirmed by full-text read) |
| Tip initiation status | UNKNOWN — not mentioned | UNKNOWN — not mentioned | N/A | UNKNOWN |
| Independently measured power | NO — device parameters are the manufacturer-set operating values; no power meter or verification step is described | NO | N/A | FACT (absence confirmed) |
| Incision speed | NOT REPORTED — no mm/s value or control-mechanism description for any group | NOT REPORTED | NOT REPORTED | UNKNOWN |
| n | 39 | 27 | 27 | FACT |
| Sample / lesion | Benign oral lesions: fibroma, angiofibroma, epulis, mucocele, papilloma, angioma, amalgam tattoo, papillae, lipoma; mean lesion dimension 5.7±2.4 mm | (same diagnosis categories, n as tabulated) 6.0±2.2 mm | 6.9±2.9 mm | FACT |
| Tissue processing | Formalin fixation, H&E staining (implied standard; explicit stain type not separately restated in Methods beyond "hematoxylin and eosin staining") | (same protocol, shared across groups) | (same protocol) | FACT |
| Pathologist involvement | **One dedicated oral pathologist**, explicitly **blinded to the employed technique** | (same pathologist/protocol, shared across all groups) | (same) | FACT |
| Maximum thermal damage along cutting margin | 71.3±51.8 μm (median 54.4, range 27.2–268.7), n=24 evaluable of 39 | 186.8±82.7 μm (median 173.3, range 50.0–406.9), n=24 evaluable of 27 — **significantly higher than both BLUE and QMR** | 111.4±55.4 μm (median 95.9, range 32.5–256.4), n=25 evaluable of 27 — significantly higher than BLUE | FACT |
| Thermal damage not quantifiable | 15 of 39 samples ("not evaluable" in smaller lesions or "not recognizable" in larger ones, pooled across the whole cohort: 20/93 total) | (pooled figure above) | (pooled figure above) | FACT |
| Histological diagnosis rendered | Yes, per lesion type (fibroma etc., Table 2) | Yes | Yes | FACT |
| Diagnosis affected by technique | **No — explicit statement**: "In all cases, the pathologist had no difficulties in performing a histological diagnosis following the use of an electrosurgical device," and "All the techniques allowed correct histological sampling" | Same statement, applies to all three groups | Same statement | FACT |

## Study design (per task's Section A)

- Human, in vivo, prospective (Ospedale Maggiore, Trieste, Italy; ethics-approved). NOT ex vivo.
- **True diagnostic/excisional biopsy pathway**: real benign oral lesions, histological diagnosis rendered for every case; patients with a dysplastic/neoplastic histological report were an explicit **exclusion** criterion applied before enrollment (i.e., all included lesions were confirmed benign — this is a deliberate scope restriction stated by the authors, not a limitation this vault infers).
- Comparator groups: 3 arms — BLUE diode (445 nm), IR diode (970 nm), QMR electrosurgical scalpel (not a laser).
- Sample size: n=93 total (39/27/27).
- Tissue/site: lip, cheek, palate, tongue, floor of mouth, gingiva — distribution not significantly different across groups (P=0.522).

## Histopathology methodology (per task's Section C)

- Stain: hematoxylin and eosin (H&E), stated generally.
- **Pathologist involvement: one dedicated oral pathologist.**
- **Blinded: YES, explicitly stated** ("A blind pathologist evaluated the thermal damage"; "blinded in regard to the employed technique").
- **Number of assessors: 1.** NOT a multi-pathologist consensus design (contrast with Seoane et al. 2013's two-pathologist consensus).
- **Consensus process: N/A** (single assessor).
- **Inter-rater reliability: NOT REPORTED** (not applicable with a single assessor).
- Magnification / measurement method: not specified beyond "quantifying the maximum thermal damage of the specimen (expressed in microns) along the cutting margin" — no ocular micrometer brand, magnification power, or image-analysis software is named (a notable gap relative to Monteiro 2019 and Vescovi 2010, both of which name their measurement instruments).

## Outcome terminology (author's exact wording, per task's Section D)

- **"Thermal damage" / "maximum thermal damage... along the cutting margin"** — the paper's own primary outcome phrase; also labeled **"thermal damage score (μm)"** in Table 4's own header, despite being a direct linear measurement, not an ordinal score — this vault preserves that exact (arguably inconsistent) source labeling rather than correcting it.
- **"Not evaluable"** vs. **"not recognizable"** — two distinct reasons given by the source for the 20 unmeasurable specimens (smaller lesions vs. larger lesions, respectively) — preserved as the source's own distinct categories, not merged.
- **"All the techniques allowed correct histological sampling"** — the paper's own diagnostic-adequacy conclusion, structurally similar to but independently worded from Monteiro 2019's "no... limitation of diagnosis" and Gundlapalle et al. 2022's slide-quality framing (already in vault).

## Outcome type (per task's Section E)

| Outcome | Type | Unit/range | Epithelial component? | CT component? | Margin-specific? | Architecture-specific? | Diagnosis affected? | Adequacy/readability judgment? |
|---|---|---|---|---|---|---|---|---|
| Thermal damage (μm) | Quantitative continuous | μm, mean±SD/median/range, by group | No — **not separated into epithelial vs. connective-tissue compartments; a single pooled "maximum thermal damage" value per specimen** | No (same) | Yes (along the cutting margin) | No | No | No |
| "Correct histological sampling" | Binary, whole-cohort statement | Yes/No | — | — | — | — | Yes | Yes |
| Non-measurability (20/93) | Count/categorical | Two named reasons (not evaluable / not recognizable) | — | — | Indirect (a margin-measurement limitation) | — | No (diagnosis still possible per the paper) | Partial — a measurement-adequacy limitation, distinct from a diagnostic-adequacy limitation |

## Score/grading details (per task's Section F)

- **No formal ordinal score is used** — despite Table 4's header calling it a "thermal damage score," the value itself is a direct μm measurement, not a categorical/ordinal grade. This vault does not treat this as a true "score" for classification purposes, per the task's instruction to preserve exact terminology while still distinguishing constructs (quantitative continuous vs. ordinal) accurately in the Outcome-type table above.
- Score name: N/A (no true ordinal instrument).
- Validation status: N/A.
- **Blinded: YES.**
- **Number of scorers: 1.**
- **Reliability statistic: NOT REPORTED.**

## Diagnostic-interpretability findings (task's specific focus for this source)

- FACT: The paper explicitly separates "quantifiable thermal damage" from "successful diagnosis" — 20 of 93 specimens (21.5%) could not have their thermal damage quantified at all (for two distinct, named reasons: too small to evaluate, or too large/damage not locatable), **yet the paper states diagnosis was still successful in every case, including these 20** ("In all cases, the pathologist had no difficulties in performing a histological diagnosis"). This is a clean, explicit demonstration that a margin-measurement outcome and a diagnostic-adequacy outcome are **not the same construct** and can diverge within the same dataset — directly relevant to this project's own distinction between thermal-damage metrics and specimen-quality/diagnostic-adequacy metrics.
- FACT: Epithelial and connective-tissue compartments are **not separated** in this paper's thermal-damage measurement — a genuine methodological limitation relative to Monteiro 2019, Vescovi 2010, and the vault's existing Al-Ani 2024/Gambino 2026 notes, all of which report compartment-specific values.

## Notes

- FACT: This is the vault's first CORE BIOPSY source with a genuine two-diode-wavelength, blinded-pathologist, real-human excisional-biopsy design — strengthens the diode-specific specimen-quality precedent materially.
- FACT: Independently measures no power and reports no incision speed for any arm — does not close this project's core measured-power + speed gap; strengthens only the outcome-methodology side.
- NEEDS VERIFICATION flagged in YAML: (1) `cw_pw: PW` — both diode arms are pulsed by the source's own description (t-on/t-off for BLUE; explicit "pulsed modality" for IR), so this reflects both arms accurately, but a human should re-confirm neither arm has an unstated CW option; (2) `contact_mode: null` — the paper never states contact vs. non-contact explicitly for any arm, despite fiber-delivered lasers typically implying contact use; per schema convention this stays `null` rather than being inferred; (3) `set_power_w` uses average power (not peak) as the primary value, matching the convention used elsewhere in this vault, but a human should confirm this is the intended reading given the paper reports both figures with comparable prominence.
- Classification for this vault: CORE BIOPSY, diode-inclusive. Directly strengthens diode-specific outcome-methodology precedent; does not touch the measured-power or incision-speed axes.

## สรุปภาษาไทย

- การศึกษานี้เปรียบเทียบเลเซอร์ไดโอด 2 ความยาวคลื่น (445 nm "BLUE" กับ 970 nm "IR") และเครื่องมือไฟฟ้า QMR ในผู้ป่วยจริง 93 ราย โดยมี**พยาธิแพทย์ 1 คนที่ปกปิดข้อมูลเทคนิคที่ใช้ (blinded)** วัดความเสียหายจากความร้อนสูงสุดตามแนวขอบตัด
- กลุ่ม BLUE มีความเสียหายน้อยที่สุด (71.3±51.8 ไมโครเมตร) กลุ่ม IR มากที่สุด (186.8±82.7 ไมโครเมตร)
- **20 ใน 93 ตัวอย่าง (21.5%) ไม่สามารถวัดปริมาณความเสียหายจากความร้อนได้เลย แต่พยาธิแพทย์ยังคงวินิจฉัยได้สำเร็จในทุกกรณี** — แสดงให้เห็นชัดเจนว่าการวัดความเสียหายจากความร้อนกับความสามารถในการวินิจฉัยเป็นคนละตัวแปรกัน
- ไม่มีการแยกผลระหว่างชั้นเยื่อบุผิวกับชั้นเนื้อเยื่อเกี่ยวพัน ไม่มีการวัดกำลังขาออกจริง และไม่มีการรายงานความเร็วตัด

## Related notes

- Literature: [[02 Literature/10.1117/1.JBO.22.12.121602]]
- Data: [[07 Data/Palaia et al 2021 - 445 nm Diode Laser In Vivo Biopsy Thermal Effect Data]] (same 445 nm wavelength class, different device/group)
- Evidence: [[04 Evidence/Biopsy Specimen Quality]]
- Concepts: [[03 Concepts/Glossary/Diagnostic Quality]]
- Synthesis: [[06 Synthesis/Diode Laser Biopsy Specimen Quality]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
- Project: [[01 Projects/Diode Laser Biopsy]]
