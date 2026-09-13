# Study Dashboard

Auto-generated Dataview tables over `07 Data/` frontmatter. Source of truth is still the prose extraction in each note — this dashboard is a queryable index, not a replacement for reading the underlying evidence.

**Coverage note:** only notes with the YAML schema applied populate these tables (currently the 12 priority studies listed in [[99 Templates/Study Metadata Schema]]). Un-tagged `07 Data/` notes simply do not appear yet — their absence is a coverage gap, not a finding that they lack the property.

**Canonical research question** (see [[01 Projects/Diode Laser Biopsy]]): How do diode laser operating parameters, actual delivered power, and incision speed affect histopathologic quality of ex vivo oral soft-tissue specimens? Primary experimental chain: `Preset / set power` → `independently measured delivered power` → `controlled or explicitly reported incision speed` → `tissue interaction` → `thermal / structural alteration` → `histopathologic specimen quality`. Clinical diagnostic-biopsy literature (Table A below) remains translational/context evidence, not the primary ex vivo endpoint.

## Legend

- **Set power ≠ measured delivered power ≠ a reported measured value.** These are three separate questions, tracked as three separate fields:
  - `measured_power` — was output independently measured at all (e.g. a calibrated power meter checked delivered output), regardless of whether a number was tabulated?
  - `measured_power_value_reported` — did the source additionally report the actual numerical measured output, as a value distinct from the set power?
  - `measured_power_w` — that explicit measured value, in watts. Populated only when `measured_power_value_reported` is `true`.
  - A study can independently measure output for QC purposes (`measured_power: true`) without ever tabulating the number (`measured_power_value_reported: false`, `measured_power_w: null`) — this is not a gap in this vault's extraction, it reflects what the source itself reported. See [[99 Templates/Study Metadata Schema]] for the full worked comparison.
- **`null` = not reported / unknown / not applicable**, never an inferred or assumed value. A blank cell in these tables means the source didn't state it, per this vault's `UNKNOWN`-over-invention rule.
- **Classification meanings** (only these three; no additional tiers):
  - `CORE BIOPSY` — a real (human or animal) diagnostic or excisional biopsy pathway; a lesion is excised and/or a histopathologic diagnosis is rendered.
  - `SUPPORTING TECHNICAL` — controlled bench/ex vivo characterization of cutting, thermal, or power behavior; no lesion, no diagnosis. A study can be methodologically central to this project's technical chain (e.g. Hanke 2021, Strakas 2023) while still carrying this classification — its importance is explained in prose/dashboard notes, not by inventing a new tier.
  - `BACKGROUND` — general/contextual literature not itself reporting new operating-parameter or outcome data (not yet used among the tagged notes below).
- **`diagnostic_outcome` is clinical context, not the primary ex vivo endpoint.** Ex vivo/bench studies are expected to show `diagnostic_outcome: false` — that is not a limitation of those studies, it reflects that they were never designed to produce a diagnosis. Only `CORE BIOPSY` studies are expected to carry a diagnostic outcome.
- **`speed_control: unknown` is the default**, not a fallback of last resort, whenever a numeric speed is reported but the source does not explicitly describe how that speed was controlled or verified. A reported number alone never justifies `mechanized` or `clinician-controlled`.

## A. Core biopsy studies

```dataview
TABLE
classification,
wavelength_nm,
set_power_w,
measured_power,
incision_speed_reported AS incision_speed_reported,
histology,
diagnostic_outcome
FROM "07 Data"
WHERE classification = "CORE BIOPSY"
SORT file.name ASC
```

## B. Closest methodological precedents

Studies that independently measured delivered power (whether or not a distinct value was tabulated), or reported a numeric incision speed — the two axes this vault treats as the strongest technical prior art regardless of whether the study was biopsy-oriented.

```dataview
TABLE
measured_power,
measured_power_value_reported,
measured_power_w,
speed_mm_s,
speed_control,
histology,
oral_tissue,
biopsy_oriented
FROM "07 Data"
WHERE measured_power = true OR incision_speed_reported = true
SORT file.name ASC
```

## C. Measured-power + speed + histology overlap — POTENTIAL NOVELTY, REQUIRES SYSTEMATIC VERIFICATION

Studies satisfying all three of: `measured_power = true`, `incision_speed_reported = true`, `histology = true`. **This table is expected to be non-empty** — Hanke et al. 2021 and Strakas et al. 2023 already satisfy this combination, and hiding that would misrepresent the evidence base. The point of this table is not whether the three-way intersection is empty; it is which of the *additional* columns are `false`/`null` across the rows that do satisfy it.

```dataview
TABLE
oral_tissue,
ex_vivo,
biopsy_oriented,
margin_quality,
tissue_architecture,
diagnostic_outcome,
measured_power_value_reported
FROM "07 Data"
WHERE measured_power = true AND incision_speed_reported = true AND histology = true
SORT file.name ASC
```

**Reading this table:** existing diode-laser studies already demonstrate independently measured output, a reported incision speed, and histologic tissue-effect assessment. What none of the rows above also carry is `biopsy_oriented: true` — none excise a real lesion or assess biopsy-oriented specimen-quality outcomes (margin readability, tissue-architecture preservation, diagnostic outcome). The remaining potential gap is applying this measurement rigor to biopsy-oriented histopathologic specimen-quality outcomes in an ex vivo oral soft-tissue model — not the absence of measured power, not the absence of a reported speed, and not the absence of histology individually. This is **not** a claim that no such study exists anywhere, and **not** a "first ever" claim — see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the full prose analysis this table summarizes.

## Validation note (schema v1 freeze)

All 12 tagged notes were re-validated after the schema v1 audit: YAML parses cleanly on every note, no boolean is stored as a string, no controlled-vocabulary field holds a value outside its allowed list, and no impossible combination exists (e.g. `measured_power_value_reported: true` with `measured_power` not `true`, or a populated `speed_mm_s` with `incision_speed_reported: false`). Two corrections came out of this audit:

- **Merigo et al. 2012** — `measured_power` was `false`, contradicting the note's own prose, which states the diode arm was independently checked with a power meter (pooled across 5 device types, not diode-isolated). Corrected to `true`, with `measured_power_value_reported: false` added — the same pattern as Hanke/Strakas. This moved Merigo into Table B.
- **Goharkhay et al. 1999** — `speed_control` was `measured`; per the schema's now-documented precedence rule (motion-generation mechanism takes priority over a separate verification detail), corrected to `mechanized` — the source's motorized handpiece generated the motion, and the stopwatch timing is a verification detail, not the primary classification.

Current membership: **Table A** 4 rows, **Table B** 6 rows (Al-Ani 2023, Al-Ani 2024, Goharkhay 1999, Hanke 2021, Merigo 2012, Strakas 2023), **Table C** 3 rows (Goharkhay 1999, Hanke 2021, Strakas 2023) — unchanged by the Merigo correction, since Merigo has no reported incision speed. Schema is frozen at v1 pending wider rollout — see [[99 Templates/Study Metadata Schema]].

## Related

- [[99 Templates/Study Metadata Schema]] — field definitions and allowed values
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] — prose analysis this dashboard summarizes in queryable form
- [[01 Projects/Diode Laser Biopsy]] — canonical research question and experimental chain
- [[04 Evidence/Power Output and Tissue Effect]]
