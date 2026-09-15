# Search Report — Preset Reliance and Technical Misuse in Dental Laser Use

**Search date:** 2026-09-15
**Conducted for:** reframing [[01 Projects/Diode Laser Biopsy]] around preset reliability; synthesis at [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]].
**Primary tool:** `paper-search-pro` skill, agent/headless mode (`scripts.agent_search`, OpenAlex primary source, `heuristic_v1` floor relevance scoring). Supplemented with direct PubMed queries (`mcp__plugin_pubmed_PubMed__search_articles`) and general web search/fetch for manufacturer manuals.

This report exists so the searches behind the synthesis note are auditable and repeatable — not to re-argue its conclusions. Raw per-query JSON output is archived under `90 Agent/_Archive/Search Reports/Preset Reliance and Technical Misuse/raw/` (moved out of this folder during Cleanup Batch 3 vault housekeeping; content unchanged) — a human-readable consolidated candidate listing (all 21 queries, sorted by floor relevance score, titles + abstract snippets) remains active in `consolidated_candidates.md` in this same folder.

## Coverage note (read first)

This was a **standard-depth, keyword-driven search**, not an exhaustive systematic review. OpenAlex's full-text index is broad but the `heuristic_v1` floor-relevance score is a coverage heuristic, not a semantic judgment — a large share of returned results for generic queries (e.g. `laser fiber tip power calibration`) were off-topic physics/materials-science literature that happened to share vocabulary ("laser," "fiber," "power," "calibration") with the dental target. Every query below was screened manually against titles and abstract snippets; only genuinely on-topic candidates are cited in the synthesis note. **Absence of a result for a given query is not treated as evidence that no literature exists** — it is recorded as a search-coverage limitation, per the task's explicit instruction.

## 1. OpenAlex queries (via `paper-search-pro` agent-search)

All queries below used `--per-strategy 40 --limit 30` (multi-strategy: cited / recent / relevance, then deduplicated). `raw` = papers retrieved before dedup (typically capped near 120 across three strategies); `dedup` = unique papers after federated dedup; `returned` = top 30 by floor relevance score, saved to the corresponding file, now under `90 Agent/_Archive/Search Reports/Preset Reliance and Technical Misuse/raw/` (see archive note above).

An initial batch of four longer, fully-conjunctive queries (e.g. `"dental laser preset default factory settings parameter selection clinician"`) was attempted first and abandoned after returning 1–3 results each — OpenAlex's full-text search performs poorly on long AND-conjunctions of many specific terms. All subsequent queries were shortened to 3–5 word phrases, which consistently returned ~120 raw results per query. This methodological correction is preserved here rather than deleted, since it affects how future searches in this vault should be phrased.

Two early runs (`domain1_preset_use`, `domain2_knowledge_training`, `domain3_knowledge_to_preset`, `domain5_setpower_vs_delivered`) also hit a `UnicodeEncodeError` on the Windows console (`cp1252` codec choking on a CJK character in the journal-rank payload), which truncated their JSON output before it could be parsed. These were re-run with `PYTHONIOENCODING=utf-8` / `PYTHONUTF8=1` set, which resolved the issue; the truncated files were deleted rather than kept as misleading partial data.

| # | Domain | Query | Raw | Dedup | File |
|---|---|---|---:|---:|---|
| 1a | 1 — preset/default use | `dental laser preset settings` | 120 | 107 | `raw/d1a_preset_settings.json` |
| 1b | 1 — preset/default use | `laser parameter selection dentistry` | 120 | 116 | `raw/d1b_parameter_selection.json` |
| 1c | 1 — guided/expert modes | `guided mode laser dentistry preset` | 120 | 72 | `raw/d1c_guided_mode.json` |
| 2a | 2 — knowledge/training | `dentist knowledge dental laser` | 120 | 108 | `raw/d2a_dentist_knowledge.json` |
| 2b | 2 — knowledge/training | `laser dentistry training survey` | 120 | 110 | `raw/d2b_training_survey.json` |
| 3a | 3 — knowledge gap → preset reliance | `novice preset reliance laser` | 120 | 46 | `raw/d3a_novice_reliance.json` |
| 3b | 3 — knowledge gap → preset reliance | `laser training preset dependence` | 120 | 98 | `raw/d3b_training_dependence.json` |
| 5a | 5 — set vs. delivered power | `diode laser power output measurement dental` | 120 | 114 | `raw/d5a_power_output_measurement.json` |
| 5b | 5 — set vs. delivered power | `laser fiber tip power calibration` | 120 | 116 | `raw/d5b_fiber_tip_calibration.json` |
| 5c | 5 — set vs. delivered power | `dental laser output power meter` | 120 | 115 | `raw/d5c_output_power_meter.json` |
| 6a | 6 — preset validation vs. tissue effect | `laser power histology thermal damage dental` | 120 | 114 | `raw/d6a_power_histology.json` |
| 6b | 6 — preset validation vs. tissue effect | `diode laser cutting efficiency histology` | 120 | 114 | `raw/d6b_cutting_efficiency_histology.json` |
| 6c | 6 — preset validation vs. tissue effect | `recommended laser parameters soft tissue surgery` | 120 | 116 | `raw/d6c_recommended_parameters.json` |
| 7a | 7 — incision speed/technique | `laser incision speed thermal damage` | 120 | 119 | `raw/d7a_incision_speed.json` |
| 7b | 7 — incision speed/technique | `laser cutting speed oral tissue` | 120 | 119 | `raw/d7b_cutting_speed_oral.json` |
| 8a | 8 — technical misuse/operator risk | `dental laser operator error` | 120 | 118 | `raw/d8a_operator_error.json` |
| 8b | 8 — technical misuse/operator risk | `laser thermal injury carbonization dental` | 120 | 114 | `raw/d8b_thermal_injury_carbonization.json` |
| 8c | 8 — technical misuse/operator risk | `inappropriate laser parameters dental injury` | 120 | 104 | `raw/d8c_inappropriate_parameters.json` |
| 9a | 9 — safety/adverse events | `dental laser adverse events safety` | 120 | 112 | `raw/d9a_adverse_events.json` |
| 9b | 9 — medico-legal | `laser dentistry malpractice litigation` | 120 | 44 | `raw/d9b_malpractice.json` |
| 9c | 9 — safety guidance | `laser safety guidelines dentistry` | 120 | 113 | `raw/d9c_safety_guidelines.json` |

