# การทดลองสัปดาห์ที่ 11  #
# การใช้งาน git ร่วมกับ Visual studio IDE #

## การทดลอง 

### 3.1 การสร้าง repository บน GitHub ด้วย Visual Studio 


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
  <li> ในช่อง Name ให้เพิ่มชื่อ repository  <b>CL60-03</b>
  <li> ในช่อง Description ให้ใส่รายละเอียดสั้นๆ  <b>Computer Laboratory 1 : Lab 03</b>
  <li> ในช่อง Local path ให้ใส่ path ไปยังงานที่เคยทำไว้แต่อยู่ใน folder หลักเดียวกัน เช่น ถ้างานเดิม c:\Code\CL60-02 ให้ใส่เป็น  <b>c:\Code\CL60-03</b>
  <li> ในช่อง Git ignore และ License คงไว้อย่างที่ปรากฏ
  <li> กดปุ่ม <b>Create</b>
</ul>
</td>
<td valign="top"><img src = "./images/Fig-3.21.png"> </p> </td>
</tr>
</table>  

 


### เมื่อสร้างเสร็จ ให้ตรวจสอบรายการ repository ที่เพิ่มขึ้นบน GitHub.com

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
<td valign="top" width = "50%">6. เมื่อ แก้ไขเสร็จ ให้คลิกที่ Changes เพื่อดูการเปลี่ยนแปลง เทียบได้กับการสั่ง git status
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




#### ++เมื่อ sync เสร็จ ให้ตรวจสอบรายการไฟล์ใน repository บน GitHub.com++ 


### การทดลอง 3.2 การ clone จาก repository ด้วย Visual Studio

9. สร้าง repository บน GitHub.com โดยมีรายละเอียดดังนี้
    <ul>
      <li> Repository name : HelloWorld
      <li> [X] Initialize this repository with a README
      <li> [ Add .gitignore : VisualStudio] 
    </ul>
<img src = "./images/Fig-3.28.png" align = "center">

<table>
<tr> 
<td valign="top" width = "50%">10. ใน Visual Studio ให้ไปที่หน้าต่าง Team Explorer แล้วคลิกที่ Manage Connections 
 <br>11. คลิกที่ Clone </td>
<td valign="top"><img src = "./images/Fig-3.29.png"> </p> </td>
</tr>
</table>


<table>
<tr> 
<td valign="top" width = "50%">12.  ในหน้าต่าง Clone a GitHub Repository ให้เลือก repository ชื่อ HelloWorld ที่ได้สร้างไว้ในขั้นตอนที่ 8 แล้วกดปุ่ม Clone</td>
<td valign="top"><img src = "./images/Fig-3.30.png"> </p> </td>
</tr>
</table>


<table>
<tr> 
<td valign="top" width = "50%">13. ให้ Double click ที่ชื่อ repository ที่ clone มา </td>
<td valign="top"><img src = "./images/Fig-3.31.png"> </p> </td>
</tr>
</table>


<table>
<tr> 
<td valign="top" width = "50%">14. หน้าต่าง Team Explorer จะแจ้งว่ายังไม่มี Solution ใดๆ ใน repository ให้เราคลิกที่  New… เพื่อสร้าง Solution  ใหม่
<br>15. ให้ทำการสร้าง Solution พร้อมทั้ง Sync กับ Github ตามขั้นตอนที่ 4 - 8</td>
<td valign="top"><img src = "./images/Fig-3.32.png"> </p> </td>
</tr>
</table>


#### ++เมื่อ sync เสร็จ ให้ตรวจสอบรายการไฟล์ใน repository บน GitHub.com++

