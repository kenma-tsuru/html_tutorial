# แบบฝึกหัด
จงสร้างไฟล์ `index.html` ขึ้นมา และทำตามคำสั่งดังต่อไปนี้ (สามารถดูผลลัพธ์ได้ด้วยการเปิดไฟล์นี้ด้วย browser และ refresh ก่อน 1 ครั้ง เมื่อมีการแก้ไข)
<hr>

## หมายเหตุ
* แบบฝึกหัดแต่ละข้อเติมลงในแต่ละส่วนแตกต่างกัน บางข้อเติมลงในส่วน head บางข้อเติมลงในส่วน body หากเติมลงผิดส่วน แม้ผลลัพธ์ถูกต้อง ก็จะไม่ได้คะแนน
* คำใบ้
    * ข้อที่เป็นข้อมูลที่เกี่ยวกับตัว HTML เติมลงใน head ส่วนข้อที่เกี่ยวกับเนื้อหาบนหน้าเว็บ ให้เติมลงใน body
    * ครอบเอกสารด้วย root element (html) เสมอ
<hr>

1. กำหนดรูปแบบเอกสาร (DOCTYPE) เป็น HTML
1. กำหนดภาษาของหน้า HTML เป็น "en-US"
1. กำหนดให้ title ของ HTML เป็น "Exercise 1: Getting to known HTML"

1. ใส่ข้อความ "I love programming. I started programming with Python, then I am studying HTML" (ไม่รวมเครื่องหมายคำพูด) ลงในไฟล์ `index.html`
    1. ครอบข้อความด้วย tag paragraph
    1. ทำให้ข้อความ "love" เป็นตัวเอียง
    1. ทำให้ข้อความ "Python" และ "HTML" เป็นตัวหนา

1. ใส่รูปจาก https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Python-logo-notext.svg/1869px-Python-logo-notext.svg.png พร้อมทั้งใส่ข้อความ alternative ของรูปว่า "Python Logo"

1. ใส่ข้อความ "Click here to visit Python Tutorial"
    1. ครอบข้อความด้วย tag paragraph
    1. ใส่ hyperlink `<a>` (anchor) ครอบ "here" โดย hyperlink ต้องมีข้อมูลดังต่อไปนี้
        1. ลิงก์ไปยังหน้าเว็บ https://docs.python.org/3/tutorial/
        1. ใส่ attribute 'title' และใส่ค่าของ attribute เป็น 'python tutorial'
        1. ใส่ attribute 'target' และใส่ค่าของ attrobute เป็น '_blank' เพื่อกำหนดให้เปิดลิงก์ใน tab ใหม่


