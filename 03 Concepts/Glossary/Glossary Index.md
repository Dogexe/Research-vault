# Glossary Index

This glossary supports interpretation of the diode-laser oral soft-tissue biopsy project (see [[01 Projects/Diode Laser Biopsy]]) — its canonical research question is how diode laser operating parameters, actual delivered power, and incision speed affect histopathologic quality of ex vivo oral soft-tissue specimens. Foundational physics (Section 1) is kept explicitly separate from project-specific evidence (Sections 2–5): general textbook-level definitions are stated as background knowledge, while claims about what this project's own literature shows are sourced to `04 Evidence/`, `06 Synthesis/`, and `07 Data/` notes. **Glossary equations are conceptual aids only and must never be used to infer or back-calculate a study's unreported values** (e.g. deriving incision speed from procedure time, or energy-per-unit-length from separately reported power and speed) — see individual notes' "Common pitfalls" sections and AGENTS.md.

Each entry uses the standard [[99 Templates/Glossary Term Template|Glossary Term Template]]: `aliases`, `category`, `unit`, `symbol`, and `equation` in frontmatter, plus Definition / Unit-equation / In this project / Common pitfalls / Related terms / Evidence-source-note sections. Older glossary notes (created before this template) keep their original prose structure with the same frontmatter added on top — see AGENTS.md's "prefer updating existing notes, minimal diffs" rule.

## 1. Fundamental Physics

Foundational radiometric/optical quantities, independent of any specific device or study.

- [[03 Concepts/Glossary/Power]]
- [[03 Concepts/Glossary/Energy]]
- [[03 Concepts/Glossary/Wavelength]]
- [[03 Concepts/Glossary/Optical Frequency]]
- [[03 Concepts/Glossary/Photon Energy]]
- [[03 Concepts/Glossary/Spot Size]] (includes beam area)
- [[03 Concepts/Glossary/Irradiance]]
- [[03 Concepts/Glossary/Fluence]]
- [[03 Concepts/Glossary/Exposure Time]]
- [[03 Concepts/Glossary/Energy per Unit Length]]

## 2. Laser Operating Parameters

Device/console-level and technique-level parameters as reported and extracted in `07 Data/`.

- [[03 Concepts/Glossary/Set Power]]
- [[03 Concepts/Glossary/Measured Power]]
- [[03 Concepts/Glossary/Delivered Power]]
- [[03 Concepts/Glossary/Power Loss]]
- [[03 Concepts/Glossary/Power Meter]]
- [[03 Concepts/Glossary/Calibration]]
- [[03 Concepts/Glossary/Measurement Location]]
- [[03 Concepts/Glossary/Output Stability]]
- [[03 Concepts/Glossary/Power Output]]
- [[03 Concepts/Glossary/Average Power]]
- [[03 Concepts/Glossary/Peak Power]]
- [[03 Concepts/Glossary/Continuous Wave]]
- [[03 Concepts/Glossary/Pulsed Mode]]
- [[03 Concepts/Glossary/Pulse Duration]]
- [[03 Concepts/Glossary/Frequency]] (pulse repetition rate)
- [[03 Concepts/Glossary/Duty Cycle]]
- [[03 Concepts/Glossary/Incision Speed]]
- [[03 Concepts/Glossary/Procedure Time]]
- [[03 Concepts/Glossary/Excision Time]]
- [[03 Concepts/Glossary/Power-to-Speed Relationship]]

## 3. Beam / Fiber Delivery

Delivery geometry — how energy actually reaches the tissue surface.

- [[03 Concepts/Glossary/Fiber Diameter]]
- [[03 Concepts/Glossary/Contact Mode]]
- [[03 Concepts/Glossary/Non-contact Mode]]
- [[03 Concepts/Glossary/Initiated Tip]]
- [[03 Concepts/Glossary/Non-initiated Tip]]
- [[03 Concepts/Glossary/Hot-tip Effect]]
- [[03 Concepts/Glossary/Beam Delivery Geometry]]

(See also [[03 Concepts/Glossary/Spot Size]] in Section 1 — not duplicated here.)

## 4. Laser–Tissue Interaction

Physical/optical mechanisms by which laser energy is absorbed and produces tissue effect, in order from optical fate → thermal mechanism → observable outcome.

