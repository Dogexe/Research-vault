\# Diode Laser Research Vault



This vault is a scientific research workspace focused on:



\- Diode lasers in dentistry

\- Laser presetting

\- Power output

\- Power losses

\- Operating parameters



\## Core Rules



1\. Never invent citations.

2\. Never invent or infer missing laser parameters.

3\. If a value is not reported, write `UNKNOWN`.

4\. Preserve source links whenever possible.

5\. Separate:

&#x20;  - FACT = directly reported by source

&#x20;  - INTERPRETATION = derived from evidence

&#x20;  - HYPOTHESIS = requires testing

6\. Do not overwrite original literature data without explicit evidence.

7\. Prefer updating existing notes over creating duplicates.

8\. Keep changes minimal and reviewable.



\## Language



This vault is bilingual: English + Thai.



\- Keep in English: technical terms, paper titles, parameter names, units, device names, manufacturer names, and citations.

\- Add concise Thai explanations where useful, alongside the English term.

\- On first mention of a technical term in a note, use the format: `Term (คำแปลภาษาไทย)`. Example: `Power loss (การสูญเสียกำลัง)`.

\- Do not translate literature extraction tables (parameter tables, data tables) unless a Thai label materially improves clarity for a specific field.

\- Thai text must not change scientific meaning, add new claims, or introduce values not present in the source. The FACT / INTERPRETATION / HYPOTHESIS separation applies equally to Thai text.

\- Evidence Note, Concept Note, and Synthesis Note templates include a `## สรุปภาษาไทย` (Thai summary) section: a concise Thai restatement of the note's existing claim or definition, not a new claim.



\## Vault Structure



\- `00 Inbox/` — unprocessed notes

\- `01 Projects/` — active research projects

\- `02 Literature/` — paper, review, guideline, manual, IFU notes

\- `03 Concepts/` — reusable scientific concepts

\- `04 Evidence/` — evidence synthesis

\- `05 Devices/` — device-specific information

\- `06 Synthesis/` — conclusions, contradictions, research gaps

\- `07 Data/` — extracted structured data and tables

\- `90 Agent/` — agent workflows and logs

\- `99 Templates/` — note templates



\## Literature Extraction



When processing a paper, extract when available:



\- device

\- manufacturer

\- wavelength

\- set power

\- measured output power

\- average power

\- peak power

\- operating mode

\- pulse duration

\- frequency

\- duty cycle

\- fiber diameter

\- tip type

\- initiated / non-initiated tip

\- contact / non-contact mode

\- exposure duration

\- measurement method

\- power loss

\- calibration method



Never infer missing values.



\## Glossary Terminology



Before extracting or synthesizing new literature:



\- consult `03 Concepts/Glossary/Glossary Index.md`

\- use canonical glossary terms for normalized interpretation

\- preserve the source's exact terminology in prose

\- do not invent mappings

\- flag new or ambiguous concepts for glossary review



See `03 Concepts/Glossary/Glossary Index.md` for the full terminology policy — do not duplicate it here.



\## Evidence Workflow



Use this flow:



Source → extracted data → claim → evidence → synthesis



## Ingestion Workflow (before extraction)



The actual pipeline that puts a source in front of Claude, upstream of "extracted data" above:



discover/find original source → add original source to Zotero → ZotLit imports source metadata/notes/PDF into Obsidian → Claude reads/extracts → `07 Data/` → `04 Evidence/` → `06 Synthesis/`



Rules:



\- Do not create `07 Data/` directly from a discovered citation, search-result snippet, or random uploaded PDF unless explicitly instructed otherwise.

\- Normal workflow requires the original source to enter through Zotero/ZotLit first.

\- Reviews, textbooks, monographs, and secondary sources may be used for discovery, citation mining, and context.

\- Primary-study metadata and evidence should come from the original primary paper whenever available.

\- If only abstract-level evidence is available, preserve that limitation explicitly.

\- Do not silently promote secondary-source claims into primary-study metadata.



Evidence notes should record:



\- supporting findings

\- conflicting findings

\- limitations

\- uncertainty

\- possible explanations for disagreement

\- research gaps



\## Device Notes



Device notes should separate:



\- manufacturer specifications

\- preset values

\- operating parameters

\- measured output from independent studies

\- reported power losses



Never treat manufacturer claims as independently verified evidence.



\## Scientific Integrity



Every numerical claim should be traceable to a source.



If source quality or interpretation is uncertain, mark:



`NEEDS VERIFICATION`



If sources conflict, preserve the conflict rather than averaging or merging conclusions.



\## Agent Behavior



Before making large structural changes:



1\. inspect the existing vault

2\. reuse existing patterns

3\. avoid unnecessary folders or abstractions

4\. keep diffs small

5\. summarize what changed after completion


\## Workspace Entry Points



\- Active canonical research project: `01 Projects/Diode Laser Biopsy.md`

\- Broader technical/background hub: `01 Projects/Diode Laser Master.md`

\- Note and extraction templates: `99 Templates/`

