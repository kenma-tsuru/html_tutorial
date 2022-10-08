# แบบฝึกหัด 1 เขียนโปรแกรม
* สร้างโฟลเดอร์ html_course_ex2 และเปิดเข้าไปในโฟลเดอร์
* สร้างไฟล์ `index.html` ขึ้นมา และทำตามคำสั่งดังต่อไปนี้ (สามารถดูผลลัพธ์ได้ด้วยการเปิดไฟล์นี้ด้วย browser และ refresh ก่อน 1 ครั้ง เมื่อมีการแก้ไข)
<hr>

## หมายเหตุ
* แบบฝึกหัดแต่ละข้อเติมลงในแต่ละส่วนแตกต่างกัน บางข้อเติมลงในส่วน head บางข้อเติมลงในส่วน body หากเติมลงผิดส่วน แม้ผลลัพธ์ถูกต้อง ก็จะไม่ได้คะแนน
* หากไม่ได้ระบุเป็นอย่างอื่น **ให้ครอบข้อความด้วย tag paragraph เสมอ**
* คำใบ้
    * ข้อที่เป็นข้อมูลที่เกี่ยวกับตัว HTML เติมลงใน head ส่วนข้อที่เกี่ยวกับเนื้อหาบนหน้าเว็บ ให้เติมลงใน body
    * ครอบเอกสารด้วย root element (html) เสมอ
* ให้ส่งคำตอบของแบบฝึกหัดนี้เป็น zip file ของโฟลเดอร์ html_course_ex2
<hr>

1. กำหนดรูปแบบเอกสาร (DOCTYPE) เป็น HTML
1. กำหนดภาษาของหน้า HTML เป็น "en-US"
1. กำหนดให้ title ของ HTML เป็น "Exercise 2: HTML Metadata"
1. ใส่ข้อความ *I love programming is "プログラミングが大好き" in japanese*
1. จงสร้าง metadata tag สำหรับแต่ละข้อมูลต่อไปนี้ลง โดยแต่ละข้อมูล ให้เลือกส่วนที่จะไปใส่ใน name หรือ content ให้ถูกต้อง
    * author / Jose Phillip
    * This is the webpage to answer the second exercise of the course / description
    * date / 2022-10-08
    * html for beginner / course_name

1. จงสร้างโฟล์เดอร์ ico ข้างใน html_course_ex2 แล้ว
    1. ดาวน์โหลดไอคอน (.ico) ใดก็ได้จาก https://icon-icons.com/pack/Halloween/3687 ลงในโฟลเดอร์ ico แล้วตั้งชื่อว่า favicon.ico
    2. นำไอคอนที่ดาวน์โหลดมานี้ไปใส่เป็น favicon ของ `index.html` ของเรา
1. สร้างไฟล์ my-css.css ข้างใน html_course_ex2 แล้ว
    1. กำหนดให้ backgroud ของหน้าเว็บเป็นสีฟ้า และขนาดตัวอักษรเป็น 25px (ดู code ได้จากตัวอย่าง `my-css-file.css` ใน github repo)
    1. link ไฟล์ css นี้เข้ากับหน้าเว็บด้วย metadata tag `<link>`
1. สร้างไฟล์ my-js.js ข้างใน html_course_ex2 แล้ว
    1. ทำให้มีการแสดง pop-up พร้อมข้อความ "Hello from JavaScript!" เมื่อเปิดเว็บ (ดู code ได้จากตัวอย่าง `my-js-file.css` ใน github repo)
    1. link ไฟล์ javascript นี้เข้ากับหน้าเว็บด้วย metadata tag `<script>`

# แบบฝึกหัด 2 ตอบคำถาม
* สร้าง question_answer.txt (ข้างใน html_course_ex2) แล้วใส่คำตอบของคำถามด้านล่าง โดยเขียนเลขข้อกำกับคำตอบด้วย
1. จงอธิบายความแตกต่างของ `<title>` และ `<h1>` มา 2 ข้อ
1. หากทำการ bookmark หน้าเว็บ ค่าของ `<title>` จะเป็นชื่อของ bookmark นั้น ใช่หรือไม่
1. หากต้องการให้เว็บเพจแสดงผลได้ครอบคลุมหลายภาษา ควรใช้การ encode ตัวอักษรแบบใด
1. การ encode ด้วย utf-8 ทำให้การแสดงผลภาษาญี่ปุ่นในแบบฝึกหัด 1 ข้อ 4 ต่างจากการ encode ด้วย ISO-8859-1 หรือไม่ ให้ระบุ browser ที่ใช้เปิดด้วย
1. ประโยชน์ของการมี description ใน metadata คืออะไร
1. จงระบุ metadata tag จาก https://www.geeksforgeeks.org/rust-vs-c-will-rust-replace-c-in-future/#:~:text=Rust%20is%20syntactically%20similar%20to,dangling%20pointers%20or%20null%20pointers. มา **3**  ตัวอย่าง โดยตัวอย่างแต่ละอัน ต้องนำข้อมูลมาให้ครบถ้วน ตั้งแต่เปิด tag จนกระทั่งปิด tag
1. หากต้องการใส่ metadata เกี่ยวกับ stylesheet css ต้องใช้ tag ใด
