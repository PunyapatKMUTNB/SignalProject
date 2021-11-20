# mini-project-010123106 Intro to Signals &amp; Systems (1/2564)
presentation video : https://www.youtube.com/watch?v=0IXh_XjhwVc

## หัวข้อที่เลือกทำ : หัวข้อที่ 1
- ผู้ใช้เลือกชนิดของสัญญาณมีคาบ จาก dropdown menu เช่น square, triangular, PWM, ....
- ตั้งค่าตัวเลขสำหรับพารามิเตอร์สำหรับสัญญาณที่เลือก เช่น แอมพลิจูด, ความถี่, ...
- แสดงรูปคลื่นสัญญาณตามพารามิเตอร์ของสัญญาณที่ผู้ใช้ปรับเปลี่ยน 

กลุ่มเราคาดว่า หัวข้อที่ 1 เป็นการทำงานเสมือนกับเครื่อง Function Generation จำลองที่สามารถใส่ค่า input ต่างๆ แสดงให้เห็น graph รูปคลื่นสัญญาณ ในรูปแบบต่างๆ

## วัตถุประสงค์ : 
- ศึกษาการใช้งาน MATLAB App Designer และการแปลงให้ได้ Desktop App / Web App
- ศึกษาการใช้งาน UI Components ชนิดต่าง ๆ
- ศึกษาการเขียนโค้ดแบบ OOP ด้วย MATLAB
- ออกแบบและสร้าง GUI APP เพื่อการประยุกต์ใช้งาน
- การสร้าง GUI Application โดยใช้ MATLAB App Designer

