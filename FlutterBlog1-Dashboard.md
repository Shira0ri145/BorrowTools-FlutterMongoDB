# Dashboard Test
## Summary
ใน Chapter นี้เราจะลองทำ Dashboard สำหรับทำงาน admin กัน

##Create Flutter app
พิม flutter create [ name ] เพื่อสร้าง project
<img width="701" alt="image" src="https://user-images.githubusercontent.com/101574457/222680296-6dd28093-a193-49e6-99cd-706e2536c2f7.png">

ทกการสร้าง Directory ไว้แยกเก็บ MVC Model View Controller                                                                           
<img width="160" alt="image" src="https://user-images.githubusercontent.com/101574457/222689762-c677c398-7eea-491b-b6fc-1ab22e7c462c.png">


## GetX
GetX เป็นแพ็กเกจสำหรับ Flutter ที่มีไว้สำหรับจัดการสถานะและการเปลี่ยนแปลงของเวิร์กโฟลว์ของแอพพลิเคชัน เช่น การจัดการสถานะการเชื่อมต่อกับเซิร์ฟเวอร์ การเปลี่ยนแปลงข้อมูลในการทำงาน การโต้ตอบกับผู้ใช้และอื่นๆ โดยเฉพาะอย่างยิ่งเมื่อเราต้องการจัดการสถานะของแอพพลิเคชันอย่างมีประสิทธิภาพ นอกจากนี้ GetX ยังเป็นแพ็กเกจที่ช่วยให้สามารถใช้งาน State Management, Dependency Injection และการนำเสนอหน้าจอได้อย่างมีประสิทธิภาพใน Flutter ได้อีกด้วย

การเพิ่ม Get คือนำ package get: ^4.6.5 ไปใส่ใน pubspec.yaml                                                                               
<img width="225" alt="image" src="https://user-images.githubusercontent.com/101574457/222689660-c524bff9-7fa0-411d-9f41-0b2fef357d69.png">


ไปที่ main.dart ลบ class MyHomePage และ _MyHomePageState เราจะทำการแยกไปอีกไฟล์นึงเพื่อให้มีความเป็นระเบียบสะอาดตา
<img width="390" alt="image" src="https://user-images.githubusercontent.com/101574457/222691255-e4bb610a-c009-48ce-8d2a-334ba3dfdbcf.png">

สร้าง ไฟล์ใหม่ที่ Directory Screen ชื่อว่า Homepage.dart จากนั้น พิมว่า stl จะมี dropdown ขึ้นมาให้เลือก flutter StatelessWidget จะเป็นการสร้าง StatelessWidget ขึ้นมาทันที
<img width="518" alt="image" src="https://user-images.githubusercontent.com/101574457/222692368-f24566dc-c13e-4b2a-98a5-f613d9a605c6.png">

ทำการแก้ชื่อ class เป็น HomeScreen และเขียนสร้าง widget ใน Template Homepage                              
<img width="816" alt="image" src="https://user-images.githubusercontent.com/101574457/222722055-4f6ad5e5-707b-4199-8a4d-7c33ba68654f.png">
สิ่งที่เขียนใน Template มีดังนี้
  1
