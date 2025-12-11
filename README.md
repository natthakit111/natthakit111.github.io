# 🏋️‍♂️ FitnessPal – ENGCE301 Term Project  

เว็บแอปพลิเคชันสำหรับติดตามสุขภาพ บันทึกโภชนาการ การออกกำลังกาย และสรุปผลแบบกราฟ ตามเอกสาร **Software Requirements Specification (SRS)**  
โปรเจกต์นี้ถูกพัฒนาภายใต้วิชา **ENGCE301: Software Design and Development**  
โดยกลุ่ม **NightFall**

---

## 📌 Project Overview  
**FitnessPal** เป็นระบบที่ช่วยให้ผู้ใช้สามารถติดตามสุขภาพของตนเองได้อย่างครบถ้วน  
รองรับการบันทึกข้อมูลรายวัน พร้อมระบบวิเคราะห์อย่างง่าย เช่น:

- บันทึกมื้ออาหาร (Calories Intake)
- บันทึกการออกกำลังกาย (Calories Burn)
- คำนวณ BMR / TDEE
- แสดงผลรายวัน รายสัปดาห์ และกราฟแนวโน้ม

ระบบถูกออกแบบและอ้างอิงตาม SRS ที่พัฒนาขึ้นในรายวิชาดังกล่าว

---

## 🎯 Objectives  

- สร้าง Prototype ของระบบติดตามสุขภาพที่ใช้งานง่าย  
- ออกแบบระบบตามกระบวนการ Software Engineering  
- รองรับการขยายระบบในอนาคต เช่น Recommendation หรือ Trainer Analysis  
- พัฒนาส่วนติดต่อผู้ใช้ (UI) แบบ Responsive รองรับมือถือเต็มรูปแบบ  

---

## 👥 Team Members (NightFall)
| Name | Student ID | Role | GitHub |
|------|-----------|------|--------|
| นายจักรกฤษณ์ จาปัญญะ | 66543206040-8 | Team Leader / Tester / Frontend | [@BakaZeno](https://github.com/BakaZeno) |
| นายเมย์คาร์ สุวรรณวิสุทธิ | 66543206085-3 | Frontend | [@Mekha1104](https://github.com/Mekha1104) |
| นายปรเมษฐ สุริคำ | 66543206038-2 | Frontend / System Analysis | [@porameter](https://github.com/porameter) |
| นายณัฐกิตติ์ ยั่งยืนปิยรัตน์ | 66543206014-3 | Backend | [@natthakit111](https://github.com/natthakit111) |
| นายจิรวัฒน์ มาลัยวรรณ | 66543206070-5 | Backend | [@Jirawat66](https://github.com/Jirawat66) |


## ✨ Key Features (ตาม SRS)

### 1️⃣ จัดการบัญชีผู้ใช้  
- สมัครสมาชิก / เข้าสู่ระบบ  
- แก้ไขโปรไฟล์  
- เก็บข้อมูลพื้นฐาน: อายุ เพศ น้ำหนัก ส่วนสูง ระดับกิจกรรม

### 2️⃣ ตั้งเป้าหมายสุขภาพ  
- เลือกประเภทเป้าหมาย  
- กำหนดน้ำหนักเป้าหมายและช่วงเวลา  

### 3️⃣ บันทึกมื้ออาหาร  
- บันทึกอาหาร, ปริมาณ, หน่วย  
- คำนวณแคลอรี่ (Energy In)

### 4️⃣ บันทึกการออกกำลังกาย  
- บันทึกกิจกรรม, ความหนัก, ระยะเวลา  
- คำนวณแคลอรี่ที่เผาผลาญ (Energy Out)

### 5️⃣ สรุปผล & กราฟความคืบหน้า  
- สรุปพลังงานเข้า–ออก  
- รายงานรายสัปดาห์ (FR-009)  
- กราฟความคืบหน้า เช่น น้ำหนัก แคลอรี่ (FR-010)

### 6️⃣ Trainer & Admin Tools  
- เทรนเนอร์สร้างโปรแกรมฝึก (FR-011)  
- ติดตามผู้ใช้งาน (FR-012)  
- ผู้ดูแลระบบจัดการข้อมูลผู้ใช้ (FR-013)

---

## 📑 Functional Requirements (FR)

| รหัส FR | รายละเอียด |
|---------|------------|
| **FR-001 – FR-003** | จัดการบัญชีผู้ใช้ |
| **FR-004** | ตั้งเป้าหมายสุขภาพ |
| **FR-005** | บันทึกมื้ออาหาร |
| **FR-006** | บันทึกกิจกรรมการออกกำลังกาย |
| **FR-007 – FR-008** | สรุปผลรายวัน |
| **FR-009** | รายงานรายสัปดาห์ |
| **FR-010** | กราฟความคืบหน้า |
| **FR-011** | เทรนเนอร์สร้างโปรแกรมฝึก |
| **FR-012** | ติดตามผู้ใช้งาน |
| **FR-013** | ผู้ดูแลระบบจัดการผู้ใช้ |

รวมทั้งหมด **13 ฟังก์ชันตาม SRS**

---

## 🧱 Tech Stack  

### 🌐 Frontend  
- HTML5  
- CSS3 (Responsive Layout)  
- JavaScript ES6  
- Google Fonts: Inter  

### 🖥 Backend (ตาม SRS)  
- Node.js + Express.js  
- JWT Authentication  

### 🗄 Database (ตาม SRS)  
- SQLite / MongoDB  

---

## 📂 Project Structure

📁 ENGCE301_LAB2.GITHUB.IO/  
├── 📄 index.html                # Landing Page  
├── 📁 css/  
│   └── 📄 style.css  
├── 📁 assets/  
│   ├── 📁 images/  
│   └── 📁 icons/  
├── 📄 SRS_Draft.md              # Requirements Specification  
├── 📄 README.md  
└── 📄 .gitignore


## 📖 Documentation
- [Software Requirements Specification (SRS)](./SRS_Draft.md)
- [User Interview Notes](./docs/interview_notes.md)

## 🌐 Demo
- **Live Demo:** [https://bakazeno.github.io/nightfall-lab2.github.io](https://bakazeno.github.io/nightfall-lab2.github.io)
- **GitHub Pages:** [https://github.com/BakaZeno/nightfall-lab2.github.io](https://github.com/BakaZeno/nightfall-lab2.github.io)

## 🏃‍♂️ How to Run Locally
```bash
# 1. Clone repository
git clone https://github.com/BakaZeno/nightfall-lab2.github.io.git

# 2. Navigate to project folder
cd project-name

# 3. Open with Live Server (VSCode Extension)
# Or simply open index.html in browser