## ที่มาของสูตร : 	
![image](https://drive.google.com/uc?export=view&id=1Bn-b566dk90JI7QM29pZR-d6vvnNTcbV)
Different Forms of Fourier Series (3)

![image](https://drive.google.com/uc?export=view&id=1O9JTARwpv0l3cSCktpavUPpjpHivuQg9)
![image](https://drive.google.com/uc?export=view&id=1Q3brmnT4HvfG_KxdMO6DewxLJ7jl-SHj)

ดูค่าจากตาราง Table of Fourier Series for Basic Periodic Signals ที่มีให้ในหน้า 43 และ หน้า 44 
จาก https://drive.google.com/file/d/1dpi_vo6R8Oz-uJMQwBLeGo_b5egUhFuB/view

นำค่ามาแทนใน Different Forms of Fourier Series (3) ซึ่งจะได้สมการ Fourier ไว้ในการวาดกราฟรูปสัญญาณตามที่ผู้ใช้ใส่ค่า input เข้ามาได้

<a href="https://drive.google.com/uc?export=view&id=1pz3lDwT1pYd6GlV8TY0Gc4HNaQH9ysqh"><img src="https://drive.google.com/uc?export=view&id=1pz3lDwT1pYd6GlV8TY0Gc4HNaQH9ysqh" style="width: 750px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a>

<a href="https://drive.google.com/uc?export=view&id=1R0gk1MfXulkS8cvvMKSJB2xLXhHjxpae"><img src="https://drive.google.com/uc?export=view&id=1R0gk1MfXulkS8cvvMKSJB2xLXhHjxpae" style="width: 750px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a>

<a href="https://drive.google.com/uc?export=view&id=1Db8jEao4XgiuPhxoM2gopmiC1EkIlDsS"><img src="https://drive.google.com/uc?export=view&id=1Db8jEao4XgiuPhxoM2gopmiC1EkIlDsS" style="width: 750px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a>

<a href="https://drive.google.com/uc?export=view&id=1XdLpmEzUQW00OoPh_1MgugW3IEUyUsNE"><img src="https://drive.google.com/uc?export=view&id=1XdLpmEzUQW00OoPh_1MgugW3IEUyUsNE" style="width: 750px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a>

-------------------------------------

## หลักการทำงาน : 
<a href="https://drive.google.com/uc?export=view&id=1jrl5wrOSx010KyI51VYa6iEYcb0PMDlh"><img src="https://drive.google.com/uc?export=view&id=1jrl5wrOSx010KyI51VYa6iEYcb0PMDlh" style="width: 400px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a> 
<a href="https://drive.google.com/uc?export=view&id=11xdxkjVr-YeEZ_gEbqkG7YBKfdQI7fMp"><img src="https://drive.google.com/uc?export=view&id=11xdxkjVr-YeEZ_gEbqkG7YBKfdQI7fMp" style="width: 400px; max-width: 100%; height: auto" title="Click to enlarge picture" /></a>
  
- เริ่มต้น กดเปิด switch (power : off/on) กดให้ power เปิด on ตัว graph จะทำงานตามค่าที่ input ที่เริ่มแรก  ( function : sine, freq : 1000Hz, amp : 1V, DC offset : 0V, phase : 0 degree, volt/dv : 1V, time/dv : 1ms )

![image](https://drive.google.com/uc?export=view&id=11xdxkjVr-YeEZ_gEbqkG7YBKfdQI7fMp)

- เราสามารถ ปรับค่า/เปลี่ยน function ได้ เมื่อ ปรับค่า/เปลี่ยน function ตัว graph ด้านขวาจะเปลี่ยนให้ทันทีใน ณ power on เมื่อเรากด power off จะทำให้ graph จะ ไม่เขียน/ไม่ทำงาน ทันที

![image](https://drive.google.com/uc?export=view&id=19EqKBizbY0x9i9zGnULQJdvzhMvs2xwo)

- ค่าที่ไว้ปรับ รูปคลื่นสัญญาณ
  - frequency (ความถี่ : Hz) : เพิ่มค่า frequency รูปคลื่นสัญญาณจะถี่มากขึ้น คาบเวลาจะน้อยลง และลดค่า frequency รูปคลื่นสัญญาณจะถี่น้อยลง คาบเวลาจะมากขึ้น ในโปรแกรมของเรา ไม่สามารถใส่ค่าติดลบได้
  - amplitude (แอมพลิจูด : V) : amplitude ในที่นี้จะเป็นแบบ Peak amplitude เพิ่มค่า amplitude ความสูง/ความลึกของสันคลื่นและท้องคลื่นในรูปคลื่นสัญญาณจะเพิ่มขึ้น และลดค่า amplitude ความสูง/ความลึกของสันคลื่นและท้องคลื่นในรูปคลื่นสัญญาณจะลดลง ไม่สามารถใส่ค่าติดลบได้
  - DC offset  (V) : เพิ่มค่า DC offset รูปคลื่นสัญญาณจะเลื่อนขึ้น และลดค่า DC offset รูปคลื่นสัญญาณจะเลื่อนลง โดยปกติ DC offset จะถูกใช้ในการทำให้ค่าของกราฟในโดเมนฝั่งบวกและฝั่งลบเท่ากัน
  - phase  (เฟส : degree) : เพิ่มค่า Leading phase องศาของรูปคลื่นสัญญาณจะเริ่มไปข้างหน้าที่เราเพิ่มองศา และเพิ่มค่า (Lagging) phase  องศาของรูปคลื่นสัญญาณจะเริ่มถอยหลังที่เราเพิ่มองศา 

- ค่าที่ไว้ปรับ ขยาย/ย่อ กราฟ
  - volt/div  (V) : เพิ่มค่า volt/div ลดขนาดรูปคลื่นสัญญาณ เพิ่มขอบเขตของตาราง (แกน Y) และลดค่า volt/div เพิ่มขนาดรูปคลื่นสัญญาณ ลดขอบเขตของตาราง (แกน Y) ไม่สามารถใส่ค่าติดลบได้
  - time/div  (s) : เพิ่มค่า time/div  บีบขนาดรูปคลื่นสัญญาณให้แคบลง เพิ่มขอบเขตของตาราง (แกน X) และลดค่า time/div ขยายขนาดรูปคลื่นสัญญาณให้กว้างขึ้น ลดขอบเขตของตาราง (แกน X) ไม่สามารถใส่ค่าติดลบได้

## ตัวอย่าง GUI :
- กราฟของ sine wave เมื่อเราปรับ frequency : 3000 Hz

![image](https://drive.google.com/uc?export=view&id=1FtmMTA49aUm_trXMoMvjbzMN3zIwwQi9)

- กราฟของ square wave เมื่อเราปรับ frequency : 2000 Hz, amplitude : 2 Volt, phase: Lagging  90 degree, volt/div : 5 Volt  และ time/div : 4 ms

![image](https://drive.google.com/uc?export=view&id=1vBs3bAv1t_fabCQQ6WjtYiqAlS4eM9_n)

- กราฟของ triangular wave เมื่อเราปรับ frequency : 1000 Hz, amplitude : 1 Volt, volt/div : 1.5 Volt  และ time/div : 4 ms

![image](https://drive.google.com/uc?export=view&id=1m4C27en1Y6RLZttOYNtiZ659Q-eCtyEn)

- กราฟของ sawtooth wave เมื่อเราปรับ frequency : 1500 Hz, amplitude : 3 Volt, DC offset : -3 Volt, phase: Lagging  90 degree, volt/div : 5 Volt  และ time/div : 4 ms

![image](https://drive.google.com/uc?export=view&id=1KddGR8Z9gESJzD9RzgkdK77ZGspQOzuP)

- กราฟของ full-wave เมื่อเราปรับ frequency : 2500 Hz, amplitude : 5 Volt, DC offset : -0.5 Volt, phase: Leading  90 degree, volt/div : 3 Volt  และ time/div : 4 ms

![image](https://drive.google.com/uc?export=view&id=1z9DZKO_x2IrQFBsFMMANn15ogTKofNhu)

- กรณีที่ไม่สามารถ ใส่ค่าติดลบ ได้ (frequency,  amplitude, volt/dv, และ time/dv)

![image](https://drive.google.com/uc?export=view&id=1j0F3TU1i7l7lFVKjIVolnkmLGzF68_tL)


## สมาชิก :
ปุญญาพัฒน์ มีมา 6301012620057 <br />
นรเศรษฐ์ กุวะลัย  6301012610051 <br />
สิทธิกร อิ่มโค่น 6301012620090 <br />
นทณรรณ ศรีจันทร์ 6301012630095 <br />
