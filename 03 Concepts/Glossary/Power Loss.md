# Power Loss

## Definition

The reported discrepancy between a laser's set/panel power and its measured or delivered output, usually expressed as a percentage of the set value. NEEDS VERIFICATION: no single authoritative definition unifies this clinical usage with the stricter optics/engineering usage, where "power loss" (or "insertion loss," "transmission loss") refers specifically to attenuation of optical power as it passes through a medium or component, typically reported in dB. In the dental-diode literature reviewed in this vault, "power loss" is used more loosely to mean any set-vs-measured discrepancy, regardless of its physical cause (transmission loss, tip fouling, diode inefficiency, calibration error), and sources do not always specify which meaning they intend.

## นิยามภาษาไทย

การสูญเสียกำลัง (Power Loss) หมายถึงส่วนต่างระหว่างกำลังที่ตั้งไว้ที่หน้าปัดกับกำลังที่วัดได้จริงหรือส่งถึงเป้าหมาย มักแสดงเป็นเปอร์เซ็นต์ของค่าที่ตั้งไว้ ยังไม่มีนิยามมาตรฐานเดียวที่ครอบคลุมทั้งความหมายทางคลินิกนี้กับความหมายที่เคร่งครัดกว่าในทางวิศวกรรมเชิงแสง (การลดทอนกำลังแสงขณะเดินทางผ่านตัวกลาง/อุปกรณ์ มักรายงานเป็น dB) — ในวรรณกรรมที่ทบทวนในคลังนี้ คำนี้ถูกใช้อย่างกว้าง หมายถึงส่วนต่างระหว่างค่าตั้งกับค่าที่วัดได้ไม่ว่าจะเกิดจากสาเหตุใด (NEEDS VERIFICATION)

## Formula

% loss = (Set Power − Measured Power) / Set Power × 100. Caution: the sign convention is not standardized across sources — some report only an unsigned "loss" percentage (implicitly assuming measured < set), while others (e.g., Xue et al. 2022, Kim et al. 2020) report signed deviations that can be positive (measured > set).

## Unit

% (dimensionless); sometimes also an absolute power difference (W).

## In this vault

Directly the subject of [[04 Evidence/Power Loss and Deviation Across Dental Diode Devices]] and [[03 Concepts/Power Loss]]. Sources disagree on direction: Parker et al. 2022 and Zegaib et al. 2011 report predominantly below-panel output; Xue et al. 2022 and Kim et al. 2020 report both above- and below-panel deviations depending on device. [[07 Data/Zegaib et al 2011 - Fiber Tip Power Loss During Periodontal Curettage]]'s own stated "54%" loss figure does not arithmetically match its own Table 1 data (~46%) — preserved as an unresolved internal inconsistency, not corrected by this vault.

## Common confusion

Do not confuse "power loss" (the set-vs-measured/delivered discrepancy meant in this vault) with optical "insertion loss" or "transmission loss" (a physical property of a fiber/component itself, typically dB, independent of any specific laser's set-point). Also distinguish a single-measurement calibration discrepancy from a repeated-use/degradation phenomenon — this vault's sources mix both without always labeling which they mean; see [[06 Synthesis/Research Gaps in Dental Diode Laser Output]].

## Source basis

**Classification:** VAULT-DEFINED TERM (non-standardized)

Optical engineering has a standardized adjacent concept — "insertion loss"/attenuation (dB), defined in IEC 61300-3-4 (*Fibre optic interconnecting devices and passive components — Attenuation*) — but that measures transmission loss through a fiber/component, not a set-point-vs-measured-output discrepancy. No ISO/IEC laser vocabulary standard, ANSI Z136 edition, or PBM dosimetry reference defines "power loss" in the set-vs-measured sense used throughout this vault, consistent with the NEEDS VERIFICATION flag already in the Definition above. Kept marked non-standardized per vault policy.

## Related

- [[03 Concepts/Glossary/Set Power]]
- [[03 Concepts/Glossary/Measured Power]]
- [[03 Concepts/Glossary/Delivered Power]]
- [[03 Concepts/Power Loss]] (vault concept note, evidence-grounded)