## การ branch 
แนวคิดในการทำ Branching เทียบเคียงกับในชีวิตประจำวัน<p>
<img src = "./images/Fig-3.33.png">
<p> แนวคิดในการทำ branching บน git อาจเทียบได้กับรูปทางด้านบน นั่นคือ การเข้าเรียนในภาควิชา ครุ.วศ. เป็นจุดเริ่มต้นของการศึกษา (หรือเทียบได้กับพัฒนา Project ของเรา) โดยแต่ละ commit (แทนด้วยสัญลักษณ์วงกลม) อาจจะหมายถึงการเรียนในแต่ละภาคการศึกษา ในแต่ละ commit จึงเป็นการเพิ่มรายวิชาลงในทรานสคริปต์ (ตามเทอมที่ลงทะเบียน) เมื่อนักศึกษาขึ้นชั้นปีที่ 2 จะต้องแยกกันไปเรียนตามความถนัดหรือตามความสามารถที่ต้องการพัฒนา จนกระทั่งจบชั้นปีที่ 4 จะต้องกลับมารวมกันอีกครั้ง เพื่อออกไปทำการฝึกสอนในฐานนะนักศึกษา ภาควิชา ครุ.วศ. </p>
<p> ในการพัฒนา software มีบ่อยครั้งที่เราต้องทำการเพิ่มเติมความสามารถพิเศษให้กับซอฟต์แวร์ หรือทำการแก้ bug ที่พบ โดยไม่ต้องการให้เกิดผลกระทบต่อ source code ที่อยู่ในสาขาหลัก (master)  เราจึงต้องทำการแยกแขนง (branch) ออกมาเพื่อพัฒนา ซึ่งในการแยก branch ออกมาพัฒนานี้ ก็ยังสามารถทำงานเป็นทีมและยังคงต้อง clone มาทำงานกับ local repository เช่นเดียวกัน </p>


## การทดลอง 3.3 การทำ Branching

16. ในหน้าต่าง Team Explorer  ให้ทำการสร้าง repository  ใหม่ โดยใช้ชื่อว่า EngEdu<p>
<img src = "./images/Fig-3.34.png">

17. ทำการเพิ่ม Solution ให้กับ repository ใช้ชื่อว่า EngEdu 
    <ul>
        <li> ชนิดเป็น Console App (.NET Framework)
        <li> Location คงไว้อย่างที่ปรากฏ
        <li> แก้ไขโปรแกรมให้เป็นดังรูปด้านล่างนี้
    </ul>

<img src = "./images/Fig-3.35.png">

18. ทำการ sync กับ GitHub.com
    <ul>
        <li> ใช้ commit message <b>“first year semester 1”</b>
        <li> ดูการเปลี่ยนแปลงของ repository EngEdu บน GitHub.com
    </ul>    




19. ทำการเพิ่มเติมไฟล์ __Program.cs__ โดยเพิ่มข้อความดังต่อไปนี้<p>
<img src = "./images/Fig-3.36.png">

20. ทำการ sync กับ GitHub.com
    <ul>
        <li> ใช้ commit message <b>“first year semester 2”</b>
        <li> ดูการเปลี่ยนแปลงของ repository EngEdu บน GitHub.com
    </ul>    



เมื่อนักศึกษาเรียนถึงชั้นปีที่ 2 จะต้องมีการแยกแขนงวิชา เพื่อศึกษาในแขนงวิชาที่ตนถนัด หรือต้องการพัฒนาศักยภาพเป็นพิเศษ เมื่อนักศึกษาแยกแขนงออกมาแล้ว ก็จะต้องเรียนในวิชาของแขนงวิชาเป็นหลัก แต่จะยังคงมีนักศึกษาบางส่วน ที่พักการเรียนในบางวิชาของปี 1 เทอม 1  จึงต้องลงทะเบียนใน ปี 2 เทอม 1 ซึ่งจะยังคงเดินตามแผนการศึกษาในรายวิชาของภาควิชาต่อไป (เรียกชื่อ branch นี้ว่า  master) 
ทำนองเดียวกัน ในการพัฒนาซอฟต์แวร์ เมื่อได้วางตลาดรุ่นที่ 1.0 แล้ว ก็อาจจะต้องมีการพัฒนา features เพิ่มเติม เป็นรุ่น 1.1, 1.2, … หรือรุ่น 2.0 สิ่งหนึ่งที่นักพัฒนาต้องพบกับความยุ่งยากคือ การพัฒนารุ่นใหม่ ไปพร้อมๆ กับการแก้บักของรุ่นเก่า จะเกิดความยุ่งยากในการรักษา code เพื่อไม่ให้ code ของแต่ละรุ่นหรือแต่ละความมุ่งหมายในการพัฒนารบกวนกัน ความสามารถด้าน branching ของ Git จึงเข้ามามีบทบาทสำคัญ
 
 

<table>
<tr> 
<td valign="top" width = "50%">21. การแยก branch ใน Visual Studio
    <ul>
        <li> ในหน้าต่าง Team Explorer ให้คลิกที่ Home และ Branches (อยู่ภายใต้หัวข้อ Project)
    </ul>    
</td>
<td valign="top"><img src = "./images/Fig-3.37.png"> </p> </td>
</tr>
</table>

