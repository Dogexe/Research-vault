# Study Dashboard

Auto-generated Dataview tables over `07 Data/` frontmatter. Source of truth is still the prose extraction in each note — this dashboard is a queryable index, not a replacement for reading the underlying evidence.

**Coverage note:** only notes with the YAML schema applied populate these tables — the schema-tagged set has grown past its original 12-note pilot batch. **Current count: 35 tagged notes in `07 Data/` as of 2026-09-17** (re-verified by searching for `classification:` in `07 Data/`; the earlier "23 as of 2026-09-14" figure below is historical, kept for the v1.1 patch's own record, not the current count). See [[99 Templates/Study Metadata Schema]] for field definitions. Un-tagged `07 Data/` notes simply do not appear yet — their absence is a coverage gap, not a finding that they lack the property. This count should be re-verified against the repository rather than assumed, since it will keep growing as more notes are tagged.

**Schema version:** now **v1.3** (see [[99 Templates/Study Metadata Schema]]). v1.3 adds `speed_varied` (whether incision speed was varied as an independent experimental condition) and `thermal_damage_measure` (the specific reported thermal-damage/coagulation/necrosis measure) on top of v1.2's `specimen_interpretability`. **Rollout is partial:** as of 2026-09-17, `speed_varied` is populated on 7 of 35 tagged notes and `thermal_damage_measure` on 15 of 35 — a coverage gap in the *rollout*, not evidence the other notes lack the property. `specimen_interpretability` (v1.2) is fully rolled out across all 35 tagged notes.

**Canonical research question** (see [[01 Projects/Diode Laser Biopsy]]): How do diode-laser operating parameters, independently measured delivered power, and incision speed/movement affect thermal tissue damage and biopsy-oriented histopathologic specimen quality in ex vivo oral soft tissue?

**Rationale (summary; canonical text: [[01 Projects/Diode Laser Biopsy#2. Current rationale|Diode Laser Biopsy §2]]):** Nominal diode-laser settings do not fully characterize tissue exposure, because independently measured delivered power can differ from the displayed value and emission characteristics, fiber/tip conditions, and incision speed also matter. Thermal tissue damage and biopsy-oriented specimen quality are related but distinct outcomes and are evaluated separately. Presets/manufacturer guidance, operator knowledge/training, and laser safety are supporting rationale only.

Clinical diagnostic-biopsy literature (Table A below) remains translational/context evidence, not the primary ex vivo endpoint.

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
- **`diagnostic_outcome` is clinical context, not the primary ex vivo endpoint.** Ex vivo/bench studies are expected to show `diagnostic_outcome: false` — that is not a limitation of those studies, it reflects that they were never designed to produce a diagnosis. Only `CORE BIOPSY` studies are expected to carry a diagnostic outcome. Where a source reports both, this vault treats `specimen_interpretability` — a whole-specimen readability/adequacy judgment — as the more direct biopsy-quality construct for this project's RQ; `diagnostic_outcome` alone (a bare yes/no diagnosis) does not substitute for it.
- **Thermal damage (`thermal_damage`, `thermal_damage_measure`) and specimen quality (`margin_quality`, `tissue_architecture`, `specimen_interpretability`) are tracked as separate outcome families and must not be conflated.** A study reporting thermal damage has not thereby reported anything about specimen quality, and vice versa — see [[01 Projects/Diode Laser Biopsy]] §3.
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

Studies that independently measured delivered power (whether or not a distinct value was tabulated), or reported a numeric incision speed — the two axes this vault treats as the strongest technical prior art regardless of whether the study was biopsy-oriented. Restricted to diode-laser, non-BACKGROUND rows (v1.1) — a non-diode comparator or a review/perspective source is not diode-laser technical prior art, even when it independently measures power or reports a speed sweep; see [[99 Templates/Study Metadata Schema]].

```dataview
TABLE
diode_laser,
measured_power,
measured_power_value_reported,
measured_power_w,
speed_mm_s,
speed_control,
histology,
oral_tissue,
biopsy_oriented
FROM "07 Data"
WHERE (measured_power = true OR incision_speed_reported = true) AND diode_laser = true AND classification != "BACKGROUND"
SORT file.name ASC
```

## C. Measured-power + speed + histology overlap — POTENTIAL NOVELTY, REQUIRES SYSTEMATIC VERIFICATION

Studies satisfying all three of: `measured_power = true`, `incision_speed_reported = true`, `histology = true`, restricted to diode-laser, non-BACKGROUND rows (v1.1, same reasoning as Table B). **This table is expected to be non-empty** — Hanke et al. 2021 and Strakas et al. 2023 already satisfy this combination, and hiding that would misrepresent the evidence base. The point of this table is not whether the three-way intersection is empty; it is which of the *additional* columns are `false`/`null` across the rows that do satisfy it.

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
WHERE measured_power = true AND incision_speed_reported = true AND histology = true AND diode_laser = true AND classification != "BACKGROUND"
SORT file.name ASC
```

**Reading this table:** existing diode-laser studies already demonstrate independently measured output, a reported incision speed, and histologic tissue-effect assessment. What none of the rows above also carry is `biopsy_oriented: true` — none excise a real lesion or assess biopsy-oriented specimen-quality outcomes (margin readability, tissue-architecture preservation, diagnostic outcome). The remaining potential gap is applying this measurement rigor to biopsy-oriented histopathologic specimen-quality outcomes in an ex vivo oral soft-tissue model — not the absence of measured power, not the absence of a reported speed, and not the absence of histology individually. This is **not** a claim that no such study exists anywhere, and **not** a "first ever" claim — see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for the full prose analysis this table summarizes.

(Table B stood at 11 rows when [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]] was first tagged — now 15; see "Current counts" below for the present figure and the historical v1.1 validation note for the count at the time of that patch. Table D below gives the fuller histology-specific breakdown.)

## D. Histopathologic specimen-quality outcome coverage

This is a **coverage matrix**, not a novelty detector. It shows which diode-laser, histology-reporting, non-BACKGROUND studies in `07 Data/` carry which specimen-quality-relevant fields, and how those overlap with measured power and incision speed. It does not compute or imply a novelty conclusion — see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] for that.

```dataview
TABLE
classification,
ex_vivo,
measured_power,
measured_power_value_reported,
speed_mm_s,
speed_control,
speed_varied,
thermal_damage,
thermal_damage_measure,
margin_quality,
tissue_architecture,
diagnostic_outcome,
specimen_interpretability,
biopsy_oriented
FROM "07 Data"
WHERE diode_laser = true
AND histology = true
AND classification != "BACKGROUND"
SORT file.name ASC
```

**How to read this table:**

- `thermal_damage: true` alone does **not** mean good or poor specimen quality — it only records that thermal damage/effect was reported as an outcome (quantified or qualitative), not its magnitude or clinical significance. `thermal_damage_measure` (v1.3) gives the short, source-faithful description of that measure where rolled out; a blank cell here can mean either "not reported" or "not yet tagged under v1.3" (see the Coverage note above) — never assume the former without checking the note.
- `speed_varied` (v1.3) records whether incision speed was tested as an independent experimental condition (`true`), held fixed (`false`), or not reported/unclear (`null`) — distinct from `speed_mm_s` (the value(s) themselves) and `speed_control` (how the value was produced). See [[06 Synthesis/Incision Speed and Movement in Diode Laser Tissue Interaction]] for the prose synthesis of which studies vary speed.
- `margin_quality` and `tissue_architecture` are free-text v1 fields (see [[99 Templates/Study Metadata Schema]]) and may contain heterogeneous descriptions — a quantified µm distance, a qualitative statement, or a margin-*width* recommendation — rather than a standardized score. Do not compare cells across rows as if they were the same scale.
- `diagnostic_outcome` is mainly clinical/translational context here, not this project's primary ex vivo endpoint (see the Legend above and [[01 Projects/Diode Laser Biopsy]]).
- `specimen_interpretability` (added in schema v1.2) is a heterogeneous free-text field for explicit specimen/slide readability or adequacy judgments. It is not a standardized scale and should not be compared numerically across studies. A `null` cell here means no distinct interpretability construct was reported under the schema definition — it does **not** mean the specimen was uninterpretable.
- `biopsy_oriented` helps distinguish real biopsy/lesion-excision pathways from technical, non-lesional incision-characterization models — it is not itself a quality score.
- The project's actual experimental gap must still be read from the **combination** of measured power, speed, and specimen-quality-relevant outcomes across rows — no single column in this table answers it by itself.
- A blank/`null` cell means not reported / not applicable / unresolved per schema rules (see [[99 Templates/Study Metadata Schema]]) — **never** treat it as proof the phenomenon was absent from the underlying study or from the wider literature.
- Absence of an otherwise-qualifying study from this table can also reflect incomplete schema rollout (an untagged `07 Data/` note) rather than a property of the study itself — see the Coverage note above.

## Current counts (refreshed 2026-09-17)

Re-counted directly against `07 Data/` frontmatter (not the dataview render, to catch quoting/formatting variance the queries above tolerate but a manual audit should not assume away):

- **Table A (CORE BIOPSY):** 14 rows.
- **Table B (measured power OR reported speed, diode, non-BACKGROUND):** 15 rows.
- **Table C (measured power AND reported speed AND histology, diode, non-BACKGROUND):** 4 rows — Goharkhay 1999, Hanke 2021, Strakas 2023, and Liu et al. 2025 (newly qualifying since the counts below were last narrated).
- **Table D (diode, histology, non-BACKGROUND):** 24 rows.

These are current figures, not a patch delta — see the historical v1.1 validation note immediately below for the schema-patch narrative that produced the v1.1 figures, which are preserved as history and are **not** current counts.

## Validation note (schema v1.1 maintenance patch, historical — figures below are as of the 2026-09-14 patch, not current)

A 10-note stress-test batch (Isola 2018, Romeo 2014, Gambino 2026, Li 2022, Romanos 2022, Suter 2010, Kim 2020, Wilder-Smith 1995, Gutiérrez-Corrales 2020, Romanos 2013) surfaced two schema/dashboard defects, now fixed as v1.1:

- **`speed_mm_s` couldn't represent a multi-point tested sweep.** Romanos et al. 2013 reports a 5-point tested incision-speed sweep (12.5, 6.0, 3.0, 1.0, 0.0 mm/s) via a programmable translation stage, but the field's v1 type was "number or `null`" only. Widened to "number, list, or `null`," matching its sibling numeric fields (`wavelength_nm`, `set_power_w`, `measured_power_w`, `fiber_diameter_um`). Romanos 2013 now carries `speed_mm_s: [12.5, 6.0, 3.0, 1.0, 0.0]` instead of `null`.
- **Tables B and C could silently admit a non-diode or review-tier row.** Wilder-Smith et al. 1995 (three CO2 lasers, `diode_laser: false`) appeared in Table B purely because it independently measures power — not diode-laser prior art. Both tables now add `diode_laser = true AND classification != "BACKGROUND"`. Confirmed: Wilder-Smith 1995 and Romanos et al. 2013 (a BACKGROUND-tier CE review) no longer appear in either table; Hanke 2021, Strakas 2023, and Goharkhay 1999 remain in Table C; Kim et al. 2020 (SUPPORTING TECHNICAL, diode, no biological tissue) correctly remains in Table B — lack of tissue is not grounds to exclude a genuine power-measurement methodological precedent, and is not addressed by this patch (see [[99 Templates/Study Metadata Schema]] for the deferred non-tissue boundary case).

Table A is untouched (already scoped by `classification = "CORE BIOPSY"`, no diode/BACKGROUND ambiguity applies there).

All 22 tagged notes re-validated after this patch: YAML parses cleanly on every note, no boolean stored as a string, no controlled-vocabulary field outside its allowed list, `speed_mm_s` values valid under the widened v1.1 type, and no impossible combination (e.g. `measured_power_value_reported: true` with `measured_power` not `true`, or a populated `speed_mm_s` with `incision_speed_reported: false`). (The "22" above is this specific validation pass's count at the time of the v1.1 patch, not a current figure — one further note, [[07 Data/Prado et al 2022 - Micro vs Super Pulsed Diode Laser Ex Vivo Thermal Damage Data|Prado et al. 2022]], was tagged afterward, bringing the current total to 23 as of 2026-09-14; see the Coverage note above.)

**Membership before → after this patch:** Table A unchanged at 8 rows. **Table B: 12 → 10** (both Wilder-Smith 1995 and Romanos et al. 2013 removed — Wilder-Smith via `diode_laser = true`, Romanos 2013 via `classification != "BACKGROUND"`; both had qualified for B under v1 via `incision_speed_reported`/`measured_power`, despite neither being diode-technical prior art). **Table C: 3 → 3, unchanged** (Goharkhay 1999, Hanke 2021, Strakas 2023) — neither Wilder-Smith nor Romanos 2013 had ever qualified for C (both lack the full three-way `measured_power AND incision_speed_reported AND histology` combination). Schema frozen at v1.1 pending the next rollout batch — see [[99 Templates/Study Metadata Schema]].

## Related

- [[99 Templates/Study Metadata Schema]] — field definitions and allowed values
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] — prose analysis this dashboard summarizes in queryable form
- [[06 Synthesis/Incision Speed and Movement in Diode Laser Tissue Interaction]] — prose synthesis behind `speed_mm_s`/`speed_control`/`speed_varied`
- [[01 Projects/Diode Laser Biopsy]] — canonical research question and experimental chain
- [[04 Evidence/Power Output and Tissue Effect]]
