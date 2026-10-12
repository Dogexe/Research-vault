# Edit plan: Part 2 → sham in every tongue, Δ = 0.30 (exact McNemar), plus cross-part consistency fixes

Source text: `proposal_accepted_view.md` (same folder). It is the current Google Doc Methods text in "accepted" view, read 2026-10-12. The literature review (§3) and references (§8) are left out.

## Decisions already made (do not re-open)
- Single manufacturer preset for all three Parts.
- Part 1: one-sample TOST, Δ = ±0.5 W. n is calculated after the pilot gives δ and the between-day σ.
- Part 2 (NEW): sham control = the fibre moved along the line with no laser emission. It goes in EVERY tongue: 2 blocks per tongue, random allocation of preset or sham. Sample size uses Δ = 0.30 = pass-proportion difference (preset − sham).
- Part 3: runs only if at least 1 Part-2 preset incision fails the criteria; skipped if 100% pass. When run, all 3 sub-experiments (power, pulse duration, frequency) as the machine allows. Paired McNemar; Part 3 Δ not yet defined.
- Desirable-incision criteria: A2 continuity AND Hohmann carbonisation score ≥ 4. Sham is expected to be A0 → it fails by definition (pass proportion 0).

## Part 2 sample-size calculation (for checking)
- McNemar (Connor 1987): n = [z₁₋α/₂·√ψ + z₁₋β·√(ψ − Δ²)]² / Δ².
- Sham never passes, so every discordant pair is (preset pass, sham fail), which gives ψ = Δ.
- Inputs: α = 0.05 two-sided, power 0.80, Δ = ψ = 0.30.
  - Normal-approx n = 23.7 → 24.
  - Exact check: the exact McNemar (binomial on discordant pairs, all in one direction) needs b ≥ 6 discordant pairs for two-sided p < 0.05 (2·0.5⁶ = 0.031). The smallest n with P(Bin(n, 0.30) ≥ 6) ≥ 0.80 is n = 25.
  - With 10% unevaluable: 25 / 0.9 → 28 tongues (56 blocks/incisions).
- Secondary statement: at n = 28 (or 25 evaluable), the Wilson 95% CI half-width for the preset pass proportion at p̂ = 0.5 is ±0.17 (±0.18).

## A. Existing defects found in the doc (fix regardless)
A1. §2.1 Q1 has a duplicated phrase: "…ที่เลือกศึกษาอยู่ภายในกับกำลังที่แสดงบนเครื่องของ manufacturer-provided surgical preset ที่เลือกศึกษาอยู่ภายในขอบเขต…". Remove the repeat.
A2. §2.2 Obj 1 has a duplicated phrase: "…ของ manufacturer-provided surgical preset ที่เลือกศึกษาของ manufacturer-provided surgical preset ที่เลือกศึกษา". Remove the repeat.
A3. Table 2 problems:
  - It still has columns "ค่าตั้ง B" and "ค่าตั้ง C". The earlier suggested column deletion did not survive.
  - The header reads "ค่าตั้งที่ศึกษาค่าตั้ง A".
  - Fix: delete columns 3–4 and set the header to "ค่าตั้งที่ศึกษา".
A4. The Table 2 caption paragraph is merged with the 6.3 heading into one NORMAL_TEXT paragraph: "ตารางที่ 2 …ในการศึกษา6.3 ส่วนการศึกษาที่ 1–3 และหน่วยทดลอง".
  - Fix: split the paragraph, restore 6.3 as a heading, and put the caption above the table (where Table 1 and Table 3 captions sit).
A5. Part 3 parameter list is inconsistent:
  - §1 last paragraph, §2.1 Q3 and §2.2 Obj 3 say "กำลังหรือความถี่ / power หรือ frequency".
  - 6.1, 6.3, 6.12, 6.14 and §7 have three sub-experiments (power, pulse duration, frequency).
  - Fix: add "ระยะเวลาพัลส์ / pulse duration" in §1, Q3 and Obj 3.
A6. §1 last paragraph does not say a single preset is studied (the earlier suggestion is gone).
  - Fix: "…ค่าตั้งล่วงหน้าจากผู้ผลิตของเลเซอร์ไดโอด 980 นาโนเมตรหนึ่งค่าตั้งในสามส่วน…".

## B. Part 2 edits (sham in every tongue, Δ = 0.30)
B1. §2.1 Q2: append "และสัดส่วนดังกล่าวแตกต่างจากกลุ่มควบคุมที่เคลื่อนปลายใยแก้วนำแสงโดยไม่ปล่อยพลังงานเลเซอร์หรือไม่".
B2. §2.2 Obj 2: append "และเปรียบเทียบสัดส่วนรอยตัดที่ผ่านเกณฑ์ลักษณะรอยตัดที่พึงประสงค์กับกลุ่มควบคุมที่ไม่ปล่อยพลังงานเลเซอร์ (sham)".
B3. 6.1: Part 2 sentence.
  - Replace "การศึกษาเชิงสำรวจ…โดยแต่ละลิ้นให้หนึ่งรอยตัดของค่าตั้ง และมีกลุ่มควบคุมที่ไม่ปล่อยพลังงานเลเซอร์ในลิ้นที่สุ่มเลือก" with:
  - "การศึกษาลักษณะการตัดเนื้อเยื่อทันทีของค่าตั้งล่วงหน้าโดยผู้ผลิตหนึ่งค่าตั้ง เปรียบเทียบแบบจับคู่ภายในลิ้นกับกลุ่มควบคุมที่ไม่ปล่อยพลังงานเลเซอร์ (sham) โดยทุกลิ้นมีสองบล็อกที่สุ่มให้ได้รับค่าตั้งหรือ sham".
