[README.md](https://github.com/user-attachments/files/26131850/README.md)
# 🛡️ Insurance Dashboard

แดชบอร์ดจัดการกรมธรรม์ประกันภัยส่วนตัว เชื่อมต่อกับ Google Sheets เพื่อเก็บข้อมูลแบบ real-time ใช้งานได้จากทุกเครื่องผ่าน Browser

---

## ✨ ฟีเจอร์หลัก

- 📋 จัดการกรมธรรม์ประกันภัยทุกประเภท — ชีวิต, สุขภาพ, รถยนต์, บ้าน, เดินทาง
- 📊 สรุปภาพรวม — เบี้ยประกันรายปี, ทุนประกันรวม, กรมธรรม์ใกล้หมดอายุ
- 🔔 แจ้งเตือนการชำระเบี้ยที่กำลังจะมาถึง
- ✏️ เพิ่ม / แก้ไข / ลบ กรมธรรม์ได้ทันที
- ☁️ ข้อมูลซิงค์กับ Google Sheets — เปิดจากเครื่องไหนก็เห็นข้อมูลเดียวกัน

---

## 🚀 วิธีติดตั้ง

### ขั้นตอนที่ 1 — ตั้งค่า Google Apps Script

1. ไปที่ [Google Sheets](https://sheets.google.com) → สร้าง Spreadsheet ใหม่
2. เปิด **Extensions → Apps Script**
3. วางโค้ดจากไฟล์ `Code.gs` ทับโค้ดเดิมทั้งหมด
4. กด **Deploy → New deployment → Web app**
5. ตั้งค่า:
   - Execute as: **Me**
   - Who has access: **Only myself** (แนะนำ — ปลอดภัยสุด)
6. คัดลอก **Web app URL** ที่ได้มา

### ขั้นตอนที่ 2 — เปิดใช้งาน Dashboard

1. เปิด [https://GOSU-Hub.github.io/insurance-dashboard](https://GOSU-Hub.github.io/insurance-dashboard)
2. วาง Web app URL ในช่องที่แสดงด้านบน
3. กด **"บันทึก URL"** → พร้อมใช้งาน!

---

## 🗂️ โครงสร้างไฟล์

```
insurance-dashboard/
├── index.html      # แดชบอร์ดหลัก
├── Code.gs         # Google Apps Script backend
└── README.md       # ไฟล์นี้
```

---

## 🔒 ความปลอดภัย

- ข้อมูลกรมธรรม์ทั้งหมดเก็บใน **Google Sheets ของคุณเอง** ไม่มีเซิร์ฟเวอร์กลาง
- ตั้งค่า Apps Script เป็น **Only myself** เพื่อให้เฉพาะบัญชี Google ของคุณเข้าถึงได้
- โค้ดใน repository นี้เป็นแค่ UI ไม่มีข้อมูลส่วนตัวใดๆ

---

## 🛠️ เทคโนโลยีที่ใช้

- **Frontend** — HTML, CSS, Vanilla JavaScript (ไม่มี dependency)
- **Backend** — Google Apps Script
- **Database** — Google Sheets
- **Hosting** — GitHub Pages