<table>
<tr> 
<td valign="top"  width = "50%">22. ภายใต้หัวข้อ  Active Git Repositories จะพบว่ามี Repo ของเราตามด้วย (master) และมี branch ที่ชื่อว่า master เป็นโหนดลูก แสดงเป็นตัวหนา
    <ul>
        <li> คลิกขวาที่ branch master
        <li> เลือก New Local Branch From...
    </ul>    
</td>
<td valign="top"><img src = "./images/Fig-3.38.png"> </p> </td>
</tr>
</table>

<table>
<tr> 
<td valign="top"  width = "50%">23. ตั้งชื่อ  Branch
    <ul>
        <li> ใส่ชื่อ Branch เป็น Computer
        <li> คลิก Create Branch
    </ul>    
สังเกตว่า ในโหนด Engedu จะมีการแสดงเป็น  EngEdu (Computer) และโหนดลูกที่ชื่อ Computer จะเปลี่ยนเป็นตัวหนาขณะที่ master กลายเป็นตัวปกติ นั่นคือ ขณะนี้ เราได้ย้ายไปทำงานใน branch ที่ชื่อ Computer
  
<p><p>
<b>***** การเปลี่ยนแปลงใด ๆ จะถูกกระทำภายใต้ branch ปัจจุบัน (ที่แสดงด้วยตัวหนา) เท่านั้น ***** </b>
<p><p>
    
การเปลี่ยน branch ทำได้ง่ายๆ โดยการ double  click ที่ชื่อ branch 

<b>***** ทุกครั้งที่มีการเปลี่ยน branch </b>
1. git จะลบไฟล์ทั้งหมดใน working directory 
2. git จะทำการ checkout ไฟล์ใน branch ปัจจุบันออกมาทำงาน  แทนไฟล์ทั้งหมดใน working directory

</td>
<td valign="top"><img src = "./images/Fig-3.39.png"> </p> </td>
</tr>
</table>

 
24. ทำให้แน่ใจว่า เรากำลังทำงานกับ Branch ที่ชื่อ  Computer 
    <ul>
        <li>ในโหนด Engedu จะต้องแสดงเป็น  EngEdu (Computer) และโหนดลูกที่ชื่อ Computer จะต้องเป็นตัวหนา
        <li>แก้โปรแกรมเป็นดังต่อไปนี้ 
    </ul>
<img src = "./images/Fig-3.40.png">


25. ทำการ sync กับ GitHub.com
    <ul>
        <li>ใช้ commit message <b>"2nd  year semester 1"</b>
        <li>ดูการเปลี่ยนแปลงของ repository EngEdu บน GitHub.com
        <li><b>กรณีที่ Sync  ไม่สำเร็จ ให้ลองใช้การ push เนื่องจากในขณะนี้ ยังไม่มี branch ที่ชื่อ Computer บน GitHub.com</b>
    </ul>


26. เปลี่ยน Branch กลับไปยัง master โดยการ double click ที่ master
    <ul>
        <li>สังเกตุการเปลี่ยนแปลงที่เกิดขึ้นกับไฟล์ Program.cs
        <li>ทดลองสลับไปมาระหว่าง branch ที่ชื่อ master และ Computer (โดยการ double click)
    </ul>



27. ทำให้แน่ใจว่า เรากำลังทำงานกับ Branch ที่ชื่อ  master
    <ul>
        <li>ในโหนด Engedu จะต้องแสดงเป็น  EngEdu (master) และโหนดลูกที่ชื่อ master จะต้องเป็นตัวหนา
        <li>แก้โปรแกรมเป็นดังต่อไปนี้ 
    </ul>
<img src = "./images/Fig-3.41.png">

<p>

28. ทำการ sync กับ GitHub.com
    <ul>
        <li>ใช้ commit message “2nd  year semester 1”
        <li>ดูการเปลี่ยนแปลงของ repository EngEdu บน GitHub.com
        <li><b>กรณีที่ Sync  ไม่สำเร็จ ให้ลองใช้การ push เนื่องจากในขณะนี้ ยังไม่มี branch ที่ชื่อ Computer บน GitHub.com</b>

    </ul>

29. เปลี่ยน Branch กลับไปยัง Computer โดยการ double click ที่ Computer
    <ul>
        <li>สังเกตุการเปลี่ยนแปลงที่เกิดขึ้นกับไฟล์ Program.cs
        <li>ทดลองสลับไปมาระหว่าง branch ที่ชื่อ master และ Computer (โดยการ double click)
    </ul>

