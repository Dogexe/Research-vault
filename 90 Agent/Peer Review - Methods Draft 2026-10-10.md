# Peer review ฉบับร่าง — REVIEW-SS2026-METHODS-20261010

> เอกสารทำงานส่วนตัว (ร่างที่ใช้ AI ช่วย) ผู้เขียนโครงร่างต้องตรวจตำแหน่ง การคำนวณ และการอ้างอิงทุกข้อก่อนนำไปใช้

## บันทึกการรับงาน (Intake record)

- เอกสารที่รีวิว: โครงร่างงานวิจัย (ฉบับย่อสำหรับพิจารณาเบื้องต้น) ฉบับร่าง 10 ตุลาคม 2569 — Google Doc "โครงร่าง method"
- สถานะผู้รีวิว: `author_requested_reader` (ผู้เขียนขอให้รีวิว)
- รูปแบบการรีวิว: `open` (รีวิวภายในก่อนส่งอาจารย์ที่ปรึกษา)
- การใช้เครื่องมือ: `approved_ai_assistance` ร่วมกับเครื่องมือ peer-review ของ Scientific Agent Skills ที่รันบนเครื่อง
- ขอบเขต: หัวข้อ 4–7 เท่านั้น ไม่ได้รับบทนำและการทบทวนวรรณกรรมมารีวิว
- ผลเครื่องมือ: intake `READY_FOR_LOCAL_REVIEW`; claim–evidence matrix 11 claims (partly supported 6, unsupported 5); statistics/reproducibility audit 22 รายการ (verified 1, partly documented 16, missing 4, not applicable 1); lint `READY_FOR_HUMAN_REVIEW`

# Comments to authors

(ความเห็นถึงผู้เขียน)

## สรุปงานตามหลักฐานที่มี

การศึกษาเชิงทดลองในห้องปฏิบัติการบนบล็อกชิ้นเนื้อผิวด้านล่างของลิ้นสุกร ใช้เครื่อง Lasotronix SMART M 980 nm หนึ่งเครื่อง กับ manufacturer preset สำหรับตัดเนื้อเยื่ออ่อน 2–3 ค่า

- **ระยะที่ 1** เป็น randomised complete block design (ลิ้น = block) วัด actual output ที่ปลาย fibre และ immediate incision outcomes โดยมี ablative depth จากหน้าตัดสด (25/50/75%) เป็น primary outcome
- **ระยะที่ 2** สุ่มรอยตัดที่ไม่ผ่าน functional cutting endpoint (FCE) เข้ากลุ่มปรับกำลังตามกฎ หรือกลุ่มตัดซ้ำด้วยค่าเดิม
- **Pilot study** (3 ลิ้น) เป็นด่านก่อนเริ่มการศึกษาหลัก

เอกสารนี้เป็นโครงร่าง จึงยังไม่มีผลการศึกษา

## จุดแข็ง

- นิยาม primary outcome ตรงกับคำแนะนำอาจารย์ และระบุชัดว่าไม่ได้เทียบกับ target depth (5.8, ตารางที่ 3)
- ระบุชัดว่า preset ที่ตัดได้ลึกที่สุดไม่ใช่ preset ที่ดีที่สุดหรือปลอดภัยที่สุด (5.11 ข้อ 4)
- ตัวแปรควบคุมในตารางที่ 2 อ้างแหล่งได้ตรง ได้แก่ ความเร็ว ความยาว การลากครั้งเดียว และความตึงจาก ref 12 ส่วนแรงสัมผัส 0.35 g สอดคล้องกับ track force 0.0035 N ของ ref 9
- มี allocation concealment โดยบุคคลอิสระและบันทึก seed ไว้ ระยะที่ 2 ใช้ stratified permuted blocks แบบสลับขนาด (5.5)
- ระยะที่ 2 มีกลุ่ม unadjusted control แบบสุ่ม ทำให้แยกผลของการปรับค่าออกจาก regression to the mean ได้
- กำหนดเกณฑ์ผ่าน pilot ไว้ล่วงหน้า (ICC ≥ 0.75) และมี stop rules (5.9, 5.12)

