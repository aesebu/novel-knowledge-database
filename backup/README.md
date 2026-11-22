# NOVEL_KNOWLEDGE_DATABASE — Backup Repository

ระบบฐานความรู้สำหรับการเขียนนิยายและงานวรรณกรรม

## โครงสร้าง

- `backup/` — ชุดสำรองข้อมูล ณ วันที่ 22 พ.ย. 2026
- แหล่งข้อมูลจริง: Google Sheets `NOVEL_KNOWLEDGE_DATABASE`
- ตารางข้อมูลหลัก 6 ตาราง + ทะเบียนสูตร 1 ตาราง

## ชุดสำรอง NKD-BK-20261122-001

| ไฟล์ | แถว | sha256 (20 ตัวแรก) |
|---|---|---|
| NKD_01_Knowledge_Records.csv | 100 | a0f1678201eea003b313 |
| NKD_01b_System_Novels_Ranked.csv | 100 | — |
| NKD_03_Story_Elements.csv | 100 | 4dc99fbffef779b89f37 |
| NKD_04_Genres_Markets.csv | 57 | ad7a22f02584f404e89e |
| NKD_05_Relationships.csv | 100 | 01181108b19bb00bc819 |

## เอกสารระบบ

- NKD-ARCH-001 — Phase 01–02 System & Database Architecture
- NKD-META-001 — Phase 03 Metadata Framework
- NKD-OPS-001 — Operations & Views Handbook
- NKD-AUDIT-001 — Phase 13 Final Audit

## ข้อจำกัดที่บันทึกไว้

- Google Drive connector ไม่รองรับการอัปโหลดไฟล์ไบนารี — ใช้ GitHub เป็นปลายทางสำรองแทน
- อักขระไทยบางคำจาก PDF ต้นฉบับเรียงสลับ ยังไม่ได้แก้
- ค่าสิทธิ์ใช้ `Not Recorded` แทน `Unknown`
- Phase 10 (Automation) ไม่พัฒนา ตามคำสั่งผู้ใช้