**Total: 21 queries, 2,520 raw retrievals, 2,459 unique after per-query dedup** (dedup is per-query against the three retrieval strategies OpenAlex uses internally, not cross-query; the same paper can and does recur across multiple domain queries — e.g. Hanke et al. 2021 and Strakas et al. 2023 surfaced under both domain 6 and domain 7 queries, confirmed by manual review, not re-deduplicated across queries in this pass).

**Deduplication notes:** No cross-query consolidated dedup pass was run (would require federating all 21 raw files through `federated_kg_resolver`, which was not done in this pass — a scope limitation). Manual review during synthesis caught and merged the recurring cross-query hits that mattered (Hanke 2021, Strakas 2023, several general dental-laser reviews appearing under 2–3 different domain queries).

**Citation-chasing seeds:** Formal citation-network expansion (`openalex_helper citation-network`) was **not run** in this pass — a scope limitation given the number of domains already covered by direct search. If resumed, the highest-value seeds for backward/forward citation chasing are: Hanke et al. 2021 (doi:10.1007/s10103-020-03243-4), Strakas et al. 2023 (doi:10.1002/lsm.23639), Al-Ani et al. 2024 (already in vault), and — newly identified in this pass — the Biolase/AMD Lasers/A.R.C. Laser manufacturer manuals themselves have no citation graph (they are not indexed academic works), so citation-chasing does not apply to §6 of the synthesis note.

## 2. PubMed direct queries