## ประเด็นหลัก (Major comments)

### Major comment M1

- Location: 5.2 เทียบกับ 5.3, 5.4 และ 5.5 (claim C02)
- Observation: 5.2 วางแผน 2–3 preset แต่ 5.4 ระบุว่าแต่ละลิ้นแบ่งได้ 4 บล็อก "ตามจำนวนค่าตั้งที่ศึกษา" ส่วนระยะที่ 2 ใน 5.5 สุ่ม "บล็อกถัดไปของลิ้นเดียวกัน" ทั้งที่ไม่มีบล็อกเหลือหลังระยะที่ 1
- Evidence or criterion: ความสอดคล้องภายในของ design และ unit of inference
- Why it matters: จำนวนลิ้น จำนวนบล็อกที่ได้ต่อลิ้น ความเป็นไปได้ และ design ระยะที่ 2 ขึ้นกับตัวเลขนี้ทั้งหมด
- Requested action: กำหนดจำนวน preset ให้แน่นอน แล้วระบุว่าบล็อกต่อลิ้น = จำนวน preset + บล็อกสำรองสำหรับระยะที่ 2 จากนั้นยืนยันใน pilot ว่าลิ้นหนึ่งลิ้นแบ่งบล็อก 2 × 1 × 2 cm จากผิวด้านล่างที่ผ่านเกณฑ์ได้ครบจำนวน

### Major comment M2

- Location: 5.4 ย่อหน้า 1–2 (claim C01)
- Observation: แบ่งเป็น 3 ประเด็น
  - สูตร (1) เป็น precision formula สำหรับประมาณค่าเฉลี่ยราย preset แต่ design และตารางที่ 4 เปรียบเทียบระหว่าง preset ด้วย LMM
  - ข้อความระบุว่า U − L ต่างกันประมาณ 200–300 µm แต่ใน ref 14 (ลิ้น, 980 nm) ช่วง CI กว้างประมาณ 420–630 µm ค่า 200–300 µm คือ SD ที่คำนวณย้อนกลับ
  - งานต้นแบบวัดความลึกจาก sealant replica 5 จุด ไม่ใช่หน้าตัดสด และประโยค "การศึกษาก่อนหน้าของกลุ่มวิจัย" ยังไม่มีเลขอ้างอิง
- Evidence or criterion: เหตุผลของขนาดตัวอย่างต้องตรงกับ target quantity และวิธีวิเคราะห์ นอกจากนี้ instruction ของโครงการให้น้ำหนักความใกล้เคียงของวิธีวัดสูงกว่าความยาวคลื่น
- Why it matters: ผู้อ่านคำนวณ σ ซ้ำไม่ได้ precision target ไม่ได้ให้ power สำหรับการเปรียบเทียบที่การวิเคราะห์ตั้งใจทำ และยังไม่ได้คิด clustering จากลิ้น
- Requested action: ปรับ 4 ข้อดังนี้
  - แก้คำเป็น "ครึ่งความกว้างของช่วงความเชื่อมั่น (half-width)" และใส่อ้างอิง ref 14
  - เลือกระหว่างระบุว่าระยะที่ 1 เป็นเชิงพรรณนา (precision-based) หรือเพิ่มการคำนวณแบบเปรียบเทียบสำหรับ RCBD/LMM
  - ระบุว่า n ต่อ preset เท่ากับจำนวนลิ้น
  - วางแผนคำนวณใหม่จาก pilot โดยใช้ upper confidence limit ของ SD

### Major comment M3

