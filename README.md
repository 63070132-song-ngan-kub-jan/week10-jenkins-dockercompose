# อันนี้เป็น Video นำเสนอครับ [>>คลิกที่นี่<<](https://drive.google.com/file/d/1HUva4ZxQFUBvFcn0CEsF32PRINw_eSVi/view?usp=sharing)

ผมใช้ Jenkins ในการรับ hook จาก GitHub เมื่อมีการ commit จากนั้นทำการ สร้าง Docker image โดยใช้ Docker Compose แล้วจึง push ขึ้น DockerHub เมื่อเสร็จได้มีการเรียกตัว slave job เพื่อ pull images จาก DockerHub เมื่อสักครู่ จากนั้นจึงทำการ run containers

โดยที่ไฟล์ `Jenkinsfile-master` เป็น job สร้าง image และ push ขึ้น DockerHub
และไฟล์ `Jenkinsfile-slave` เป็น job ที่ pull image จาก DockerHub และ run container

frontend ใช้เป็น Vue.js ครับ ใส่รูปแล้วประมวลผลจาก backend ได้
```sh
npm install
npm run dev
```
เปิดที่ port 8081 ได้เลยครับ

backend เป็น FastAPI ตามโค้ดของอาจารย์เลยครับ
```sh
pip install -r requirements.txt
uvicorn main:app --host 0.0.0.0 --port 8082
```

<br><br>

<img width="100%" src="https://media.tenor.com/D11n3-s_HakAAAAC/woody-toy-story.gif" />
