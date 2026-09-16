# Search Log — Gemini EVO and SOL Manual Verification (2026-09-16)

**Conducted for:** an independent full-text verification pass on Gemini EVO and SOL manufacturer-manual claims that had first surfaced via a broader `paper-search-pro` academic-literature search (WebSearch snippets + a subagent's own manual retrieval, not independently confirmed at the time). This log records only the verification retrieval; findings are written up in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] under "Follow-up (2026-09-16): Gemini EVO and SOL manufacturer manuals."

## Gemini EVO

**Web search query (`WebSearch`):** `Ultradent Gemini EVO diode laser manual IFU preset procedure settings` — surfaced two manufacturer-hosted PDFs directly from `ctfassets.net` (Ultradent's CDN): a large "International IFU" (`Gemini-EVO-Diode-Laser-International-IFU-1010399AR02.pdf`) and a smaller US-market manual (`Gemini-EVO-Laser-IFU-1010000AR02.pdf`).

**Retrieval attempts:**
1. `WebFetch` on the International IFU (1010399AR02) → failed: `maxContentLength size of 10485760 exceeded` (file too large for WebFetch's fetch limit). Not retried at this URL.
2. `WebFetch` on the smaller US manual (1010000AR02) → tool returned successfully but its built-in summarizer reported it could not extract readable text ("heavily compressed... binary image and stream data"), despite saving the binary PDF (5.5MB) to a local cache path.
3. `Read` tool attempted on the saved PDF with a page range → failed: `pdftoppm is not installed` (page-image rendering unavailable in this environment).
4. **Resolution:** `pdftotext -layout` (poppler-utils, confirmed present in the shell `PATH`) run directly against the locally cached PDF from step 2 → succeeded, producing a clean 151,427-character / 2,426-line text file. `WebFetch`'s own PDF-to-text path evidently failed on this particular file where the underlying binary was intact and `pdftotext` parsed it without issue — a tool-specific limitation, not a corrupted or image-only source document.

**Extraction method:** `Grep` over the extracted `.txt` for preset/wavelength/recommendation/tolerance/calibration/fiber/speed/provenance keywords, then `Read` of the relevant sections (preset table, customization procedure, system specifications, procedural-recommendations/guideline section) for exact quoting. No summarizing step was used for quoted claims — text was read and copied directly.

**Known extraction limitation:** the 16-row preset table (`PRESET PROCEDURE SETTINGS AND CUSTOMIZATION`, page 19) did not survive `pdftotext -layout`'s column reconstruction cleanly for 8 of the 16 named procedures (Hemostasis, Debridement, Gingivectomy, Frenectomy, Pulpotomy, Troughing, and two others) — power values are present in the source table but not legibly recoverable in this text extraction. Flagged `UNKNOWN (extraction artifact)` rather than guessed at. Re-extraction would require visual/page-image rendering (`pdftoppm`), unavailable in this environment.

**Not retrieved/reviewed in this pass:** the larger International IFU (1010399AR02) — exists at Ultradent's CDN but was not successfully fetched or mined; all Gemini EVO claims in the synthesis note trace only to the 1010000AR02 US manual.

## SOL

**Web search query (`WebSearch`):** `DenMat SOL diode laser user manual preset settings dental` — surfaced two independently hosted copies of the same underlying IFU (same Den-Mat document number 823059600), at different revisions:
1. `https://media.brasselerusa.com/userfiles/IFU,Manuals,Brochures/SOL%20Desktop%20Laser%20DFU.pdf` — cover reads "SOL Portable Diode Laser," document 823059600 **Rev 8, 10/23** (Oct 2023).
2. `https://universadent.com/wp-content/uploads/2021/05/SOL-Laser-Universadent.pdf` — cover reads "SOL Laser" (different cover name, same underlying device), document 823059600 **Rev 6, 01/20** (Jan 2020).

**Retrieval:** `WebFetch` on both URLs; both returned successfully but, as with Gemini EVO, the built-in summarizer could not extract readable text from the raw fetch. Both binaries were cached locally and converted with `pdftotext -layout` → 107,802 characters (Rev 8, primary) and 73,958 characters (Rev 6, secondary), both cleanly parsed with no column-alignment issues in the preset table.

**Extraction method:** same as Gemini EVO — `Grep` for keyword sections in the Rev 8 (2023, primary) text, `Read` for exact-quote extraction of the Smart Presets table, the calibration/power-verification section, and the procedural-guidelines/provenance paragraph.

**Rev 6 (2020) vs. Rev 8 (2023):** confirmed to be two revisions of the same document number, ~3.5 years apart, with a different cover device-name ("SOL Laser" vs. "SOL Portable Diode Laser"). **Not diffed line-by-line** — all SOL claims in the synthesis note trace to the Rev 8 (2023) text only; the existence of the older Rev 6 copy is noted but its content is not asserted to be identical, per the task's instruction not to infer beyond documents actually reviewed.

**Manufacturer-identity note:** both SOL IFU copies retrieved in this pass identify the manufacturer as "Den-Mat Holdings, LLC," 1017 W. Central Ave., Lompoc, CA 93436 USA. This vault's existing [[05 Devices/SOL]] note (sourced from Romeo et al. 2014) attributes the device to "DenMat Italia, Italy." Both are recorded in the device note as an unresolved discrepancy — not reconciled by assumption in this pass (e.g., no assumption that one is a regional distributor/subsidiary of the other).

## Tools and environment notes for future sessions

- Confirms the prior search log's (2026-09-15) finding: `pdftotext -layout` (poppler-utils) is available in this shell's `PATH` and reliably parses manufacturer PDF manuals that `WebFetch`'s own PDF-to-text handling fails on, even for files that are not actually image-only or corrupted.
- `pdftoppm` (page-image rendering, needed for the `Read` tool's PDF-page-viewing mode) is **not** installed in this environment — any manual whose table structure doesn't survive `pdftotext -layout`'s column reconstruction cannot currently be resolved by visual inspection; flag as an extraction artifact rather than a missing value.
- `WebFetch`'s content-length cap (10,485,760 bytes / 10MB) blocks retrieval of larger manufacturer PDFs (e.g., Gemini EVO's International IFU) outright; no workaround attempted in this pass beyond falling back to the smaller regional manual.

## Related notes

- Synthesis: [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]], "Follow-up (2026-09-16): Gemini EVO and SOL manufacturer manuals"
- Prior search logs (same topic): [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Report - Preset Reliance and Technical Misuse]], [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Log - Epic 10 and SIROLaser Blue Manual Verification 2026-09-15]]
- Devices: [[05 Devices/Gemini Evo]], [[05 Devices/SOL]]