- Location: 5.4 ย่อหน้า 3, 5.9, ตารางที่ 4 (claims C03, C09)
- Observation: แบ่งเป็น 4 ประเด็น
  - ระยะที่ 2 ใช้ Fisher's exact test (α = 0.025, power 80%, p = 0.30 vs 0.70) โดยไม่มีแหล่งที่มาของสัดส่วน และไม่ได้อธิบายเหตุผลของ α = 0.025
  - primary outcome คือ FCE ใน "รอยตัดถัดไป" แต่ขั้นตอนอนุญาตให้ปรับได้ถึง 3 ขั้นพร้อม stop rule เรื่อง oscillation
  - ตารางที่ 4 ไม่มีการวิเคราะห์ระยะที่ 2
  - ไม่ได้กำหนดวิธีจัดการเมื่อผลตัดสินหน้างานของผู้ตัดไม่ตรงกับผลของผู้ประเมินที่ถูกปกปิด
- Evidence or criterion: prespecification, analysis–design alignment และ clustering
- Why it matters: ประเมิน claim เชิงยืนยันของระยะที่ 2 ไม่ได้ และเมื่อยังไม่รู้อัตราการไม่ผ่าน FCE ก็คาดจำนวนลิ้นที่ต้องใช้ไม่ได้
- Requested action: เลือกทางใดทางหนึ่ง แล้วเพิ่มแถวการวิเคราะห์ระยะที่ 2 ในตารางที่ 4
  - (ก) design เชิงยืนยัน: ต้องมีสมมติฐานขนาดผลที่มีแหล่งอ้างอิงหรือระบุว่าเป็นสมมติฐานของผู้วิจัย, α ที่มีเหตุผล, การวิเคราะห์ข้อมูล binary ที่คิด clustering (GEE หรือ mixed logistic model), outcome timepoint ที่ตายตัว และ analysis set ที่กำหนดไว้ล่วงหน้า
  - (ข) descriptive pilot ตั้งแต่ต้น ซึ่งสอดคล้องกับคำแนะนำอาจารย์ข้อ 12

### Major comment M4

- Location: หัวข้อ 4 เทียบกับตารางที่ 4 (claims C07, C11)
- Observation: เลขวัตถุประสงค์ในตารางที่ 4 ไม่ตรงกับหัวข้อ 4 แถวที่ 4 (correlation และ simple linear regression เพื่อทำนายความลึกจาก actual output) ไม่มีวัตถุประสงค์รองรับ ส่วนวัตถุประสงค์ข้อ 1 ระบุ "การเปลี่ยนแปลงระหว่างวันทดลอง" แต่ 5.6 ไม่ได้ระบุการวัด reference ซ้ำรายวัน และตารางที่ 4 วิเคราะห์เฉพาะก่อนเทียบหลังชุดการทดลอง
- Evidence or criterion: ทุกวัตถุประสงค์ต้องมีการวิเคราะห์ และทุกการวิเคราะห์ต้องมีวัตถุประสงค์
- Why it matters: เครื่องเดียวกับ 2–3 preset ทำให้ actual output มีเพียง 2–3 กลุ่มค่า E_L = P/v ที่ v คงที่ไม่ได้เพิ่มข้อมูล และ preset ที่ต่างกันที่ emission mode ทำให้ผลของวัตต์ถูกรบกวน สมการทำนายจึงขัดกับหลักของโครงการที่ห้ามตีความจากวัตต์อย่างเดียว
- Requested action: จัดเลขให้ตรงกัน ตัด predictive regression ออก หรือลดเป็น exploratory covariate ภายใน preset ใน LMM และเพิ่มการวัด reference รายวันพร้อมการวิเคราะห์ หรือตัดคำว่า "ระหว่างวัน" ออกจากวัตถุประสงค์ข้อ 1

### Major comment M5

- Location: ตารางที่ 4 แถว 2–3 (analysis.method_design_alignment)
- Observation: พบ 6 จุด
  - ทางเลือกเมื่อข้อมูลไม่แจกแจงปกติมี Kruskal–Wallis ซึ่งไม่คิด block
  - ทดสอบ normality กับข้อมูลดิบ
  - ระบุ McNemar ทั้งที่อาจมี 3 preset
  - ค่าความลึก 0 เมื่อไม่เกิดรอยตัดถูกรวมกับค่าความลึกจริง
  - ยังไม่เลือก primary depth summary (ค่าเฉลี่ยหรือค่าสูงสุดของ 3 หน้าตัด)
  - ไม่ได้ระบุวิธีปรับ multiplicity สำหรับ pairwise comparison
