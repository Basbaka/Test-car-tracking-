# Real-time Vehicle Tracking Simulation

ระบบจำลองการติดตามยานพาหนะแบบเรียลไทม์ (Real-time GPS Tracking Simulation) วิ่งบนเส้นทางถนนจริงจาก ศรีราชา ถึง กรุงเทพฯ (อโศก) ผ่านถนนสุขุมวิท ด้วยความเร็วคงที่ 100 กิโลเมตรต่อชั่วโมง

## คุณสมบัติเด่น (Features)
- **Real-time Map Rendering**: แสดงผลแผนที่ลื่นไหลด้วย Leaflet.js
- **OSRM Routing Integration**: ดึงข้อมูลโครงสร้างถนนจริงผ่าน OSRM API เพื่อให้รถวิ่งตรงตามแนวถนนและทางโค้ง
- **Custom SVG Vehicle Icon**: ไอคอนรถยนต์ดีไซน์โมเดิร์นที่หมุนองศาหน้ารถ (Heading) ตามทิศทางการเคลื่อนที่จริง
- **Auto-Pan Camera**: กล้องแผนที่แพนตามตำแหน่งรถยนต์อัตโนมัติ
- **Data Logging & Export**: บันทึกพิกัด (Latitude, Longitude), ความเร็ว, และองศารถ ทุกๆ 1 วินาที พร้อมปุ่มดาวน์โหลดออกเป็นไฟล์ `.txt` (CSV Format)

## เทคโนโลยีที่ใช้ (Tech Stack)
- HTML5 / CSS3 / Vanilla JavaScript
- [Leaflet.js](https://leafletjs.com/) (Map Library)
- [OSRM API](http://project-osrm.org/) (Routing Machine)
- CARTO Voyager (Map Tiles)

## วิธีการใช้งาน (How to Use)
1. เปิดไฟล์ `index.html` ผ่านเว็บบราวเซอร์
2. ระบบจะทำการโหลดเส้นทางและเริ่มการจำลองการขับขี่ทันที
3. สังเกตตัวเลขจำนวนข้อมูล Log ที่เพิ่มขึ้นทางกล่องเมนูด้านซ้าย
4. เมื่อต้องการข้อมูล สามารถกดปุ่ม **"ดาวน์โหลดไฟล์ .txt"** เพื่อนำพิกัดไปใช้งานต่อได้