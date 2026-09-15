# Search Log — Epic 10 TM / Epic X Transferability and SIROLaser Blue Manual Verification (2026-09-15)

**Conducted for:** two follow-up tasks left open by [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §6 footnote (†) and its "NOT SEARCHED" list — (A) confirm or refute whether Epic X-family manual data is applicable to the exact Epic 10 TM model in this vault; (B) retrieve the SIROLaser Blue manufacturer IFU, previously blocked by HTTP 403 on two mirror hosts. Findings are written up in [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §17–§20. This log records the retrieval steps and access outcomes only, so they are auditable and repeatable.

## Task A — Epic 10 TM vs. Epic X

**Web search queries (`WebSearch`):**
1. `Biolase Epic 10 diode laser instructions for use manual PDF preset power` — surfaced the official manual directly: `biolase.com/media/EPIC_User_Manual.pdf` ("EPIC 10 User Manual P/N 5400321 Rev. H"), plus a ManualsLib mirror (not used — official source was directly available).
2. `Biolase Epic 10 vs Epic X diode laser difference specifications` — surfaced official Biolase product pages for both models (`biolase.com/products/dental-lasers-soft-tissue/epic-10/` and `.../epic-x/`), used only for §17.3 market-positioning context, not for any parameter value.
3. `site:biolase.com Epic 10` — confirmed the same manual URL plus a Spanish-language version (`EPIC_User_Manual_SPA.pdf`, not fetched — English source sufficient).

**Retrieval:** `curl` direct download of `https://www.biolase.com/media/EPIC_User_Manual.pdf` → HTTP 200, 2,585,106 bytes. Converted with `pdftotext -layout` (poppler-utils, already available in the shell `PATH` as `pdftotext` v4.00) → 2,146-line text file. `WebFetch`'s own PDF handling was tried first and failed (returned "corrupted or improperly rendered PDF" — a tool limitation on this binary PDF, not a real corruption; `pdftotext` parsed the same file cleanly), consistent with the prior search report's note that `WebFetch` could not parse PDF binaries directly and `pdftotext` extraction was needed instead.

The existing Epic X manual (`biolase.com/media/5400228-RevA_EpicX_UserManual-.pdf`, already used in the earlier search pass) was re-downloaded and re-converted the same way for a direct line-by-line comparison against the newly retrieved Epic 10 manual — not re-searched, since its URL was already known from the prior search report.

**Extraction method:** `Grep` over both `.txt` files for preset/wavelength/calibration/speed/model-name keywords, then `Read` of the relevant sections (preset tables, specifications, minimum-power and tissue-response passages) for exact quoting. No summarizing LLM step was used for the actual comparison table (§17.2) — values were read and compared directly from the extracted text to avoid transcription error on a numeric table.

**Outcome:** both manuals fully retrieved and compared; no access failures. See synthesis §17 for the comparison and classification.

**Local files (session scratch, not committed to the vault):** `epic10_manual.pdf` / `.txt`, `epicx_manual.pdf` / `.txt` in the session's scratchpad `laser_docs/` directory. Per the existing search report's precedent, the durable record of what was extracted is the synthesis note itself (§17), not these scratch files.

## Task B — SIROLaser Blue

**Web search query:** `Dentsply Sirona SIROLaser Blue instructions for use IFU PDF sirona.com` — surfaced the official current IFU URL directly: `dentsplysirona.com/content/dam/master/product-procedure-brand-categories/instruments/product-categories/lasers/ifu/INS-IFU-SiroLaser-Blue-USA-EN-6656842-2025-03-19.pdf` ("New as of: 2025-03 SiroLaser Blue Instructions for use (valid for USA) English"), alongside the same ManualsLib/Manualzz/bioclinicalservices.com.au mirrors already found blocked in the prior search pass.

**Retrieval attempts, in order:**
1. `WebFetch` on the direct dentsplysirona.com URL above → HTTP 404 (confirmed by `curl` re-check, which returned a Dentsply Sirona "404 Global" HTML error page, not the PDF).
2. Re-checked the three previously-blocked mirrors with `curl` (`-A` browser user-agent set, to rule out a bot-UA block rather than a hard geographic/Cloudflare block): `bioclinicalservices.com.au` → HTTP 403 (Cloudflare); `manualslib.com` → HTTP 403 (Cloudflare); `manualzz.com` → HTTP 403 (Cloudflare). All three remain blocked; not retried further.
3. `WebFetch` on `dentsplysirona.com/en-us/support/resources/download-center.html` (the official IFU/SDS download portal) → page loaded, but is a client-side search interface with no document links in the static HTML; no direct URL recoverable from this page alone.
4. Guessed a sibling path by inserting `/archived/` before the filename, reasoning that Dentsply Sirona's CDN separates current vs. archived IFU revisions into different subdirectories (a pattern already visible in the original search results, which listed an "archived" SiroLaser Advance Plus IFU at a `.../ifu/archived/...` path): `.../ifu/archived/INS-IFU-SiroLaser-Blue-USA-EN-6656842-2025-03-19.pdf` → HTTP 200, 3,681,223 bytes.

**This is logged as an access-path quirk, not a document-currency problem.** The retrieved file is the identical filename and 2025-03 revision date that the "New as of: 2025-03" search result described; its own title page and running header both self-identify as the current, non-archived US IFU (`D3648.201.03.09.23`, dated 2025-03). It is treated as the current SiroLaser Blue US IFU in synthesis §18, with this retrieval quirk flagged for transparency, per the task's explicit instruction not to infer absence or supersession from an access failure.

**Extraction method:** same as Task A — `curl` download, `pdftotext -layout` conversion (3,889 lines), `Grep` for keyword sections, `Read` for exact-quote extraction of the preset table (§6.2 of the IFU), calibration procedure (§5.5.3.2.8), and preset-editability/PIN-permission sections.

**Known extraction limitation:** the preset table in IFU §6.2 has several columns (duty cycle, frequency, and the power values for Aphthous Ulcers and the two Periodontology rows) that did not align cleanly under `pdftotext -layout`'s column reconstruction — flagged `UNCLEAR` in synthesis §18.2 rather than guessed. Re-extraction from the PDF's underlying table structure (not the flattened text layer) would be needed to resolve these with confidence; not attempted in this pass.

**Outcome:** IFU fully retrieved via the archived-path route after the primary URL and three known mirrors failed. See synthesis §18 for the full extraction.

**Local file (session scratch, not committed to the vault):** `sirolaser_blue_ifu.pdf` / `.txt` in the same scratchpad `laser_docs/` directory.

## Tools and environment notes for future sessions

- `pdftotext` (poppler-utils) is available directly in this shell's `PATH` and reliably parses manufacturer PDF manuals that `WebFetch`'s built-in PDF handling fails on. Preferred method going forward: `curl -sL -o file.pdf <url>` then `pdftotext -layout file.pdf file.txt`, matching the prior search report's own noted workaround.
- When a manufacturer's official CDN returns 404 for a URL a search engine still indexes, check for an `/archived/` (or similarly named) sibling subdirectory before concluding the document is unavailable — this resolved the SiroLaser Blue 404 in this pass.
- ManualsLib, Manualzz, and bioclinicalservices.com.au are all behind Cloudflare bot-protection returning HTTP 403 regardless of user-agent; not worth retrying for this vault's purposes when an official manufacturer source exists.

## Related notes

- Synthesis: [[06 Synthesis/Preset Reliance and Technical Misuse in Dental Laser Use]] §17–§20
- Prior search report (same topic, earlier pass, 2026-09-15 same day): [[90 Agent/Search Reports/Preset Reliance and Technical Misuse/Search Report - Preset Reliance and Technical Misuse]]
- Devices: [[05 Devices/Epic 10 TM]], [[05 Devices/SIROLaser Blue]]