- Evidence or criterion: หลักการวิเคราะห์ RCBD และ prespecification
- Why it matters: การทดสอบทางเลือกที่ไม่ถูกต้องและค่าศูนย์ที่กองรวมกัน (point mass) อาจทำให้การเปรียบเทียบความลึกเอนเอียง
- Requested action: ปรับ 4 ข้อดังนี้
  - ใช้ Friedman test (หรือ LMM กับข้อมูลที่แปลงค่า) เป็นทางเลือก และตรวจ normality ที่ residual ของ model
  - ใช้ Cochran's Q หรือ GEE เมื่อมีมากกว่า 2 preset
  - วิเคราะห์ความลึกเฉพาะชิ้นที่เกิดรอยตัด และรายงานอัตราการเกิดรอยตัดแยกต่างหาก
  - กำหนดค่าเฉลี่ย 3 หน้าตัดเป็น primary และระบุวิธีปรับ multiplicity

### Major comment M6

- Location: ตารางที่ 3 แถว carbonisation และหัวข้อ 6 ข้อ 1 (claims C06, C10)
- Observation: carbonisation ที่เห็นจากภาพถ่ายด้านบนถูกเรียกว่า "safety boundary" และผลที่คาดว่าจะได้รับข้อ 1 อ้างถึง "ค่าตั้งล่วงหน้าที่ใช้ในสถานบริการ"
- Evidence or criterion: หลักของโครงการระบุว่า visible thermal effect ไม่เท่ากับ histological thermal damage และขอบเขตการศึกษาคือเครื่องเดียว
- Why it matters: สื่อเกินกว่าที่การวัดและการสุ่มตัวอย่างรองรับ
- Requested action: เปลี่ยนเป็น "เกณฑ์ขอบเขตผลความร้อนที่มองเห็นได้ (visible thermal-effect criterion) ซึ่งไม่ใช่การประเมินทางจุลพยาธิวิทยา" และจำกัดผลที่คาดว่าจะได้รับให้อยู่ที่เครื่องและ preset ที่ศึกษา

## ประเด็นรอง (Minor comments)

### Minor comment m1

- Location: 5.6 ย่อหน้า 2 (claim C04)
- Observation: เกณฑ์ความต่าง ≥ 5% แล้วตัดปลาย fibre ใหม่ อ้าง ref 14 และ 15
- Evidence or criterion: ref 14 ไม่ได้วัด actual output ส่วน ref 15 เป็น systematic review ด้านจุลพยาธิ เกณฑ์นี้รายงานใน ref 9 (และ ref 8)
- Why it matters: อ้างอิงผิดแหล่ง
- Requested action: เปลี่ยนเป็น ref 8 และ 9

### Minor comment m2

- Location: ตารางที่ 2 แถว fibre และ 5.6
- Observation: วัด output หลัง cleave แต่ก่อน initiate ทั้งที่การ initiate เปลี่ยนการปลดปล่อยพลังงานที่ปลาย fibre
- Evidence or criterion: ตำแหน่งและจังหวะการวัดเป็นตัวกำหนดว่า "actual output" หมายถึงอะไร
- Why it matters: ค่าที่วัดได้ไม่ใช่ output ขณะตัดจริง
- Requested action: ระบุและให้เหตุผลว่าวัดเมื่อใด หรือวัดทั้งสองจุด และบันทึกว่า thermal sensor รายงานเป็น average power สำหรับ preset แบบพัลส์

### Minor comment m3