- [[03 Concepts/Glossary/Absorption]]
- [[03 Concepts/Glossary/Scattering]]
- [[03 Concepts/Glossary/Reflection]]
- [[03 Concepts/Glossary/Transmission]]
- [[03 Concepts/Glossary/Chromophore]]
- [[03 Concepts/Glossary/Photothermal Interaction]]
- [[03 Concepts/Glossary/Thermal Relaxation Time]]
- [[03 Concepts/Glossary/Coagulation Zone]]
- [[03 Concepts/Glossary/Vaporization]]
- [[03 Concepts/Glossary/Ablation]]
- [[03 Concepts/Glossary/Carbonization]]
- [[03 Concepts/Glossary/Temperature Rise]]
- [[03 Concepts/Glossary/Thermal Damage]] (includes thermal artifact / thermal-affected zone / TIZ / lateral, vertical, horizontal subtypes / collagen denaturation)
- [[03 Concepts/Glossary/Incision Depth]] (includes cutting depth)
- [[03 Concepts/Glossary/Cutting Efficiency]]

## 5. Histopathology / Biopsy Quality

Specimen-level histopathologic outcomes — this project's primary endpoint domain.

- [[03 Concepts/Glossary/Histology]]
- [[03 Concepts/Glossary/Histological Artifact]]
- [[03 Concepts/Glossary/Specimen Margin]]
- [[03 Concepts/Glossary/Margin Quality]] (includes margin readability)
- [[03 Concepts/Glossary/Tissue Architecture Preservation]]
- [[03 Concepts/Glossary/Diagnostic Quality]] (includes diagnostic outcome)
- [[03 Concepts/Glossary/Biopsy-oriented]]
- [[03 Concepts/Glossary/Biopsy Specimen Quality]] (composite project outcome concept)
- [[03 Concepts/Glossary/Artifact Grading]]

## Canonical terminology

This glossary is the preferred vocabulary layer for the vault: when writing or updating metadata, evidence synthesis, or project-level notes, prefer the canonical term listed here over a scattered mix of synonyms. This does **not** mean rewriting evidence — a source's original wording must still be preserved in extraction prose (per AGENTS.md). Normalization exists so that different sources' terminology can be compared consistently at the synthesis/metadata layer, not to overwrite what a source actually said.

## Usage rules

- Preserve the source's original wording in extraction prose.
- When a source uses a synonym or alternate phrasing, map it to the canonical glossary term where appropriate.
- Prefer canonical glossary terms in metadata, evidence synthesis, and project-level writing.
- Use Obsidian wikilinks to canonical glossary notes when they improve navigation or disambiguation.
- Do not force a mapping if the source uses a term in a materially different technical sense.
- If a genuinely distinct concept appears that is not covered by the glossary, flag it for glossary review before creating a new note.
- Do not create duplicate synonym notes; add aliases to the canonical glossary note instead.
- Foundational equations in glossary notes are conceptual aids only and must not be used to infer or back-calculate unreported study parameters.
- When terminology is ambiguous, preserve the original source wording and record the ambiguity rather than normalizing aggressively.

## Key distinctions to check when reading a new source

These pairs are easy to conflate; each is addressed explicitly in the relevant notes' "Common pitfalls"/"Common confusion" sections:

- [[03 Concepts/Glossary/Power]] vs [[03 Concepts/Glossary/Energy]]
- [[03 Concepts/Glossary/Set Power]] vs [[03 Concepts/Glossary/Measured Power]]
- [[03 Concepts/Glossary/Average Power]] vs [[03 Concepts/Glossary/Peak Power]]
- [[03 Concepts/Glossary/Optical Frequency]] vs [[03 Concepts/Glossary/Frequency]] (pulse repetition rate)
- [[03 Concepts/Glossary/Irradiance]] vs [[03 Concepts/Glossary/Fluence]]
- [[03 Concepts/Glossary/Fiber Diameter]] vs [[03 Concepts/Glossary/Spot Size]]
- [[03 Concepts/Glossary/Incision Speed]] vs [[03 Concepts/Glossary/Procedure Time]] / [[03 Concepts/Glossary/Excision Time]]
- [[03 Concepts/Glossary/Thermal Damage]] vs [[03 Concepts/Glossary/Margin Quality]]
- Technical ex vivo cutting characterization vs [[03 Concepts/Glossary/Biopsy-oriented]] specimen-quality assessment

## Related

- Template: [[99 Templates/Glossary Term Template]]
- Broader, evidence-grounded concept notes: [[03 Concepts/Power Output]], [[03 Concepts/Power Loss]], [[03 Concepts/Operating Parameters]], [[03 Concepts/Laser Presetting]]
- Schema: [[99 Templates/Study Metadata Schema]]
- Main research hub: [[01 Projects/Diode Laser Master]]
- Biopsy research hub: [[01 Projects/Diode Laser Biopsy]]
- [[06 Synthesis/Study Dashboard]], [[06 Synthesis/Novelty Matrix - Diode Laser Biopsy]]
