# บันทึกงานเปลี่ยนมิเตอร์ชำรุด – กฟส.คำชะอี

ฟอร์มมือถือ (GitHub Pages) → Google Apps Script → Google Sheet

## ติดตั้ง 3 ขั้นตอน
1. **Google Sheet**: สร้างชีตใหม่ > ส่วนขยาย > Apps Script > วางโค้ด `Code.gs` > Deploy > New deployment > Web app
   (Execute as: Me / Who has access: Anyone) > คัดลอก URL `.../exec` (ครั้งแรกกดอนุญาตสิทธิ์ Sheet+Drive)
2. แก้ `index.html` บรรทัด `API_URL` ใส่ URL ที่ได้
3. **GitHub**: สร้าง repo > อัปโหลดไฟล์ทั้งหมดในโฟลเดอร์นี้ > Settings > Pages > Deploy from branch `main` / root
   เปิดลิงก์ `https://<ชื่อ>.github.io/<repo>/` บน Chrome มือถือ > ⋮ > เพิ่มลงในหน้าจอหลัก

หมายเหตุ: ถ้าแก้ Code.gs ภายหลัง ต้อง Deploy > Manage deployments > New version
