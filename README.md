# DADS5001_Mini-Project
- Average price per living &amp; eating score for each upcountry of Thailand
- Average price of property type ( บ้านเดี่ยว, บ้านแฝด, ทาวน์โฮม, คอนโด ) from 2020 to 2022

# Authur
- Kanisorn Hongthong
- ID: 6420422024
- Subject: DADS5001

# Dataset Information

- Residental Project Data source: https://gobestimate.com/data-detail/Residental-Project-Data
- Living Score By Location source: https://gobestimate.com/data-detail/Living-Score-By-Location
- Eating Score By Location source: https://gobestimate.com/data-detail/Eating-Score-By-Location

Total: 
  - Residental Project Data : 23,604 Rows
  - Living Score By Location : 708 Rows
  - Eating Score By Location : 554 Rows
  
 Column:
 
   Residental Project Data source:
   
   - row_number
   - propertytype_name_en
   - price_min
   - subdistrict_name_th
   - district_name_th
   - province_name_th
   - date_updated
  
   Living Score By Location source:
   
   - subdistrict_name_th
   - district_name_th
   - province_name_th
   - walk_total
   - access_total
   - drive_total
   
   Eating Score By Location source:
   
   - subdistrict_name_th
   - district_name_th
   - province_name_th
   - eating_daytime
   - eating_nighttime
  
 # Analysis Question
 1. อ้างอิงจาก Living score และ Eating score ของแต่ละเขต พื้นที่ใดมีราคาเฉลี่ยต่อ 1 คะแนนดีที่สุด
    - Ans: จาก Data ที่มีได้ว่า หากเป็นพื้นที่ปริมณฆล พื้นที่จังหวัด Nakornpatom เป็นพื้นที่ที่คุ้มที่สุด มีราคาเฉลี่ยต่อ 1 คะแนน Living score กับ Eating score ถ้าหากเป็นพื้นที่ต่างจังหวัด จังหวัดระยองจะเป็นพื้นที่มีราคาเฉลี่ยคุ้มค่าที่สุด
 2. หากต้องการเลือกซ์้ออสังหาริมทรัพย์ (บ้านเดี่ยว, บ้านแฝด, ทาวน์โฮม, คอนโด) จะสามารถนำข้อมูลราคามีช่วยในการตัดสินใจได้หรือไม่
    - Ans: อ้างอิงจากราคาเฉลี่ยของอสังหาริมทรัพย์ (บ้านเดี่ยว, บ้านแฝด, ทาวน์โฮม, คอนโด) จากราคา update ในแต่ละปี จะพบว่า บ้านเดี่ยว เป็นอสังหาริมทรัพย์ที่ราคาเฉลี่ยในแต่ละปีไม่ลดลงในทุกๆปี
    
 # Issue
 1. ชื่อ Subdistrict และ district 1 ชื่อจะซ้ำกันในหลายๆจังหวัด ทำให้ต้องสร้าง Key ที่ใช้ Mapping ขึ้นมาใหม่โดยใช้ (Subdistrict + District + Province)
 2. เนื่องจากข้อจำกัดทางด้านเวลา ทำให้ความเข้าใจใน dataset อสังหาริมทรัพย์มีไม่มากพอ ทำให้ insight ที่หามาได้ อาจจะไม่สมบูรณ์ และไม่สามารถตอบคำถามที่ตั้งได้อย่าง 100%
 
  # Graph
  
  
  ![image](https://user-images.githubusercontent.com/115795313/195882543-d6060bdf-397e-40d8-919b-b253659440a7.png)


  ![image](https://user-images.githubusercontent.com/115795313/195882708-9833ee28-db08-457b-a451-0ac6882e9e6d.png)

 
 
  
