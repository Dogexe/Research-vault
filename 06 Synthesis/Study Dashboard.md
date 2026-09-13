# Study Dashboard

Auto-generated Dataview tables over `07 Data/` frontmatter. Source of truth is still the prose extraction in each note — this dashboard is a queryable index, not a replacement for reading the underlying evidence.

**Coverage note:** only notes with the YAML schema applied populate these tables (currently the 12 priority studies listed in [[99 Templates/Study Metadata Schema]]). Un-tagged `07 Data/` notes simply do not appear yet — their absence is a coverage gap, not a finding that they lack the property.

## Legend

- **Set power ≠ measured delivered power.** `set_power_w` is the console/dial value the operator selected. `measured_power` / `measured_power_w` record only an independently instrument-verified output value (power meter at the fiber tip or outflow). A study can report a set power with `measured_power: false` — that means no independent verification was reported, not that the set value is wrong.
- **`null` = not reported / unknown**, never an inferred or assumed value. A blank cell in these tables means the source didn't state it, per this vault's `UNKNOWN`-over-invention rule.
- **Classification meanings:**
  - `CORE BIOPSY` — a real (human or animal) diagnostic or excisional biopsy pathway; a lesion is excised and/or a histopathologic diagnosis is rendered.
  - `SUPPORTING TECHNICAL` — controlled bench/ex vivo characterization of cutting, thermal, or power behavior; no lesion, no diagnosis. Used for operating-parameter and methodology evidence, not diagnostic-outcome evidence.
  - `BACKGROUND` — general/contextual literature not itself reporting new operating-parameter or outcome data (not yet used among the tagged notes below).
- **`diagnostic_outcome` is clinical context, not the primary ex vivo endpoint.** Ex vivo/bench studies are expected to show `diagnostic_outcome: false` — that is not a limitation of those studies, it reflects that they were never designed to produce a diagnosis. Only `CORE BIOPSY` studies are expected to carry a diagnostic outcome.

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

Studies that independently measured delivered power, or reported a numeric incision speed (mechanized, clinician-controlled, or otherwise measured) — the two axes this vault treats as the strongest technical prior art regardless of whether the study was biopsy-oriented.

```dataview
TABLE
oral_tissue,
ex_vivo,
measured_power,
measured_power_w,
speed_mm_s,
speed_control,
histology,
biopsy_oriented
FROM "07 Data"
WHERE measured_power = true OR incision_speed_reported = true
SORT file.name ASC
```

## C. Novelty-gap candidates

Studies that combine all three of: independently measured power, a reported incision speed, AND histology. This is the intersection the vault's novelty analysis cares about — a near-empty or single-row result here is itself the finding (see [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]).

```dataview
TABLE
oral_tissue,
biopsy_oriented,
diagnostic_outcome,
margin_quality,
tissue_architecture
FROM "07 Data"
WHERE measured_power = true AND incision_speed_reported = true AND histology = true
SORT file.name ASC
```

## Related

- [[99 Templates/Study Metadata Schema]] — field definitions and allowed values
- [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]] — prose analysis this dashboard summarizes in queryable form
- [[04 Evidence/Power Output and Tissue Effect]]
