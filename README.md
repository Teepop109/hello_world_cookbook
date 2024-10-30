## ESP32-hello-world - `hello_world`
ESP32-hello-world เป็นตัวอย่างพื้นฐานที่ใช้ไมโครคอนโทรลเลอร์ ESP32 เพื่อทำความเข้าใจพื้นฐานของการพัฒนาและการเขียนโปรแกรมด้วย ESP32 โครงการนี้มักจะเน้นการสื่อสารพื้นฐาน เช่น การแสดงข้อความใน Serial Monitor เป็นต้น
## ขั้นตอนการใช้งาน
1. เริ่มต้นโดยการเลือกตัวอย่าง `hello_world`
# ![Screenshot 2024-10-30 215803](https://github.com/user-attachments/assets/f838d0cc-f0a4-4743-af1b-b4194f0a8b73)
# ![Screenshot 2024-10-30 215812](https://github.com/user-attachments/assets/b905d39e-b4cc-429d-9cac-5cbe809b4753)

2. หลังจากเลือกตัวอย่างแล้ว ให้กดปุ่ม **Create**
# ![Screenshot 2024-10-30 215817](https://github.com/user-attachments/assets/ec1d1641-afc3-4e16-821e-b24bbcc5f7c6)

3. ตรวจสอบโค้ดในไฟล์ ` hello_world_main.c` สามารถแก้ไขเพื่อให้แสดงผลข้อความต่างๆ นอกเหนือจาก hello world และให้โชว์ ข้อมูลต่างๆ ของ ESP32
# ![Screenshot 2024-10-30 215919](https://github.com/user-attachments/assets/c80c3f4a-85d2-4b4f-82ef-114778939c63)
# ![Screenshot 2024-10-30 215930](https://github.com/user-attachments/assets/b78cbe63-6be0-4fb3-8b6b-5c6e7e26aa62)

ผลการทำงานจะเเสดงคำว่า Hello world! จากนั้นนับถอยหลัง restart การทำงาน

กด Build และรันโปรแกรม จากนั้นเลือก **UART** ผลการทำงานจะเป็นดังนี้
# ![Screenshot 2024-10-30 220206](https://github.com/user-attachments/assets/0c0e5af3-ce8c-4bc9-a31e-e138908ca943)

# การเเก้ไข
เมื่อแก้ไขโค้ดใน main/hello_world_main.c ให้แสดงผล Hi My name is Teepop พร้อมสูตรคูณ แม่ 25 จากนั้นนับถอยหลัง restart การทำงาน
# ![Screenshot 2024-10-30 220738](https://github.com/user-attachments/assets/7e19265f-3cb7-4d87-8cf6-87482c36484f)

```
printf("Hello world!\n");
    printf("Hi My name is Teepop\n"); 

    for (int i = 1; i <= 12; i++) {
        printf("25 x %d = %d\n", i, i * 25);
    }
```

หลังจากนั้น build flash เพื่อดูผลการทำงาน
# ผลการรันตัวอย่างการเเก้ไข ดังนี้
# ![Screenshot 2024-10-30 220717](https://github.com/user-attachments/assets/51dd6679-b55b-4e31-9bf0-32a90835adfc)

### สรุปการทดลอง
การทดลอง Hello World Example บน ESP32 เป็นขั้นพื้นฐานที่ช่วยให้เราเข้าใจการเชื่อมต่อและการเขียนโค้ดเบื้องต้นบนบอร์ด ESP32 ได้ดี เมื่ออัปโหลดโค้ดสำเร็จ และเปิด Serial Monitor จะเห็นข้อความ "Hello, World!" ถูกพิมพ์ออกมาตามที่ตั้งไว้ในโปรแกรม ซึ่งแสดงว่าการเชื่อมต่อและการอัปโหลดโค้ดทำงานได้อย่างถูกต้อง ถ้ามีความต้องการจะเปลี่ยนแปลงข้อความหรือแก้ไขระยะเวลาในการ restart ก็สามารถที่จะปรับเปลี่ยนได้ตามความต้องการดังตัวอย่างที่มีการเเก้ไขให้ให้แสดงผล Hi My name is Teepop พร้อมสูตรคูณ แม่ 25 จากนั้นนับถอยหลัง restart การทำงาน
