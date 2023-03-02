# Welcome to My Database class repository!

## Installations [Mac os]
Spec Required
  - Operating Systems: macOS
  - Disk Space: 2.8 GB (does not include disk space for IDE/tools).
  - Tools: Flutter uses git for installation and upgrade. We recommend installing Xcode, which includes git, but you can also install git separately.

โหลด Flutter SDK มาใช้ในกรณีของผมใช้เป็นสถาปัตยกรรม ARM จังเลือกแบบ Apple Silicon 
  - Tips - SDK ย่อมาจาก Software Development Kit
  <img width="722" alt="image" src="https://user-images.githubusercontent.com/101574457/222463238-2d5e1d02-ba91-4069-9bf6-630250eb9b04.png">                                    

สร้างโฟลเดอร์ชื่อ Development                                                         
  <img width="713" alt="image" src="https://user-images.githubusercontent.com/101574457/222466804-660e28ed-bf3b-498f-a470-8e338901d676.png">

นำ Flutter file มาวาง                                       
  <img width="276" alt="image" src="https://user-images.githubusercontent.com/101574457/222467290-0e98101f-7e64-466e-b73f-14f3eae7f1f3.png">

## Update your path
เราจะอัพเดท path เพื่อให้ใช้ Flutter ได้

ไปที่ Terminal พิมว่า echo $SHELL
<img width="367" alt="image" src="https://user-images.githubusercontent.com/101574457/222468512-04d3cbb1-715f-4ca8-8160-ee35999f8ef4.png">

ทำการสร้าง .zshrc ขึ้นมาและเปิดมัน
  - ถ้าจะใช้ Bash ให้แก้ไข $HOME/.bash_profile หรือ $HOME/.bashrc
  - ถ้าใช้ Z shell ให้แก้ไข $HOME/.zshrc
<img width="466" alt="image" src="https://user-images.githubusercontent.com/101574457/222471976-e80f1a40-14e4-4cc1-b715-c54e87d905b0.png">

เพิ่ม export PATH="$PATH:[PATH ของตัว Flutter GIT Directory]/bin" เข้าไปใน .zshrc ( ในกรณีนี้เราจะใช้ export PATH="$PATH:/Users/mercuone/development/flutter/bin"
 ที่เป็นที่เก็บไฟล์ของเรา )
<img width="417" alt="image" src="https://user-images.githubusercontent.com/101574457/222473481-dda587fa-a407-455a-836f-fd2b96270952.png">

จากนั้น source $HOME/.<rc file> และ พิม flutter เพื่อใช้งาน
<img width="500" alt="image" src="https://user-images.githubusercontent.com/101574457/222474073-6b260aef-7f16-4aa7-9736-b8cfbbdf6a35.png">                                            
<img width="582" alt="image" src="https://user-images.githubusercontent.com/101574457/222474404-6c6d27ef-6544-40c0-b043-85c659308162.png">

รันคำสั่ง Flutter doctor                                                                                              
ซึ่ง Flutter doctor เป็นเครื่องมือใน Flutter SDK ช่วยตรวจสอบสถานะของเครื่องและแสดงข้อความแนะนำสำหรับการตั้งค่าเพื่อให้สามารถพัฒนาแอปพลิเคชัน Flutter ได้อย่างถูกต้อง ช่วยในการตรวจสอบว่าคุณมี Flutter SDK, Android SDK, iOS SDK, และ Android Studio ที่จำเป็นสำหรับการพัฒนาแอปพลิเคชัน Flutter หรือไม่
<img width="490" alt="image" src="https://user-images.githubusercontent.com/101574457/222474840-1d594003-eb54-449a-9a49-4ff8311877f0.png">

## iOS setup
### Install Xcode
  
ติดตั้ง Xcode application                                                                                                                                                   
  <img width="934" alt="image" src="https://user-images.githubusercontent.com/101574457/222478939-ac80d04a-ee5d-4130-98b3-f62cf9a30b67.png">

รันคำสั่ง "sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer" และ "sudo xcodebuild -runFirstLaunch" ใน Terminal Flutter 
<img width="572" alt="image" src="https://user-images.githubusercontent.com/101574457/222482429-c1789f1c-1823-40ba-9355-19de9e6238c3.png">

เมื่อรัน flutter doctor อีกรอบ  ก็จะพบว่า Xcode ขึ้นสีเหลือยังขาด CocoaPods ให้ไปดูที่ Deploy to IOS devices                                                                                                                                
<img width="560" alt="image" src="https://user-images.githubusercontent.com/101574457/222485237-a5caae71-c3af-45c1-bc17-431f851945e5.png">

### Set up the iOS simulator
รันคำสั่ง open -a Simulator เพื่อเปิดตัว Simulator                                                                                            
  <img width="382" alt="image" src="https://user-images.githubusercontent.com/101574457/222483451-36eecae5-9411-48b6-9c96-217e76272304.png">

### Deploy to iOS devices
รันคำสั่ง sudo gem install cocoapods                                                                                                              
<img width="1443" alt="image" src="https://user-images.githubusercontent.com/101574457/222485035-a5f806e1-3652-4a23-9532-0d5a4c37c823.png">

### ทดลองสร้าง project
 ใช้คำสั่ง flutter create my_app สร้าง floder my_app ขึ้นมาและเก็บ flutter framework
<img width="550" alt="image" src="https://user-images.githubusercontent.com/101574457/222489227-79df6e5b-8e54-4b87-872b-371bdde60ee1.png">

 cd my_app เพื่อไปที่ floder my_app และทำการ flutter run                                                                
<img width="425" alt="image" src="https://user-images.githubusercontent.com/101574457/222491434-5d4e5272-b13f-46fb-bdf8-d39a58f85177.png">            
  <img width="798" alt="image" src="https://user-images.githubusercontent.com/101574457/222491698-45f7f80b-580d-4acb-89a8-971bfefe6877.png">


