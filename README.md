# NOVEL_KNOWLEDGE_DATABASE

ระบบฐานความรู้สำหรับการเขียนนิยายและงานวรรณกรรม

## ที่มาของ repo นี้

repo นี้สร้างขึ้นเป็นที่เก็บสำรองข้อมูล แทน Google Drive เนื่องจาก connector ของ Google Drive ไม่รองรับการอัปโหลดไฟล์ไบนารีหรือไฟล์ขนาดใหญ่ (สร้างได้เฉพาะไฟล์จากข้อความสั้น)

## โครงสร้าง

```
backup/
  ├── NKD-BK-20261122-001_MANIFEST.txt
  ├── NKD-BK-20261122-001_LOG.txt
  └── IMPORT_STATUS.md
```

## ฐานข้อมูลจริง

- Google Sheets: NOVEL_KNOWLEDGE_DATABASE — Master (7 แท็บ)
- โฟลเดอร์ Drive: NOVEL_KNOWLEDGE_DATABASE/ (14 โฟลเดอร์)
- หน้าโครงการ Notion: NOVEL_KNOWLEDGE_DATABASE

## จำนวนข้อมูล

| ตาราง | ในชีต | ในไฟล์ CSV |
|---|---|---|
| 01 Knowledge Records | 55 | 100 |
| 01b System Novels | 0 | 100 |
| 02 Sources | 8 | — |
| 03 Story Elements | 1 | 100 |
| 04 Genres & Markets | 57 | 57 |
| 05 Relationships | 100 | 100 |
| 06 Pipeline Log | 20 | — |
| 07 Lookup Index | 7 | — |

## เอกสารระบบ (แนบในแชท)

- NKD-ARCH-001 — Phase 01–02 System & Database Architecture
- NKD-META-001 — Phase 03 Metadata Framework
- NKD-OPS-001 — Operations & Views Handbook
- NKD-AUDIT-001 — Phase 13 Final Audit

## ข้อจำกัดที่บันทึกไว้

- Google Drive connector ไม่รองรับการอัปโหลดไฟล์ — ใช้ GitHub เป็นปลายทางสำรอง
- อักขระไทยบางคำจาก PDF ต้นฉบับเรียงสลับ (สระ/วรรณยุกต์) ยังไม่ได้แก้
- ค่าสิทธิ์ใช้ Not Recorded แทน Unknown
- Phase 10 (Automation) ไม่พัฒนา ตามคำสั่งผู้ใช้
- ความสัมพันธ์ในตาราง 05 ชี้ไปยัง NKD-STY/NKD-EL ที่ยังไม่ได้นำเข้า