### แบบฝึกหัด
ให้ทำการเพิ่ม commit ตามภาคการศึกษาต่างๆ โดยเขียน Hilight ที่นักศึกษาคิดว่าที่จะพบในแต่ละภาคการศึกษา จนถึงชั้นปีที่ 4 ภาคเรียนที่ 2

เมื่อเราพัฒนาซอฟต์แวร์ โดยการแยก branch และคิดว่าถึงจุดหนึ่งที่สามารถนำไปรวมกับ master ได้ เราจะต้องทำการ merge เพื่อรวม branch เข้าด้วยกัน ซึ่งการ merge นี้ระบบของ git จะทำการตรวจเช็คให้ด้วย ว่าสามารถ merge ได้หรือไม่

30. การรวม Branch (merge)
    <ul>
        <li>ทำให้แน่ใจว่าอยู่ที่ Branch ปลายทางที่จะทำการ merge  ในที่นี้คือ master ดังนั้น ที่โหนด  EngEdu ต้องแสดงเป็น EngEdu (master) และโหนดลูก master ต้องเป็นตัวหนา
        <li>คลิกขวาที่โหนดลูก เลือก Merge From… จากเมนูป๊อบอับ
    </ul>
<img src = "./images/Fig-3.42.png">

<p>
    
<table>
<tr> 
<td valign="top"  width = "50%">31. ทำการ merge
    <ul>
        <li> Merge from branch : Computer 
        <li> Into current branch: master
        <li> คลิก Merge
    </ul>    
</td>
<td valign="top"><img src = "./images/Fig-3.43.png"> </p> </td>
</tr>
</table>

<p>
    
<table>
<tr> 
<td valign="top" width = "50%">32. Merge conflict<p>
ในการ merge เราจะพบว่า บางครั้งมีการแก้ไข source code ที่หมายเลขบรรทัดเดียวกัน บนไฟล์เดียวกัน กรณีนี้เรียกว่าเกิดการขัดแย้ง
เราต้องดำเนินการอย่างใดอย่างหนึ่ง เพื่อจัดการกับความขัดแย้งนั้น เพื่อให้สามารถดำเนินการพัฒนาซอฟต์แวร์ต่อไปได้
ถ้าเจอสถานการณ์นี้ ให้คลิก Conflict: 1</td>
<td valign="top"><img src = "./images/Fig-3.44.png"> </p> </td>
</tr>
</table>


    
<p>
    
<table>
<tr> 
<td valign="top" width = "50%">33. การแก้ไข Merge conflict<p>
    ในการ merge เราจะพบว่า บางครั้งมีการแก้ไข source code ที่หมายเลขบรรทัดเดียวกัน บนไฟล์เดียวกัน กรณีนี้เรียกว่าเกิดการขัดแย้ง
ให้คลิกที่ชื่อไฟล์ที่ขัดแย้งนั้น จะพบว่า เราสามารถแก้ไขได้ในหลายรูปแบบเช่น
<ol>
    <li> ยกเลิกการ merge โดยการคลิกที่  Undo Merge </li>
    <li> เปรียบเทียบความแตกต่างระหว่างไฟล์ทั้งสอง โดยการคลิกที่ Compare file
    <li> เข้าไปแก้ไขไฟล์ใน branch ปลายทาง
    <li> เข้าไปแก้ไขไฟล์ที่นำมา merge
</ol>

ให้นักศึกษาทดลองคลิกที่ตัวเลือกต่างๆ 

__ถ้าต้องการกลับไปก่อนการ merge ให้กด Undo merge__</td>
<td valign="top"><img src = "./images/Fig-3.45.png"> </p> </td>
</tr>
</table>


34. ดูผลการเปลี่ยนแปลงหลังจากการ merge
    <ul>
        <li> สังเกตุการเปลี่ยนแปลงที่เกิดขึ้นกับไฟล์ Program.cs
        <li> ทดลองสลับไปมาระหว่าง branch ที่ชื่อ master และ Computer (โดยการ double click)
    </ul>    


## คำถาม

<ol>
<li> ในกรณีที่ต้องการรักษา source code ของทั้งสองไฟล์ไว้ ควรทำอย่างไร
<li> ผลของการ keep target ออกมาเป็นอย่างไร
<li> ผลของการ take source ออกมาเป็นอย่างไร
<li> ให้ capture หน้าจอของ Compare files, Diff ที่ source, Diff ที่ target
</ol>

__หมายเหตุ หากนักศึกษาทำการทดลองเพื่อที่จะตอบคำถามข้างต้น แล้วทำให้เกิดผลที่ไม่คาดคิด ให้กด `Undo merge`__


