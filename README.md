#Part 1: Git Fundamentals & Local Development - [งานเดี่ยว] (40 คะแนน)
วัตถุประสงค์
เรียนรู้การใช้งาน Git commands พื้นฐาน
สามารถเชื่อมต่อ Local Repository กับ GitHub
ฝึกการทำงานกับ branching และ merging
เตรียมตัวก่อนเริ่มทำแลป
ติดตั้ง Git บนเครื่องคอมพิวเตอร์
สร้างบัญชี GitHub
ตั้งค่า Git configuration

# ตั้งค่าชื่อและอีเมล
git config --global user.name "thanakon"

git config --global user.email "thanakon.170147@gmail.com"

# ตรวจสอบการตั้งค่า
git config --list

<img width="483" height="63" alt="image" src="https://github.com/user-attachments/assets/31dc2792-7fe6-4002-bdf3-a6d40ec2d838" />

ขั้นตอนที่ 1: สร้าง Repository และเชื่อมต่อกับ GitHub
1.1 สร้างโฟลเดอร์โปรเจกต์
# สร้างโฟลเดอร์โปรเจกต์
mkdir my-portfolio
cd my-portfolio

# เริ่มต้น Git repository
git init

<img width="998" height="337" alt="image" src="https://github.com/user-attachments/assets/78b29ce7-8c7c-4a07-b5e0-e3737dda2297" />

1.2 สร้างไฟล์พื้นฐาน
สร้างไฟล์ index.html:

<img width="1294" height="856" alt="image" src="https://github.com/user-attachments/assets/28e69634-47c6-4819-a12c-7f9525011848" />

สร้างไฟล์ style.css:

<img width="888" height="1260" alt="Screenshot 2568-07-16 at 13 48 07" src="https://github.com/user-attachments/assets/0d4250de-ba1a-4074-95bc-f57affd37730" />

1.3 เพิ่มไฟล์ไปยัง Repository
# ตรวจสอบสถานะไฟล์
git status

# เพิ่มไฟล์ทั้งหมดไปยัง staging area
git add .

# ตรวจสอบสถานะอีกครั้ง
git status

# Commit ครั้งแรก
git commit -m "Initial commit: Add basic portfolio structure"

<img width="1005" height="913" alt="image" src="https://github.com/user-attachments/assets/caa101c5-bad0-470f-b735-3f90d7d55fe4" />

1.4 สร้าง Repository บน GitHub และเชื่อมต่อ
ไปที่ GitHub.com และล็อกอิน
คลิก "New Repository"
ตั้งชื่อ repository เป็น "my-portfolio"
ไม่ต้องเลือก "Initialize with README"
คลิก "Create Repository"

<img width="1618" height="755" alt="Screenshot 2568-07-16 at 13 36 18" src="https://github.com/user-attachments/assets/2f83952b-1d30-48e7-9450-53350f9407dd" />

git remote add origin git@github.com:[your-username]/my-portfolio.git

# ตรวจสอบการเชื่อมต่อ
git remote -v

# Push ไฟล์ไปยัง GitHub
git push -u origin main

<img width="819" height="364" alt="Screenshot 2568-07-16 at 13 53 04" src="https://github.com/user-attachments/assets/02f272d6-e77b-419a-b434-2944af640ee2" />

ขั้นตอนที่ 2: การทำงานกับ Branches
2.1 สร้าง Branch ใหม่สำหรับเพิ่มฟีเจอร์

# สร้าง branch ใหม่และเปลี่ยนไป
git checkout -b feature/add-projects

# ตรวจสอบ branch ปัจจุบัน
git branch






