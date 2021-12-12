# การทดลองสัปดาห์ที่ 11 #

# การใช้งาน git ร่วมกับ Visual studio IDE 2017 #

---

## 11.1 การสร้าง repository บน GitHub ด้วย Visual Studio ##

<table>
<tr>
<td valign="top"  width = "50%">ในแท็บ Team Explorer ให้สร้าง repository โดยการคลิกปุ่ม <b>Create</b></td>
<td valign="top "><img src = "./images/Fig-3.20.png"> </p> </td>
</tr>
</table>  

<table>
<tr>
<td valign="top"  width = "50%">ระบุรายละเอียดของ repo ใหม่ที่จะสร้าง
<ul>
  <li> ในช่อง Name ให้เพิ่มชื่อ repository  <b>CL64-xxx-week11</b>
  <span style="color:blue">โดย xxx คือเลขสามตัวท้ายของรหัสนักศึกษา</span>
  <li> ในช่อง Description ให้ใส่รายละเอียดสั้นๆ  <b>Computer Laboratory 1 :  week 11</b>
  <li> ในช่อง Local path ให้ใส่ path ไปยังงานที่เคยทำไว้แต่อยู่ใน folder หลักเดียวกัน เช่น ถ้างานเดิม c:\Code\ ให้ใส่เป็น  <b>c:\Code\CL64-xxx-week11</b>
  <li> ในช่อง Git ignore และ License คงไว้อย่างที่ปรากฏ
  <li> กดปุ่ม <b>Create</b>
</ul>
</td>
<td valign="top"><img src = "./images/Fig-3.21.png"> </p> </td>
</tr>
</table>  

### เมื่อสร้างเสร็จ ให้ตรวจสอบรายการ repository ที่เพิ่มขึ้นบน GitHub.com ###

```
  
  อธิบายสิ่งที่พบ บน github.com ว่ามี repository ที่เราเพิ่งสร้างบน Visual Studio หรือไม่ 
  - ถ้าไม่มี ปัญหาเกิดจากอะไร ให้ copy ข้อความผิดพลาดหรือหน้าจอมาใส่ในเอกสารนี้ด้วย 

```
### มี repository ปรากฎขึ้นบน github.com หลังสร้าง repository ด้วย Visual Studio ###
<img src = "./image_tosubmit/Picture4.png">

<table>
<tr>
<td valign="top"  width = "50%">3. เพิ่ม solution ใหม่ไปยัง repository<br>
คลิกที่ New… จะปรากฏหน้าต่าง ให้สร้าง Solution ใหม่ ให้ทำตามข้อ 4
</td>
<td valign="top"><img src = "./images/Fig-3.22.png"> </p> </td>
</tr>
</table>

4. ใส่รายละเอียดของ Solution  ใหม่ที่ต้องการสร้าง

<img src = "./images/Fig-3.23.png">

5. เมื่อ Solution ใหม่ถูกสร้างขึ้นมา ให้แก้ไข code ตามรูปต่อไปนี้
<img src = "./images/Fig-3.24.png">

<table>
<tr>

ทดลอง Build และ Run โปรแกรมที่ได้ ว่ามีความถูกต้องหรือไม่ ให้แก้ไขจนกว่าจะได้โปรแกรมที่ถูกต้องและรันได้ตามต้องการ

```
บันทึกหน้าจอที่ได้ 

```

<img src = "./image_tosubmit/Picture5.png">

<td valign="top" width = "50%">6. เมื่อได้โปรแกรมที่สมบูรณ์แล้ว ขั้นต่อไปคือการเก็บโปรแกรมนี้ไว้ในที่ปลอดภัย เพราะเราอาจจะทำการแก้ไขโปรแกรมนี้ในอนาคต หากเกิดข้อผิดพลาดกับโปรแกรมที่แก้ไขนั้น หรือต้องการใช้งานโปรแกรมรุ่นนี้ ก็จะสามารถย้อนกลับมาดึง code ที่เคยทำงานได้นี้กลับมาในทันที ไม่ต้องเขียนใหม่
<br><br> ให้คลิกที่ <b>Changes</b> เพื่อดูการเปลี่ยนแปลง (เทียบได้กับการสั่ง git status)
</td>
<td valign="top"><img src = "./images/Fig-3.25.png"> </p> </td>
</tr>
</table>

<table>
<tr>
<td valign="top" width = "50%">7. Team Explorer จะรายงานไฟล์ที่มีการเปลี่ยนแปลง พร้อมทั้งมีช่่องให้ใส่ข้อความสำหรับการ  commit  เมื่อกรอกข้อความเสร็จให้คลิกปุ่ม Commit All
</td>
<td valign="top" ><img src = "./images/Fig-3.26.png" > </p> </td>
</tr>
</table>

การสั่ง Commit All จะเป็นการเก็บบันทึกการเปลี่ยนแปลงที่แสดงในรูปไว้ใน Local repository ถ้าหากเราต้องการบันทึกการเปลี่ยนแปลงไว้บนเวบ GitHub จะต้องทำการ Sync  ซึ่งคำสั่ง Sync  นี้จะทำการ pull และ push ให้เราโดยอัตโนมัติทั้ง 2 คำสั่ง

<table>
<tr>
<td valign="top" width = "50%" >8. ให้ทำการ sync repo ที่เราสร้างขึ้นไปบน Github</td>
<td valign="top" ><img src = "./images/Fig-3.27.png"> </p> </td>
</tr>
</table>

__การสร้าง solution ใหม่ จะสร้างขึ้นใน working directory เหมือนการทำงานตามปกติ ในขณะที่เรากำลังพัฒนาโปรแกรมนั้น จะไม่มีการรบกวนใดๆ ทั้งสิ้น จาก git__

#### ++เมื่อ sync เสร็จ ให้ตรวจสอบรายการไฟล์ใน repository บน GitHub.com++ ###

```
  
  อธิบายสิ่งที่พบ บน github.com 
  สามารถ capture หน้าจอมาใส่ในเอกสารนี้ได้ 


```