- Location: ตารางที่ 2 แถวแรงสัมผัส (claim C05)
- Observation: การบันทึกแรง 0.30–0.40 g ตลอดการลากต้องใช้ load cell ที่ละเอียดกว่า 0.05 g ซึ่งยังไม่ได้ระบุอุปกรณ์ ref 9 ตรวจแรงทุก 5 รอยตัดด้วยรอยหมึก และเครื่องควบคุมความเร็วของกลุ่มเป็นแบบควบคุมตำแหน่ง
- Evidence or criterion: ความเป็นไปได้และความตรงกับแหล่งที่อ้าง
- Why it matters: อาจควบคุมตามที่เขียนไม่ได้จริง
- Requested action: ระบุอุปกรณ์และความละเอียด หรือเปลี่ยนเป็นการตรวจเป็นระยะแล้วรายงานเป็นข้อจำกัด และทดสอบใน pilot ข้อ 1

### Minor comment m4

- Location: ตารางที่ 3 immediate tissue endpoint
- Observation: กลุ่มทับซ้อนกัน (รอยตัดไม่ต่อเนื่อง + คาร์บอนระดับ 2) และกลุ่ม 3 ฝังเกณฑ์คาร์บอนไว้
- Evidence or criterion: การจัดกลุ่มต้อง mutually exclusive และครอบคลุมทุกกรณี
- Why it matters: การจำแนกและการคำนวณ kappa คลุมเครือ
- Requested action: แยกเป็น 2 แกน คือความต่อเนื่อง 3 ระดับ × ระดับคาร์บอน 0–2 แล้วนิยาม FCE จากสองแกนนี้ และระบุว่าเกณฑ์ 0.5/1.0 mm และ 50% เป็นเกณฑ์ที่ผู้วิจัยกำหนดและจะทดสอบใน pilot

### Minor comment m5

- Location: 5.1, 5.2, 5.8, 5.12
- Observation: พบ 4 จุด
  - มีเครื่องหมายร่างตกค้าง ได้แก่ "(ประเด็นที่ 9)", "(ประเด็นที่ 1)", "(ข)", "(ก)"
  - มีข้อความจากฉบับหลายเครื่องตกค้าง ได้แก่ "[ถ้ามี]", ระยะโฟกัสสำหรับระบบ non-contact และ "ชนิดของเลเซอร์"
  - ใช้ "กำลังสูงสุด (output power)" ในความหมายของ peak power
  - ตารางที่ 1 ยังว่าง และรายการอ้างอิงไม่มีคู่มือ Lasotronix
- Evidence or criterion: ความสอดคล้องภายใน และการสืบย้อนข้อมูลผู้ผลิตกลับไปยังแหล่งได้
- Why it matters: ผู้อ่านสืบย้อนค่า preset กลับไปยังผู้ผลิตไม่ได้
- Requested action: ลบเครื่องหมายร่างที่ตกค้าง ใช้คำว่า "peak power" กรอกตารางที่ 1 จากคู่มือ และเพิ่มคู่มือในรายการอ้างอิง

### Minor comment m6

- Location: 5.3
- Observation: ยังยืนยันจากบันทึกที่มีไม่ได้ว่าตำแหน่ง "ส่วนหน้าต่อ frenulum" มาจาก ref 12 และยังไม่ได้ระบุอุณหภูมิขณะทดลองเป็นตัวเลข รวมถึงวิธีรักษาความชื้นระหว่างพักชิ้นเนื้อ
- Evidence or criterion: การรายงานรายละเอียดชิ้นเนื้อ
- Why it matters: ความแปรปรวนของชิ้นเนื้อมีผลต่อความลึก
- Requested action: ตรวจกับ ref 12 §2.2 ระบุอุณหภูมิ (ref 12 ใช้ 25 °C) และวิธีรักษาความชื้น

## วิธีการ สถิติ และ reproducibility

ช่องว่างด้านการรายงานที่ยังไม่ได้กล่าวถึงข้างต้น:
- ไม่มีแผน flow ของ ลิ้น → บล็อก → รอยตัด → หน้าตัด
- ไม่ระบุเวอร์ชัน SPSS และ ImageJ
- ไม่ระบุรุ่นของ power meter และใบรับรองการสอบเทียบ
- ไม่มีแผนเก็บรักษาและแชร์ภาพและข้อมูล
- วางแผนรายงาน 95% CI สำหรับสัดส่วนและ output แต่ไม่ได้วางแผนสำหรับความแตกต่างระหว่าง preset

