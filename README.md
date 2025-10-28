# Github_command
Just command 
----------------------------------------------------------
+++ Version Control for Software Project +++
----------------------------------------------------------
On local (GitLocal) by Git-SCM
1. ทำแค่ครั้งแรกครั้งเดียวต่อโปรเจ็กต์หนึ่งๆ หรือโฟล์เดอร์หลักหนึ่งๆ
- git  init
- git  config  --global  user.email  "xxxxxxxxxxxxx@gmail.com"
- git  config  --global  user.name  "xxxxxxxxxxxxx"
2. ทำทุกครั้งที่จะทำ Version Control บน On local
- git  add  .
- git  commit  -m  "พิมพ์ข้อความกำกับการทำ Commit/Version/Backup"
-----------------------------------------------------------------------------
On cloud (GitServer/GitService) by GitHub 
- ที่ GitHub สร้าง new -> repository โดยตั้งชื่อเดียวกับชื่อโปรเจ็กต์
1. ทำแค่ครั้งแรกครั้งเดียวต่อโปรเจ็กต์หนึ่งๆ หรือโฟล์เดอร์หลักหนึ่งๆ
- git branch -M main
- git remote add origin https://github.com/Maninfinity13/xxxxxxxxxxxxx.git
2. ทำทุกครั้งที่จะ Upload ขึ้น GitHub
- git push -u origin main
----------------------------------------------
คำสั่ง git ที่น่าสนใจ
- git config --global --list ตรวจสอบ user.email, user.name
- git log ตรวจสอบว่าทำ commit ไปกี่ครั้งแล้ว (กรณีเห็นไม่หมดให้กด Enter กรณีต้องการออกจาก git log กด q)
- git status ตรวจสอบสถานะของการทำ version ณ ปัจจุบัน
- git remote -v ตรวจสอบ ตำแหน่งของ remote ณ โปรเจ็กต์ปัจจุบัน
- git remote set-url origin https://github.com/Maninifinity13/xxxxxxxxxxxxx.git
 ----------------------------------------------------------
คำสั่ง Command Line พื้นฐานที่ใช้กับ Command Prompt หรือ Terminal
- cls     ล้างหน้าจอ
- cd \     จะไปที่ไดร์ฟต้นทาง เช่น ไดร์ฟ C:\> หรือ ไดร์ฟ D:\>
- cd folder_name  เข้าไปที่โฟล์เดอร์
- dir    ดูโฟล์เดอร์และไฟล์ในไดเรกทอรี่/โฟล์เดอร์ขณะนั้น
--------------------------------------------------
คำสั่ง pull/fetch/merge
git pull <remote> <branch>
git merge <branch>
<!-- example: git checkout main
git merge feature-login -->
-------------------------------------------
git pull origin main          # ดึงการเปลี่ยนแปลงล่าสุดจาก remote main

git checkout feature-login    # สลับไปทำงานบน branch ของ feature
git add .                     # stage การเปลี่ยนแปลง
git commit -m "เพิ่มระบบ login"
git checkout main             # กลับไป main
git merge feature-login       # รวม feature-login เข้ากับ main
git push origin main          # อัปโหลด main กลับไป remote
 
