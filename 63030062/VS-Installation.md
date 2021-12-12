# การทดลองสัปดาห์ที่ 11  #
# การใช้งาน git ร่วมกับ Visual studio IDE #


## แนะนำ IDE
  __IDE__ ย่อมาจาก __Integrated Development Environment__ เป็นซอฟต์แวร์ประยุกต์ที่รวบรวมเครื่องมือ และทรัพยากรต่าง ๆ เพื่อช่วยในการพัฒนาซอฟต์แวร์ เริ่มตั้งแต่การ coding, debugging และ deploying ซอฟต์แวร์ IDE ส่วนมากจะช่วยงานง่าย ๆ นับตั้งแต่ การตรวจสอบคำผิด เติมเต็มคำอัตโนมัติ เพื่อช่วยลดเวลาในการพิมพ์ code, ช่วยในการค้นหาและแก้ไข code ไปจนถึงการคอมไพล์ ดีบัก หรือช่วยออกแบบส่วน user interface เป็นต้น (IDE จะต่างจาก text editor ตรงที่ IDE จะรวมเอาชุด compiler สำหรับการแปลภาษา และ debugger สำหรับการค้นหาและแก้ไขข้อผิดพลาดของโปรแกรมอีกด้วย)  
  IDE ที่ใช้งานในการทดลองนี้ เป็น IDE ที่ชื่อว่า Microsoft Visual Studio รุ่น Community edition เป็น  IDE ที่ครอบคลุมการแก้ไข code ไปจนช่วยงานออกแบบ UI ตามที่เราต้องการ
	นอกจาก IDE ที่ใช้ในวิชาเรียนนี้แล้ว ในการพัฒนาโปรแกรม เราสามารถใช้  text editor ที่มีความสามารถสูง เช่น visual studio code, sublime หรืออื่น ๆ นักศึกษาสามารถศึกษาเพิ่มเติมได้จากแหล่งค้นคว้าที่ระบุในเอกสารอ้างอิง


## การติดตั้ง
<p align="center">  <img src = "./images/Fig-3.6.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.7.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.8.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.9.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.10.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.11.png" width = "80%"> </p>
<p align="center">  <img src = "./images/Fig-3.12.png" width = "80%"> </p>


## 3. การทดสอบใช้งาน

### การใช้งาน IDE ร่วมกับ repository (Github)
  
<table>
<tr> 
<td valign="top" width = "50%"><img src = "./images/Fig-3.13.png"> </p> </td>
<td valign="top">หลังจากติดตั้ง IDE และ Github extension เรียบร้อยแล้ว ให้คลิกที่เมนู View -> Team Explorer เพื่อเรียกหน้าต่าง Team Explorer ขึ้นมา จะได้หน้าต่างดังรูปซ้ายมือ </td>
</tr>
</table>   

ปุ่มกดสำหรับหน้าต่าง Team Explorer มีหน้าตาดังรูปต่อไปนี้  <img src = "./images/Fig-3.14.png">  จากซ้ายไปขวา คือปุ่ม Backward, Forward, Home, Manage connection และ Refresh ตามลำดับ ให้คลิกที่ปุ่ม manage connection ปุ่มที่ 4

<table>
<tr> 
<td valign="top" width = "50%"><img src = "./images/Fig-3.15.png"> </p> </td>
<td valign="top">เมื่อกดปุ่ม manage connection จะปรากฏ Host Service Providers พร้อมทั้งชื่อ Host คือ GitHub ให้คลิกที่ Connect… เพื่อเชื่อมต่อไปยัง Guthub
(ในกรณีที่ยังไม่มีบัญชีผู้ใช้ ให้กด Sign up เพื่อลงทะเบียนกับ GitHub ซึ่งมีทั้งชนิดฟรีและเสียค่าใช้จ่าย) </td>
</tr>
</table>   

<table>
<tr> 
<td valign="top" width = "50%"><img src = "./images/Fig-3.16.png"> </p> </td>
<td valign="top">เมื่อคลิก Connect จะปรากฏหน้าต่าง Sign in ไปยัง   Github.com ให้ใส่  User name หรือ email ที่ลงทะเบียนไว้กับ Github.com พร้อมทั้ง password แล้วกดปุ่ม <img src = "./images/Fig-3.17.png">  </td>
</tr>
</table>   



<table>
<tr> 
<td valign="top" width = "50%"><img src = "./images/Fig-3.18.png"> </p> </td>
<td valign="top">หลังจาก Sign in สำเร็จ หน้าต่าง Team Explorer จะแสดง repository ทั้งหมดที่เรามีบน Localhost (อยู่บน harddisk) 
นอกจากนี้จะมีตัวเลือก Clone | Create | Sign out  ถ้าเราคลิกที่ Clone หรือ Create ก็จะมีการแสดงหน้าจอ popup ขึ้นมา เพื่อให้ clone หรือ สร้าง repo ใหม่ตามต้องการ </td>
</tr>
</table>   


<table>
<tr> 
<td valign="top" width = "50%"><img src = "./images/Fig-3.19.png"> </p> </td>
<td valign="top">ในกรณีที่เลือก clone จะปรากฏหน้าต่าง Clone a GitHub Repository และแสดง repository  ทั้งหมดที่เรามีอยู่บน  Github 
<ul>
  <li> หากมี repo จำนวนมากก็สามารถใช้วิธีการ search ได้
  <li> เมื่อเลือก repo ที่ต้องการได้แล้ว ก็ต้องเลือก local path ที่จะ clone มาเก็บไว้
  <li> จากนั้นกดปุ่ม Clone </td>
</ul>
</tr>
</table>   



