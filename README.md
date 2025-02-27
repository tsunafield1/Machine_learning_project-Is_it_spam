# Is it spam?
โปรเจคนี้มีชื่อว่า "Is it spam?" หรือ "อีเมลนี้เป็นสแปมหรือไม่?" ทำขึ้นเพื่อตรวจสอบว่าอีเมลนั้นๆ เป็นสแปมหรือไม่
โดยในโปรเจคนี้ จะใช้ภาษา Python ในการวิเคราะห์ และประมวลผล
มีการใช้ dataset จาก kaggle 2 ชุด แบ่งเป็น train-test dataset และ validate dataset 
และใช้ model จาก sklearn 2 ตัว คือ MLPClassifier และ RandomForestClassifier

สามารถทดลองใช้งานได้ใน Demo/IsItSpam.py โดยจะใช้ tkinter ในการแสดง GUI

![alt text](https://github.com/tsunafield1/Is_it_spam/blob/main/Example.PNG?raw=true)

------------------------------------------------

ใน Source จะมี 4 ไฟล์
- Create_test_dataset.ipynb คือ ไฟล์ที่จะทำการแปลง validate dataset ให้อยู่ในรูปแบบเดียวกับ train-test dataset
- Dataset Reference.txt คือ ที่มาของ dataset เนื่องจากไฟล์มีขนาดใหญ่เกินไปที่อัพโหลด จึงให้เป็นที่มาแทน
- IsItSpamMLP.ipynb คือ ไฟล์ที่ใช้ MLPClassifier ซึ่งจะมีการใช้ joblib เพื่อบันทึกสิ่งที่ต้องการไว้
- IsItSpamRF.ipynb คือ ไฟล์ที่ใช้ RandomForestClassifier

ใน Demo จะมี 6 ไฟล์
- COL.sav คือ ไฟล์ที่บันทึกชื่อ column ของ dataset ไว้ โดยใช้ joblib ในการโหลด
- Demo_Ans.xlsx คือ ไฟล์ excel ที่บันทึกตัวอย่างอีเมลพร้อมคำตอบไว้ (ใช้เพื่อนำเสนอ)
- Demo_emails.xlsx คือ ไฟล์ excel ที่บันทึกตัวอย่างอีเมลไว้ (ใช้เพื่อนำเสนอ)
- IsItSpam.py คือ ไฟล์ที่รันเพื่อทดลองใช้งานโปรเจค
- MLP.sav คือ ไฟล์ที่บันทึก model ที่พร้อมใช้งานไว้ โดยใช้ joblib ในการโหลด
- STD.sav คือ ไฟล์ที่บันทึก StandardScaler ที่พร้อมใช้งานไว้ โดยใช้ joblib ในการโหลด

Medium Draft: https://medium.com/@GlitR/1c856196bd43

โปรเจคนี้เป็นส่วนหนึ่งของวิชา Machine learning ภาควิชาวิศวกรรมคอมพิวเตอร์ คณะวิศวกรรมศาสตร์ สถาบันเทคโนโลยีพระจอมเกล้าเจ้าคุณทหารลาดกระบัง