Run via `mcp__plugin_pubmed_PubMed__search_articles` (native PubMed query syntax, MeSH-term expansion applied automatically by PubMed's own translator).

| Query | Query translation (PubMed MeSH expansion) | Results |
|---|---|---|
| `(dentist OR dental practitioner) AND (laser parameter OR laser setting) AND (knowledge OR training OR awareness)` | Full MeSH expansion in raw tool output | 13 PMIDs |
| `laser preset OR "default setting" AND dental AND (novice OR training OR experience)` | Full MeSH expansion in raw tool output | **0 results** |

All 13 PMIDs from the first query were retrieved with full metadata (`get_article_metadata`) and reviewed. None was substantively on-topic for dentist knowledge of laser *parameters* specifically — matches were driven by broad OR-expansion pulling in halitosis, TMJ physiotherapy, pediatric dental anxiety, occlusal caries diagnosis, and unrelated topics. One tangential hit (Wigdor 2008, doi:10.1016/j.aodf.2008.07.031, "Basic physics of laser interaction with vital tissue") discusses parameter understanding conceptually but is not an empirical knowledge/training assessment. **The 0-result query is recorded as a direct, confirmed absence for domain 3 (knowledge gap → preset reliance) within PubMed's indexed literature** — see synthesis note §5.

**Coverage gap identified:** The dental-laser awareness/knowledge survey literature that *was* found via OpenAlex (Tanjore 2018, India 2018, South India 2024, "need of the hour" 2020 — see synthesis note §3) did not surface in these PubMed MeSH-driven queries, indicating these venues (Biomedical & Pharmacology Journal, Journal of Dental Lasers, Journal of Pharmacy and Bioallied Sciences) are likely not MEDLINE-indexed, or are indexed under terms this query phrasing did not capture. This is noted as a PubMed indexing/coverage limitation, not as evidence these sources are unreliable.

**No PubMed rate limiting or API failures occurred in this pass.**

## 3. Semantic Scholar / Crossref / arXiv

**Not queried as independent sources in this pass.** `agent_search`'s default engine is OpenAlex, which aggregates Crossref-registered DOI metadata broadly; a separate direct Crossref or Semantic Scholar pass, and formal citation-network expansion via Semantic Scholar's influential-citation-count enrichment, were not run — a scope/budget limitation, not a failure or rate-limit event. arXiv was not queried: this topic (clinical/dental laser use) has no meaningful arXiv presence, and no freshness/preprint signal in the query language justified enabling it per the skill's own routing guidance.

## 4. Manufacturer manual / IFU searches (web search + fetch)

Four `WebSearch` queries were run to locate manufacturer manuals for devices already catalogued in this vault's [[05 Devices/Device Index|05 Devices]] folder:

1. `Biolase Epic 10 diode laser instructions for use preset power settings soft tissue manual`
2. `Dentsply Sirona SIROLaser Blue user manual preset power soft tissue table`
3. `AMD Lasers Picasso diode laser user manual recommended settings power soft tissue`
4. `A.R.C. Laser FOX diode laser manual preset power settings dental`

**Successfully retrieved and read in full text** (PDF → `pdftotext` extraction, since `WebFetch`'s built-in summarizer could not parse the binary PDF stream directly):
- AMD Lasers Picasso Operating Instructions Manual (810 nm, 7 W) — `velopex.com/wp-content/uploads/2017/12/amd-picasso-diode-laser-7w-810nm-operating-instructions-manual-english.pdf`
- A.R.C. Laser FOX User Manual (810/980/1064 nm, rev0, August 2021) — `intern.arclaser.com/fileadmin/arc-laser/intern/ENT/Laser_Technology/Diode_Laser/User_Manuals/User_Manual_FOX_rev0_new_logo.pdf` (general medical-device manual; dental-specific IFU identity not confirmed — see synthesis note §6 footnote)
- Biolase Epic X User Manual (940 nm) — `biolase.com/media/5400228-RevA_EpicX_UserManual-.pdf` (same product family as this vault's Epic 10 TM, not confirmed identical model)

**Blocked / not retrieved:**
- Dentsply Sirona SIROLaser Blue Instructions for Use — two candidate hosts found (ManualsLib, Manualzz), both returned **HTTP 403 Forbidden** on `WebFetch`. Not retried with an alternative method in this pass.
- No manual search was attempted in this pass for: Dentek LD 15, Gemini Evo, K2 Mobile, LITEMEDICS, Quicklase 12W Dual 4, Raffaello, SOL, Saeshin Diode Laser, Wiser 3, Zolar Plus, A.R.C. Laser WOLF (1470 nm). This is a scope limitation of this pass — **absence of a search for these devices is not evidence about their preset provenance.**

Extracted manual text is saved locally (session scratch/tool-results directory, not committed to the vault) as `picasso.txt`, `foxmanual.txt`, `epicx.txt`; the specific quoted passages used are reproduced verbatim in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §6, §8, §9 with page/section context, so the vault synthesis note itself is the durable record of what was extracted.

## 5. Failed / rate-limited APIs

- **HTTP 403** on ManualsLib and Manualzz (SIROLaser Blue manual hosts) — access blocked to the fetch tool, not a rate limit; not retried via an alternative access method in this pass.
- **No rate-limiting** encountered on OpenAlex (agent_search), PubMed, or general WebSearch in this pass.
- **`UnicodeEncodeError`** on four early `agent_search` calls (Windows console `cp1252` default encoding vs. a CJK character in the journal-rank payload) — resolved by setting `PYTHONIOENCODING=utf-8` and `PYTHONUTF8=1`; not a data-source failure, a local environment issue, recorded here so a future session does not need to rediscover it.

## 6. Major coverage limitations (summary)

- Standard-depth keyword search, not an audit-tier/systematic search; no formal PRISMA-S log was generated for this pass (the vault's existing `paper-search-pro` audit-tier run from 2026-09-13, at `90 Agent/Search Reports/diode_laser_oral_biopsy_standard_20260913_171515/`, remains the vault's most systematic prior search and was not repeated here).
- No cross-query consolidated deduplication was performed (§1).
- No citation-network expansion was performed (§1).
- No independent Semantic Scholar, Crossref, or arXiv queries were run (§3).
- Only 3 of 15 catalogued vault devices had their manufacturer manuals searched and retrieved in this pass (§4); the rest are `UNCLEAR` by omission.
- Most abstract-level survey hits in synthesis note §3, §11, and §12 were not verified at full text — several `UNCLEAR` flags in the synthesis note trace back to this and are listed as full-text priorities in the final report to the user.
- The A.R.C. Laser FOX manual's applicability to the specific dental FOX units catalogued in this vault ([[05 Devices/A.R.C. Laser FOX (810 nm)]] etc.) is unconfirmed (general medical-device manual vs. dental-specific IFU).

## Related notes

- Synthesis: [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]]
- Project: [[01 Projects/Diode Laser Biopsy]]
- Prior systematic search (2026-09-13, different topic scope): `90 Agent/Search Reports/diode_laser_oral_biopsy_standard_20260913_171515/`