B4. Table 1, Part 2 row:
  - Design: "Paired within-tongue comparison: preset vs sham".
  - Unit: "รอยตัดบนบล็อก ลิ้นละ 2 บล็อก (ค่าตั้ง 1, sham 1)".
  - Primary outcome unchanged.
  - Analysis: "สัดส่วนพร้อม 95% CI (Wilson); exact McNemar test เทียบค่าตั้งกับ sham".
B5. 6.2 para 2: Part 2 needs 2 eligible blocks per tongue (was 1, plus 1 more in sham tongues). k ≥ 3 is unchanged because of Part 3.
B6. 6.3 Part 2 paragraph:
  - Every tongue gives 2 blocks; one incision per block.
  - Within each tongue, which block gets the preset or the sham is randomised.
  - Replace the closing sentence "รอยตัดของค่าตั้งมาจากลิ้นละหนึ่งรอยตัด จึงเป็นหน่วยที่เป็นอิสระต่อกัน" with: preset incisions are independent across tongues (one per tongue); preset-vs-sham data are paired within tongue.
B7. 6.4:
  - Intro: "(σ, p และ ψ)" → "(δ, σ และ ψ)", because Part 2 no longer depends on pilot p.
  - Part 2: replace the precision formula/paragraph with the McNemar calculation above. Keep one sentence giving the Wilson ±0.17 precision as a secondary justification.
  - Remove "กลุ่มควบคุมใช้ 1 บล็อกในลิ้นที่สุ่มเลือก 10 ลิ้นจาก 28 ลิ้น รวม 10 บล็อก".
  - EQUATION: the existing precision equation object cannot be edited via the API. Options:
    - (i) keep it, labelled as the secondary precision check, and point to the McNemar equation shown under Part 3;
    - (ii) insert a new McNemar equation through the browser.
    - Preference: (i).
B8. 6.5 item 7:
  - p from the pilot is now descriptive only. ψ is still used for Part 3.
  - Change "เพื่อคำนวณขนาดตัวอย่างของส่วนการศึกษาที่ 2 และ 3 ใหม่" → "เพื่อใช้ประกอบการคำนวณขนาดตัวอย่างของส่วนการศึกษาที่ 3".
B9. 6.7: replace "สุ่มเลือกลิ้น 10 ลิ้นจาก 28 ลิ้นไว้ล่วงหน้า เพื่อเพิ่มบล็อกกลุ่มควบคุมลิ้นละ 1 บล็อก ในลิ้นเหล่านี้สุ่มว่า…" with: every tongue has 1 preset block and 1 sham block; randomise allocation and cutting order within each tongue.
B10. 6.14 Part 2 paragraph:
  - Keep the Wilson CI as the main estimate.
  - Add: preset vs sham with the exact McNemar test (two-sided α = 0.05); report the paired difference in proportions with a 95% CI.
  - Change "จึงไม่มีการเปรียบเทียบระหว่างค่าตั้ง และรอยตัดเป็นอิสระต่อกัน".
  - Sham component outcomes are still reported descriptively.
B11. Table 5, "ส่วนที่ 2 ผลลัพธ์หลัก": replace "กลุ่มควบคุมรายงานเชิงพรรณนาเท่านั้น" with the exact McNemar test vs sham.
B12. 6.14 data-handling: "ส่วนการศึกษาที่ 2 ใช้ลิ้นละหนึ่งรอยตัดของค่าตั้ง จึงไม่ต้องปรับสำหรับ clustering" → reword: preset-vs-sham pairing is handled by McNemar; preset-only estimates use one incision per tongue.
B13. §9 item 3: "ค่า σ, p และ ψ" → "ค่า δ, σ และ ψ".
B14. §7 item 2 (optional): add "เทียบกับกลุ่มควบคุมที่ไม่ปล่อยพลังงานเลเซอร์".

## C. Cross-part consistency issues to FLAG to the user (no edit unless approved)
C1. Part 3 mismatch:
  - Sample size uses pairwise McNemar at α = 0.025 (Bonferroni, 2 pairs).
  - The analysis uses GEE logistic + Holm.
  - Option: make the exact McNemar with Holm the primary pairwise test, with GEE as supportive.
C2. Part 3: there is no multiplicity control across the 3 sub-experiments (6 comparisons total).
C3. The Part 3 Δ is undefined. The projected n per sub-experiment (Δ 0.30, ψ 0.30–0.54, α 0.025) is about 33–62 tongues with 10% added, i.e. potentially 100–180 tongues. That is a feasibility risk.
C4. Part 1 unit is ambiguous: "รอบการวัดหรือวันทดลอง" (Table 1, 6.3, 6.4). The pilot now estimates between-day σ, so the unit should be fixed as "1 รอบการวัดต่อวันทดลอง".
C5. §4 framework (group-authored) still treats the preset as an independent variable and the measured output as a mediator. The advisor flagged the mediator wording. Do not edit; flag only.
C6. Part 2 preset-vs-sham test: the outcome is predictable (sham ≈ 0%). The scientific value is attribution (separating laser effect from mechanical contact) plus assessor blinding, not the p-value. Interpretation text should say so.

## Editing constraints
- All content edits go in as Google Docs SUGGESTIONS (writeMode SUGGEST) via replaceAllText / ranged edits.
- The literature review (§3) is not touched.
- Equations cannot be edited via the API.
