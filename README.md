# SYNC Platform  
## อนุชนสภาคริสตจักรในประเทศไทย  
Youth Council of the Church of Christ in Thailand

SYNC Platform คือเว็บไซต์และโครงสร้างดิจิทัลกลางของ  
**อนุชนสภาคริสตจักรในประเทศไทย**  
ออกแบบเพื่อใช้เป็นศูนย์กลางการสื่อสาร การพัฒนา และการเชื่อมโยงอนุชนทั่วประเทศ

โครงการนี้ถูกพัฒนาในรูปแบบ **Static Website + Web Components**  
เพื่อให้มีความเรียบง่าย ยั่งยืน และสามารถส่งต่อการดูแลได้ในระยะยาว

---

## 🎯 เป้าหมายของโครงการ (Project Objectives)

1. เป็นเว็บไซต์กลางอย่างเป็นทางการของอนุชนสภาคริสตจักรในประเทศไทย
2. ใช้เป็นแม่แบบ (Standard Template) สำหรับ:
   - เว็บอนุชนภาค
   - เว็บโครงการ / ค่าย / กิจกรรมระดับประเทศ
3. สนับสนุนการทำงานร่วมกันของ:
   - คณะกรรมการอนุชน
   - ทีมสื่อ
   - อนุชนรุ่นใหม่
4. รองรับการต่อยอดในอนาคต เช่น:
   - ระบบข่าว / ปฏิทิน
   - แบบฟอร์มออนไลน์
   - CMS
   - AI / Dashboard

---

## 🧱 หลักการออกแบบ (Design Principles)

- **HTML-first**: ทุกคนอ่านและแก้ไขได้
- **Component-based**: แยกส่วนชัดเจน ดูแลง่าย
- **Framework-free**: ไม่ผูกกับ React / Vue / Framework ใด
- **Long-term**: ใช้งานได้หลายปี ไม่ต้องรื้อระบบบ่อย
- **Mobile-first**: เหมาะกับอนุชนยุคปัจจุบัน

---

## 🔧 Technology Stack

- HTML5
- Tailwind CSS (CDN)
- Vanilla JavaScript
- Web Components (Custom Elements)
- GitHub Pages (Production Hosting)

> หมายเหตุ:  
> โครงการนี้ **ตั้งใจไม่ใช้ framework หนัก**  
> เพื่อให้บุคลากรหลากหลายช่วงวัยสามารถดูแลร่วมกันได้

---

## 📁 โครงสร้างโปรเจกต์ (Project Structure)
syncwebsite/
├─ index.html
│
├─ components/
│  ├─ layout/
│  │  ├─ app-header.js
│  │  ├─ app-footer.js
│  │  └─ app-container.js
│  │
│  ├─ sections/
│  │  ├─ hero-section.js
│  │  ├─ vision-section.js
│  │  ├─ mission-section.js
│  │  ├─ strategy-section.js
│  │  ├─ project-section.js
│  │  ├─ region-section.js
│  │  ├─ team-section.js
│  │  └─ contact-section.js
│  │
│  └─ ui/
│     ├─ ui-card.js
│     ├─ ui-section-title.js
│     ├─ ui-button.js
│     ├─ ui-badge.js
│     └─ ui-grid.js
│
└─ assets/
   ├─ images/
   ├─ icons/
   └─ documents/

---

## 🧩 Component Architecture

โครงสร้าง Component แบ่งเป็น 3 ระดับ

### 1) Layout Components
ใช้ควบคุมโครงเว็บหลัก  
แก้ไขโดยทีมแกนกลางเท่านั้น

- `<app-header>`
- `<app-footer>`
- `<app-container>`

---

### 2) Section Components
แทนแต่ละส่วนของหน้าเว็บ  
แต่ละ section ดูแลแยกกันได้

- `<hero-section>`
- `<vision-section>`
- `<mission-section>`
- `<strategy-section>`
- `<project-section>`
- `<region-section>`
- `<team-section>`
- `<contact-section>`

---

### 3) UI Components
ใช้ซ้ำได้ทั้งเว็บไซต์  
เป็นมาตรฐานร่วมของทุกโครงการ

- `<ui-card>`
- `<ui-section-title>`
- `<ui-button>`
- `<ui-badge>`
- `<ui-grid>`

---

## ✏️ แนวทางการแก้ไข (Editing Guidelines)

### แก้เนื้อหา
- แก้เฉพาะไฟล์ใน `components/sections/`
- ห้ามเขียน HTML ตรงใน `index.html`

### แก้โครงเว็บ
- แก้ใน `components/layout/`
- ต้องผ่านการตกลงของทีมแกนกลาง

### เพิ่ม UI ใหม่
- ต้องอยู่ใน `components/ui/`
- ออกแบบให้ reusable เสมอ

---

## 🚀 Deployment (GitHub Pages)

1. Push โค้ดขึ้น GitHub repository
2. ไปที่ **Settings → Pages**
3. ตั้งค่า:
   - Branch: `main`
   - Folder: `/root`
4. Save

เว็บไซต์จะออนไลน์ที่: www.cctyouth-thailand.org

---

## 🧭 แนวทางการขยายในอนาคต (Roadmap)

ระยะที่ 1 (ปัจจุบัน)
- เว็บไซต์กลาง
- Component Standard
- ใช้งาน Static เต็มรูปแบบ

ระยะที่ 2
- ข่าว / ปฏิทินกิจกรรม
- แบบฟอร์มสมัคร / ติดต่อ
- Content จาก Google Sheet / JSON

ระยะที่ 3
- CMS
- Dashboard
- AI Assistant สำหรับอนุชน

---

## 👥 การกำกับดูแลโครงการ (Governance)

โครงการนี้อยู่ภายใต้การดูแลของ:
- อนุชนสภาคริสตจักรในประเทศไทย
- คณะกรรมการที่ได้รับมอบหมาย

การเปลี่ยนแปลงโครงสร้างหลัก  
ควรผ่านการพิจารณาในระดับคณะกรรมการ

---

## 📌 หมายเหตุสำคัญ

- โปรเจกต์นี้ออกแบบเพื่อใช้งานระยะยาว
- หลีกเลี่ยงการแก้โครงสร้างโดยไม่จำเป็น
- ควรใช้เป็นแม่แบบเดียวกันทั่วประเทศ

---

## 📄 License / Usage

โครงการนี้จัดทำเพื่อการรับใช้และพันธกิจ  
สามารถนำไปปรับใช้ภายในคริสตจักรและองค์กรในเครือ  
โดยคงไว้ซึ่งเจตนารมณ์และโครงสร้างมาตรฐาน

---

© 2026  
อนุชนสภาคริสตจักรในประเทศไทย  
Youth Council of the Church of Christ in Thailand
