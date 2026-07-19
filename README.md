# Git & Fork Setup Guide

คู่มือการเริ่มต้นใช้งาน Git และ Fork สำหรับผู้เริ่มต้น ตั้งแต่การติดตั้ง Git การตั้งค่า `user.name` และ `user.email` ไปจนถึงการติดตั้ง Fork และเชื่อมต่อกับ GitHub

---

## 📌 สิ่งที่ต้องเตรียม

- Windows 10 / 11
- บัญชี GitHub
- อินเทอร์เน็ต

---

# 1. ดาวน์โหลดและติดตั้ง Git

## ดาวน์โหลด

ดาวน์โหลด Git ได้จากเว็บไซต์ทางการ

👉 https://git-scm.com/download/win

## ขั้นตอนการติดตั้ง

1. เปิดไฟล์ติดตั้ง Git
2. กด **Next** ไปเรื่อย ๆ
3. ใช้ค่าตั้งต้น (Default) ทุกขั้นตอน
4. กด **Install**
5. กด **Finish**

---

## ตรวจสอบการติดตั้ง

เปิด **Git Bash** แล้วพิมพ์

```bash
git --version
```

ตัวอย่าง

```bash
git version 2.50.1.windows.1
```

หากขึ้นเวอร์ชัน แสดงว่าติดตั้งสำเร็จ

---

# 2. ตั้งค่า Git Configuration

Git จะใช้ข้อมูลนี้ทุกครั้งที่มีการ Commit

## ตั้งชื่อผู้ใช้

```bash
git config --global user.name "Your Name"
```

ตัวอย่าง

```bash
git config --global user.name "John Smith"
```

---

## ตั้งค่า Email

```bash
git config --global user.email "your@email.com"
```

ตัวอย่าง

```bash
git config --global user.email "john@gmail.com"
```

> แนะนำให้ใช้อีเมลเดียวกับที่สมัคร GitHub

---

## ตรวจสอบข้อมูล

ดูชื่อ

```bash
git config --global user.name
```

ดู Email

```bash
git config --global user.email
```

ดูทั้งหมด

```bash
git config --list
```

---

# 3. ดาวน์โหลดและติดตั้ง Fork

Fork เป็นโปรแกรม GUI สำหรับใช้งาน Git

## ดาวน์โหลด

👉 https://git-fork.com/

## ติดตั้ง

1. ดาวน์โหลดโปรแกรม
2. เปิดไฟล์ติดตั้ง
3. กด **Next**
4. กด **Install**
5. กด **Finish**

---

# 4. เชื่อมต่อ Fork กับ GitHub

เปิดโปรแกรม **Fork**

ไปที่

```
File
└── Accounts
```

เลือก

```
GitHub
```

จากนั้นกด

```
Sign in with Browser
```

ล็อกอิน GitHub

กด

```
Authorize Fork
```

เมื่อเสร็จแล้ว Fork จะสามารถใช้งานกับ GitHub ได้

---

# 5. Clone Repository

ภายใน Fork

```
File
└── Clone
```

หรือกด

```
Clone Repository
```

นำ URL Repository เช่น

```
https://github.com/username/project.git
```

เลือกตำแหน่งจัดเก็บ

กด

```
Clone
```

---

# 6. สร้าง Repository บน GitHub

1. เข้า https://github.com
2. กด **New Repository**
3. ตั้งชื่อ Repository
4. กด **Create Repository**

---

# 7. Workflow การใช้งาน Git

```
แก้ไขไฟล์
      │
      ▼
Stage
      │
      ▼
Commit
      │
      ▼
Push
      │
      ▼
GitHub
```

---

## Stage

เลือกไฟล์ที่ต้องการ

กด

```
Stage
```

---

## Commit

พิมพ์ข้อความ เช่น

```
Add login page
```

กด

```
Commit
```

---

## Push

กด

```
Push
```

เพื่ออัปโหลดงานขึ้น GitHub

---

## Pull

หากมีการอัปเดต Repository

กด

```
Pull
```

เพื่อดึงข้อมูลล่าสุด

---

# 8. คำสั่ง Git ที่ใช้บ่อย

| คำสั่ง | ความหมาย |
|---------|-----------|
| `git init` | สร้าง Git Repository |
| `git clone <URL>` | Clone Repository |
| `git status` | ตรวจสอบสถานะ |
| `git add .` | เพิ่มไฟล์ทั้งหมดเข้า Stage |
| `git commit -m "message"` | Commit |
| `git push` | ส่งขึ้น GitHub |
| `git pull` | ดึงข้อมูลล่าสุด |
| `git log` | ดูประวัติ Commit |

---

# 9. ตัวอย่างการเริ่มต้นใช้งาน

ตรวจสอบเวอร์ชัน

```bash
git --version
```

ตั้งชื่อ

```bash
git config --global user.name "John Smith"
```

ตั้งอีเมล

```bash
git config --global user.email "john@gmail.com"
```

ตรวจสอบข้อมูล

```bash
git config --list
```

---

# 🎯 สรุปขั้นตอน

- ✅ ติดตั้ง Git
- ✅ ตั้งค่า `user.name`
- ✅ ตั้งค่า `user.email`
- ✅ ติดตั้ง Fork
- ✅ เชื่อมต่อ GitHub
- ✅ Clone Repository
- ✅ Stage
- ✅ Commit
- ✅ Push
..................
---

# 📚 อ้างอิง

- Git Official: https://git-scm.com/
- GitHub Docs: https://docs.github.com/
- Fork Official: https://git-fork.com/