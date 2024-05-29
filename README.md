# Queue-Management-and-Store-Management-System
# ระบบจัดการคิวและบริหารร้านค้า
โครงงานระบบจัดการคิวและบริหารร้านค้าเป็นโครงงานสำหรับร้านค้า เพิ่มประสิทธิภาพให้กับร้านค้าและความพึงพอใจให้กับลูกค้า โดยที่ลดภาระงานให้กับพนักงาน ภายในระบบจะประกอบด้วยทั้งหมด 4 ส่วน
1. พนักงานเรียกคิว : สามารถเปิดคิว ยืนยันคิว และระบุโต๊ะให้แก่ลูกค้าตามหมายเลขคิว
2. ลูกค้า : สามารถทำการสแกนคิวอาร์โค้ดเพื่อทำการเปิดหน้าการสั่งซื้อรายการอาหาร สามารถทำการตรวจสอบรายการอาหารที่สั่งซื้อทั้งหมดพร้อมทราบยอดที่ต้องชำระ
3. แม่ครัว : สามารถทราบการอาหารที่ลูกค้าสั่ง และบันทึกสถานะการปรุงอาหาร
4. พนักงานเก็บเงิน : สามารถตรวจสอบยอดราคาสินค้าที่ลูกค้าสั่งซื้อ และเรียกเก็บเงินให้กับลูกค้า
# สารบัญ
 - [วิธีการติดตั้งระบบจัดการคิวและบริหารร้านค้า](#%E0%B8%A7%E0%B8%B4%E0%B8%98%E0%B8%B5%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%95%E0%B8%B4%E0%B8%94%E0%B8%95%E0%B8%B1%E0%B9%89%E0%B8%87%E0%B8%A3%E0%B8%B0%E0%B8%9A%E0%B8%9A%E0%B8%88%E0%B8%B1%E0%B8%94%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%84%E0%B8%B4%E0%B8%A7%E0%B9%81%E0%B8%A5%E0%B8%B0%E0%B8%9A%E0%B8%A3%E0%B8%B4%E0%B8%AB%E0%B8%B2%E0%B8%A3%E0%B8%A3%E0%B9%89%E0%B8%B2%E0%B8%99%E0%B8%84%E0%B9%89%E0%B8%B2)
 - [วิธีการใช้งานระบบจัดการคิวและบริหารร้านค้า](#%E0%B8%A7%E0%B8%B4%E0%B8%98%E0%B8%B5%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B9%83%E0%B8%8A%E0%B9%89%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B8%A3%E0%B8%B0%E0%B8%9A%E0%B8%9A%E0%B8%88%E0%B8%B1%E0%B8%94%E0%B8%81%E0%B8%B2%E0%B8%A3%E0%B8%84%E0%B8%B4%E0%B8%A7%E0%B9%81%E0%B8%A5%E0%B8%B0%E0%B8%9A%E0%B8%A3%E0%B8%B4%E0%B8%AB%E0%B8%B2%E0%B8%A3%E0%B8%A3%E0%B9%89%E0%B8%B2%E0%B8%99%E0%B8%84%E0%B9%89%E0%B8%B2)
	 - [พนักงานเรียกคิว](#%E0%B8%9E%E0%B8%99%E0%B8%B1%E0%B8%81%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B9%80%E0%B8%A3%E0%B8%B5%E0%B8%A2%E0%B8%81%E0%B8%84%E0%B8%B4%E0%B8%A7)
	 - [ลูกค้า](#%E0%B8%A5%E0%B8%B9%E0%B8%81%E0%B8%84%E0%B9%89%E0%B8%B2)
	 - [แม่ครัว](#%E0%B9%81%E0%B8%A1%E0%B9%88%E0%B8%84%E0%B8%A3%E0%B8%B1%E0%B8%A7)
	 - [พนักงานเก็บเงิน](#%E0%B8%9E%E0%B8%99%E0%B8%B1%E0%B8%81%E0%B8%87%E0%B8%B2%E0%B8%99%E0%B9%80%E0%B8%81%E0%B9%87%E0%B8%9A%E0%B9%80%E0%B8%87%E0%B8%B4%E0%B8%99)
# วิธีการติดตั้งระบบจัดการคิวและบริหารร้านค้า
1. ทำการลงทะเบียนเปิดใช้ Oracle Apex 
2. ทำการเลือก App Builder
3. ทำการ import ไฟล์ทั้ง 5 ไฟล์ เข้าไปใน Oracle Apex 
3.1 ไฟล์ที่ 1 คือ create_table_script คือไฟล์ระบบจัดการคิวและบริหารร้านค้าเป็นไฟล์สำหรับผู้ประกอบการและฐานข้อมูล
3.2 ไฟล์ที่ 2 คือ พนักงานเรียกคิว คือไฟล์สำหรับระบบของพนักงานเรียกคิว
3.3 ไฟล์ที่ 3 คือ ลูกค้า คือไฟล์สำหรับระบบของลูกค้า
3.4 ไฟล์ที่ 4 คือ แม่ครัว คือไฟล์สำหรับระบบของแม่ครัว
3.5 ไฟล์ที่ 5 คือ พนักงานเก็บเงิน คือไฟล์สำหรับระบบของพนักงานเก็บเงิน

# วิธีการใช้งานระบบจัดการคิวและบริหารร้านค้า
## พนักงานเรียกคิว
1. พนักงานเรียกคิวทำการกดปุ่มขอคิวให้กับลูกค้า พร้อมมอบตั๋วหมายเลขคิวให้กับลูกค้า
2. เมื่อถึงคิวของลูกค้า พนักงานเรียกคิวทำการกดปุ่มเรียกโต๊ะให้กับลูกค้า พร้อมทำการกำหนดโต๊ะให้กับลูกค้า
*(กรณีลูกค้าขอยกเลิกคิวสามารถกดยกเลิกคิวปัจจุบันเพื่อเรียกคิวถัดไป)*
## ลูกค้า
1. ทำการสแกนคิวอาร์โค้ดเพื่อทำการเปิดใบออเดอร์
2. สั่งรายการอาหารตามที่ต้องการ
3. เมื่อต้องการตรวจสอบรายการที่สั่งซื้อ สามารถกดปุ่มตรวจสอบเมนูที่สั่ง เพื่อดูรายการที่ตนเองสั่ง
*(กรณีลูกค้าต้องการแก้ไขรายการที่สั่งซื้อ สามารถทำการแก้ไขรายการที่สั่งซื้อได้ เมื่อเมนูที่ต้องการแก้ไขแสดงปุ่ม "แก้ไข" แต่หากไม่แสดงปุ่ม "แก้ไข" จะไม่สามารถแก้ไขในรายการนั้นได้)*
4. เมื่อลูกค้าต้องการเรียกเก็บเงินสามารถกดที่ปุ่มแจ้งจ่ายเงิน
## แม่ครัว
เเม่ครัวทำการเลือกรายการอาหารที่ต้องการจะทำการปรุงเพื่อทำการเปลี่ยนสถานะ โดยที่ในแต่ละรายการจะแสดงจำนวนของรายการที่ลูกค้าสั่งซื้อให้แม่ครัวได้ทราบ
## พนักงานเก็บเงิน
พนักงานเก็บเงินจะเห็นใบออเดอร์ที่ลูกค้าได้ทำการกดแจ้งจ่ายเงิน
1. พนักงานเก็บเงินทำการเลือกใบออเดอร์ที่ต้องการจะทำการเก็บเงิน 
2. เมื่อทำการตรวจสอบรายการอาหารที่ลูกค้าสั่งซื้อสำเร็จแล้ว สามารถกดชำระเงินสำเร็จ เพื่อยืนยันให้ทางระบบทราบว่าลูกค้าโต๊ะนั้นมีการชำระเงินเป็นที่เรียบร้อยแล้ว 