แนะนำให้ปรึกษานักชีวสถิติเรื่อง design ข้อมูล binary แบบมี clustering ในระยะที่ 2

## จริยธรรม ความโปร่งใส ภาพ ตาราง และการอ้างอิง

- ยังไม่มีหัวข้อจริยธรรม การจัดการของเสียชีวภาพ laser controlled area แว่นป้องกัน และการดูดควัน ตามคำแนะนำ Methods ของอาจารย์ข้อ 16
- เครื่องมือเลือก reporting guideline เสนอได้เพียง SPIRIT-2025 เพราะระยะที่ 2 มีการสุ่ม แต่ SPIRIT ไม่ได้ออกแบบมาสำหรับงาน ex vivo บนชิ้นเนื้อ checklist สำหรับงาน in vitro ทางทันตกรรม (CRIS guidelines) อาจเหมาะกว่า แต่ต้องตรวจเวอร์ชันปัจจุบันก่อนนำมาใช้ [ต้องยืนยัน]

## ข้อจำกัดของรีวิวนี้

- รีวิวเฉพาะหัวข้อ 4–7
- ตรวจรายละเอียดแหล่งอ้างอิงเทียบกับ extraction notes ใน vault ไม่ได้เปิดต้นฉบับครบทุกฉบับ
- ค่าของ Puttapiban (ref 14) อ่านจากภาพสแกน และขอบ CI หนึ่งค่าอ่านไม่ออก
- ไม่ได้คำนวณซ้ำนอกจากตรวจเลขคณิตของสูตร (1) (σ = 300, E = 100 → n = 34.6 → 35)
- ไม่ได้ตรวจค่าบนเครื่องจริง

# Confidential comments to editor

(ความเห็นลับถึงบรรณาธิการ)

> โครงร่างที่รีวิวภายในไม่มีช่องทางความเห็นลับ รายการด้านล่างจึงเป็นประเด็นสำหรับอาจารย์ที่ปรึกษา

## การเปิดเผยของผู้รีวิว

- Conflicts and editor clearance: ไม่พบผลประโยชน์ทับซ้อน
- Competence limits or specialist review needed: design ข้อมูล binary แบบมี clustering ในระยะที่ 2 (ชีวสถิติ)
- Assistance or tools used and required disclosure: ร่างด้วย AI ช่วย โดยใช้เครื่องมือ peer-review ของ Scientific Agent Skills ที่รันบนเครื่อง (อ้างอิง [1])
- Confidentiality or retention issue: ไม่มี

## ประเด็นด้านกระบวนการหรือความถูกต้อง

ไม่พบ ประเด็นที่ต้องให้อาจารย์ตัดสินใจมีดังนี้:
- ex vivo หรือ in vitro (ชื่อเรื่องที่อาจารย์เสนอใช้ "in vitro")
- ระยะที่ 2 เป็นเชิงยืนยันหรือ descriptive pilot
- ความขัดกันระหว่างคำแนะนำแนว endpoint-guided (target depth 2.0 ± 0.3 mm) กับคำแนะนำ Methods ฉบับหลัง (ไม่มี target depth)
- เพดานทรัพยากรของจำนวนลิ้น

# เครื่องมือที่ใช้และเอกสารอ้างอิง

1. Kassis T, Agarwal V, He Y, Patel D, Brueckner AM. Scientific Agent Skills: a library of procedural knowledge for research agents [Preprint]. arXiv; 2026. arXiv:2609.00065. doi:10.48550/arXiv.2609.00065

> ตรวจกับ arXiv record เมื่อ 2026-10-10: ผู้แต่ง 5 คนตามลำดับข้างต้น เวอร์ชันปัจจุบัน v2 (2 ก.ย. 2026) ยังไม่มี journal reference หรือ publisher DOI จึงอ้างเป็น preprint โดยไม่ระบุเวอร์ชันตามคำแนะนำของ skill
