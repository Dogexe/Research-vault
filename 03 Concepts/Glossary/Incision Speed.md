---
aliases: [Cutting Speed, Advancement Speed]
category: laser-operation
unit: mm/s
symbol: v
equation:
related_terms: [Procedure Time, Excision Time, Power-to-Speed Relationship, Energy per Unit Length]
---

# Incision Speed

## Definition

The rate at which the laser fiber tip is moved across or through tissue during an incision, typically reported qualitatively (e.g., "slow," "fixed") or in mm/s; a delivery-technique parameter distinct from the laser's power or energy setting, but one that co-determines the energy actually deposited per unit tissue length/area alongside power and spot size. According to PubMed-indexed vault data, Al-Ani et al. report a "fixed exposure duration/incision speed" as part of their operating-parameter protocol for a dual-wavelength diode laser used in oral soft-tissue incisions ([[07 Data/Al-Ani et al 2023 - Dual-Wavelength Diode Operating Parameters]]; source: Al-Ani AJ, Al-Alawi AS, Taher HJ. "Analysis of the Temperature Elevation of the Dual-Wavelength Diode Laser and the Er, Cr: YSGG Laser in Oral Soft Tissue Incisions." *J Lasers Med Sci.* 2023;14:e37. DOI: [10.34172/jlms.2023.37](https://doi.org/10.34172/jlms.2023.37)).

## นิยามภาษาไทย

Incision speed (ความเร็วในการตัด) คืออัตราที่ปลายไฟเบอร์เลเซอร์เคลื่อนที่ผ่านเนื้อเยื่อระหว่างการตัด มักรายงานเชิงคุณภาพ (เช่น "ช้า" "คงที่") หรือเป็นหน่วย mm/s เป็นพารามิเตอร์ด้านเทคนิคการใช้งานที่แยกจากค่ากำลังหรือพลังงานของเลเซอร์ แต่ร่วมกำหนดปริมาณพลังงานที่ส่งจริงต่อหน่วยความยาว/พื้นที่เนื้อเยื่อ ร่วมกับกำลังและขนาดจุดโฟกัส

## In this vault

[[03 Concepts/Operating Parameters]] already records Al-Ani et al.'s incision-speed control as FACT. NEEDS EVIDENCE for any vault source that varies incision speed as an independent variable and measures its effect on thermal damage or specimen histologic quality — no source currently in this vault does this.

A second numeric diode incision-speed value now exists: Li et al. 2022 reports a fixed "tip movement speed" of 1 mm/s for a 300 μm, 3.0 W pulsed diode laser in a mouse oral-mucosa wound model ([[07 Data/Li et al 2022 - Diode vs Er-YAG vs Cold Scalpel Mice Oral Mucosa Data]]), alongside the vault's existing Goharkhay et al. 1999 value (10 mm/s, ex vivo pig mandible, different device). Speed was held fixed in both sources, not varied as an independent variable, and the two values are not transferable to each other (different device, species, and tissue context) or to any diagnostic-biopsy source in this vault — the NEEDS EVIDENCE gap above is unchanged.

## Advancement speed as an alias

[[07 Data/Romanos et al 2013 - Diode Laser Soft-Tissue Surgery Review Data|Romanos et al. 2013]]'s own extraction table row is literally labeled "Incision/advancement speed" for its 5-point tested sweep (12.5, 6.0, 3.0, 1.0, 0.0 mm/s); [[07 Data/Lu et al 2026 - Dual-Wavelength 980-1470 nm Liver Cutting Parameters Data (Abstract-Level)|Lu et al. 2026]] (non-oral, cited here only for the terminology) similarly reports a fixed "fiber advancement speed." This vault treats "advancement speed" as the same concept as incision speed, not a distinct one — both describe the fiber tip's rate of travel through tissue.

## Common confusion

Incision speed is an operator/technique-dependent variable, not a device setting — it is not reported by any of this vault's power-deviation sources (Parker, Xue, Zegaib, Kim), because those studies measure static fiber-tip output rather than a moving incision.

## Source basis

**Classification:** FIELD-USAGE TERM

A technique parameter, not itself a radiometric quantity — unlike [[03 Concepts/Glossary/Irradiance]] or [[03 Concepts/Glossary/Fluence]], it has no ISO/ANSI radiometric definition, though it modulates the effective dose delivered per tissue location.

## Incision speed vs. procedure/excision time

Incision speed (mm/s, the fiber tip's rate of advancement through tissue) must not be confused with, or derived from, [[03 Concepts/Glossary/Procedure Time]] or [[03 Concepts/Glossary/Excision Time]] — total elapsed durations that include non-cutting time (positioning, hemostasis, multiple passes, pauses). Per the Study Metadata Schema's `incision_speed_reported`/`speed_mm_s` fields, this vault records a numeric speed only when the source itself states it as a value; dividing incision length by procedure/excision time to back-calculate a speed is explicitly disallowed (see [[99 Templates/Study Metadata Schema]] and AGENTS.md).

## Related

- [[03 Concepts/Operating Parameters]]
- [[03 Concepts/Glossary/Fluence]]
- [[Thermal Damage]]
- [[03 Concepts/Glossary/Procedure Time]]
- [[03 Concepts/Glossary/Excision Time]]
- [[03 Concepts/Glossary/Power-to-Speed Relationship]]
