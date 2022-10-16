# แบบฝึกหัด 3 เขียนโปรแกรม
* สร้างโฟลเดอร์ html_course_ex3 และเปิดเข้าไปในโฟลเดอร์
* สร้างไฟล์ `index.html` ขึ้นมา และทำตามคำสั่งดังต่อไปนี้ (สามารถดูผลลัพธ์ได้ด้วยการเปิดไฟล์นี้ด้วย browser และ refresh ก่อน 1 ครั้ง เมื่อมีการแก้ไข)

1. ใส่ข้อความ "Click here to read stock news" และครอบข้อความด้วย tag paragraph
   1. ใส่ลิงค์ https://www.cnbc.com/world/?region=world ครอบคำว่า "here"
   2. ใส่ title ด้วยค่า "CNBC news"

2. ใส่รูปภาพ logo facebook (รูปใดก็ได้จาก google search)
   1. ใส่ลิงค์ https://www.facebook.com/ ครอบรูปภาพ
   2. ใส่ title ด้วยค่า "Facebook homepage"

3. ใส่ข้อความ "infinite width networks in neural tangent kernel" และใส่ลิงค์ https://lilianweng.github.io/posts/2022-09-08-ntk/ ครอบข้อความนี้ โดยเมื่อให้คลิกลิงค์แล้ว ให้โชว์ส่วนที่เป็นหัวข้อ infinite width networks
4. จงเติม table of content ด้านบน ในไฟล์ jeff-bernat-playlist.html ให้สมบูรณ์ โดย
   1. ลิสต์ชื่อเพลงที่ปรากฏในหน้าเว็บออกมาเป็น unordered list 
   2. ใส่ h1 ให้กับชื่อเพลง (แต่ละเพลงเว้น 2 บรรทัด)
   3. ใส่ id ให้แต่ละชื่อเพลง
   4. ลิงค์แต่ละเพลงเข้ากับรายชื่อเพลงใน table of content (เมื่อคลิกที่ชื่อเพลง หน้าเว็บจะเลื่อนไปยังเพลงนั้น)

5. จงสร้างลิงค์สำหรับดาวน์โหลดไฟล์ https://cses.fi/book/book.pdf 
   1. กำหนดข้อความเป็น "click here to download the book"
   2. แนบลิงค์ตรงคำว่า "here" 
   3. กำหนดชื่อไฟล์เมื่อดาวน์โหลดเป็น "competitive-programming-book.pdf"


# แบบฝึกหัด 3 ตอบคำถาม
* สร้าง question_answer.txt (ข้างใน html_course_ex3) แล้วใส่คำตอบของคำถามด้านล่าง โดยเขียนเลขข้อกำกับคำตอบด้วย


1. กำหนดไฟล์ และไดเรกทอรี่ดังต่อไปนี้

```text
.
├── src/
│   ├── header.png
│   ├── profile.png
│   ├── images/
│   │   ├── food.png
│   │   └── fruit.png
│   └── recipes/
│       ├── tom-yum-kung.txt
│       └── pad-thai.txt
├── contact.html
├── profile.html
└── index.html
```

หากต้องการลิงค์จากไฟล์ index.html ไปยังไปยังไฟล์ต่อไปนี้ ต้องใส่ค่าใน href อย่างไร

    1. contact.html
    2. profile.png
    3. fruit.png
    4. pad-thai.txt


2. การใส่ค่า `download="cp-book.pdf"` กับ `download` เฉยๆ ใน hyperlink ให้ผลแตกต่างกันอย่างไร