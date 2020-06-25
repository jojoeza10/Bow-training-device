# Bow aiming stance training  device
คือ อุปกรณ์ที่ช่วยฝึกนักธนูให้สามารถตั้งท่าพื้นฐานได้อย่างถูกต้อง ผู้ใช้สามารถทราบองศาการเล็งคันธนูของตัวเองเมื่อเทียบกับพื้น เมื่อผู้ใช้ตั้งท่าอยู่ในจุดที่ถูกต้อง(ขนานกับพื้นราบ)จะมีเสียงดังขึ้นและเมื่อผู้ใช้มีองศาการเล็งอยู่ระหว่าง 0 องศาถึง 45 องศาจะมีแสงเลเซอร์สว่างขึ้น

## ที่มาและความสำคัญ
ในปัจจุบันการยิงธนูนั้นเป็นเกม,กีฬา,การล่าสัตว์รวมไปถึงเป็นของเล่นสำหรับเด็ก แต่การจะฝึกการยิงธนูให้มีความชำนาญหรือความแม่นยำนั้นย่อมเกิดจากการตั้งท่าที่ถูกต้อง การฝึกท่าถือคันธนูแบบไม่ใช้ศูนย์นั้น ผู้ใช้จะต้องตั้งท่าให้แขนตั้งฉากกับลำตัวอยู่ตลอดเวลาจึงได้เกิดเป็นโปรเจคนี้ขึ้นเพื่อสร้างอุปกรณ์ที่สามารถให้ข้อมูลกับผู้ใช้ว่า ขณะนี้ผู้ใช้เล็งคันธนูอยู่ในมุมที่ถูกต้องแล้วหรือไม่

## กลุ่มเป้าหมาย
+ นักธนูที่ต้องการฝึกฝนท่าการเล็งแบบไม่ใช้ศูนย์ 
+ อุปกรณ์อื่นๆที่ต้องการฝึกทักษะการเล็ง เช่น ปืน

## รายละเอียดโปรเจค

### Perception Module
- 3-Axis Gyroscope & 3-Axis Accelerometer

### Behavior
1. อ่านค่าแกนx,y,zและองศาแกนx,y,z
2. ถ้าค่าองศาอยู่ระหว่าง0-45องศา Red dot laserจะเปล่งแสง
3. แสดงค่าองศาผ่าน 7 Segment
4. ถ้าผู้ใช้เล็งองศาไปที่ 0 Active Buzzerจะส่งเสียง

### Manipulation Module
- Red dot Laser
- Active Buzzer 
- I2C 4 Digit 7-Segment Display

### โครงสร้างพื้นฐาน
![diagram picture][diagram]

[diagram]: https://github.com/jojoeza10/Bow-training-device/blob/master/image/diagram.jpg "Diagram"

### ระบบการทำงาน 
![flowchart picture][flowchart]

[flowchart]: https://github.com/jojoeza10/Bow-training-device/blob/master/image/Flowchart.jpg "flowchart"

