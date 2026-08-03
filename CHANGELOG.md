# Changelog: Laundromat Notification System
โปรเจกต์: ระบบแจ้งเตือนเครื่องซักผ้าร้าน


## [v1.0.0] - 2026-08-02
### Added
- LO1: โครงสร้างข้อมูลคงที่ `VALID_STATUSES` (frozenset) และ `ADMIN_ACCOUNT` (tuple)
- LO1: โครงสร้างสถานะเครื่องซักผ้าหลัก `machines` (dict)
- LO2: ฟังก์ชัน `get_available_machines` สกัดข้อมูลเครื่องว่างด้วย Set Comprehension
- LO3: ระบบเมนูโต้ตอบหลัก (while loop) และระบบ Login ผู้ดูแลร้าน (ลิมิต 3 ครั้ง)
- LO4: ระบบ Defensive Check ป้องกัน KeyError และ try-except ดักจับ ValueError

## [v0.4.0] - 2026-07-XX
### Added
- ตรวจสอบความถูกต้องของหมายเลขเครื่องก่อนเข้าถึงข้อมูล (`machine_id in machines_dict`)
### Fixed
- ป้องกัน IndexError/KeyError เมื่อผู้ใช้กรอกหมายเลขเครื่องนอกช่วง 1-10

---

> 📝 หมายเหตุ: v1.0.0 คือเวอร์ชันตอนส่ง mini project (ครบทั้ง 7 ฟีเจอร์หลัก: Config, Data Model, Check Available, My Machine Tracking, Admin Auth, Status Update, Interactive CLI) ตามรายละเอียดใน `mini_project_kanban.pdf`
