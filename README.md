Mustangs Down
====

<p align="center">
  <img src="files/Header NewMustang (3).gif" alt="Demo animation">
</p>


This repository contains the documentation for the Mustangs Down team's robot for the 2025 World Robot Olympiad Future Engineers category competition. The robot was designed and built by a team of three.

Table of contents
----

- [The Team](#the-team)
- [Photos of the robot](photos-of-the-robot)

## The team
======

Mark Chen, Age: 16

![image](https://github.com/user-attachments/assets/263bca30-1d4f-4f59-a675-890829c32520)

School: Panamerican School of Panama, PAS

Hi!, I'm Mark from Panama with Chinese origin born in February 8 2009. I've been participating in WRO since 2022 and this is my second year participating in the Future Engineers category. I enjoy playing piano and I am a part of a school band, other hobbies include cubing (Rubik's cube competitions), gaming, drawing and writing.

----

Juan Pablo Gomez, Age: 16

![image](https://github.com/user-attachments/assets/b9244ac9-54e1-4af8-89d1-042ac478571a)

School: Panamerican School of Panama, PAS

Hi, I'm Juan Pablo, from Colombia. I love robotics. I've been working with robots since I was 8 years old. My main hobbies are playing bass, hanging out with friends, playing video games, driving karts, and participating in various sports such as football and volleyball.

----

Julio Chong, Age: 16

![image](https://github.com/user-attachments/assets/39dfb391-f71d-4759-b822-fce67cd3f061)

School: Panamerican School of Panama, PAS

My name is Julio Chong, a panamenian teen with chinese antescedents who was born in August 24, 2008. I've been into robotics since 9th grade on 2023. My hobbies are playing the guitar, cooking, coding, learning new languages and also doing lots of exercise or sport, especially contact sports such as jiujitsu.

----

Victor Sanchez (Coach), Age: 35

![image](https://github.com/user-attachments/assets/98a81bb6-1889-4778-b462-37a8654daace)

School: Panamerican School of Panama, PAS

lorem ipsum

----

Team photo

(inset picture)

The competition
====

Unlike the structured missions of other WRO categories, Future Engineers presents a broad problem (often related to autonomous vehicles, smart systems, or complex automation), and teams must engineer a full solution. Teams work within defined technical limits (size, cost, sensors, etc.) that mimic real-life engineering conditions. This challenge has two main tasks, the first round which tests the robot's progamming of being able to drive many laps without crashing. The second round adds obstacles that the robot must avoid crashing into and a parking space where the robot should finish.

This challenge emphasizes all aspects of the engineering process, including:

- Mobility: Developing efficient vehicle movement.

- Obstacle managing: Detecting and dodging the different obstacles (Green and Red blocks) with effiency.

- Documentation: Showcasing engineering progress, design planning, and collaboration though a GitHub repository.

Points are awarded based on the performance of the robot. In the first round, points are awarded if the robot does not crash or stop during the round. In the second round, points are awarded for every obstacle the robot is able to detect and avoid, bonus points are rewarded if the robot can succesfully finish in the designated parking space.

## Photos of the robot
====

| Top | Bottom |
|--------|---------|
| ![WhatsApp Image 2025-06-30 at 15 49 33_9f3bbfec](https://github.com/user-attachments/assets/43aaa545-8b6f-4e37-bc9e-2e6eea242892) |![WhatsApp Image 2025-06-30 at 15 49 33_6a293fe1](https://github.com/user-attachments/assets/cedce72b-bcb6-45e5-8ab6-52f743984c7b) |

| Left | Right |
|--------|---------|
| ![WhatsApp Image 2025-06-30 at 15 49 33_56ea4051](https://github.com/user-attachments/assets/e097a6ab-d837-4754-b5e6-7f1f7045d6de)|![WhatsApp Image 2025-06-30 at 15 49 33_4cf76fe9](https://github.com/user-attachments/assets/52f4f881-262d-4f04-9244-fb63604a4117) |

| Front | Back |
|--------|---------|
|![WhatsApp Image 2025-06-30 at 15 49 33_d7e21712](https://github.com/user-attachments/assets/a18d05f4-239c-4867-8839-75a2133e14b0)|![WhatsApp Image 2025-06-30 at 15 49 33_67d5e010](https://github.com/user-attachments/assets/7c809ffd-461f-4f71-b14a-5659f50b11cb)
|

Motors, sensors and systems
====
The robot operates with multiple motors and sensors which will be showcased here.

Movement
----
The robot uses motors for drving and steering, these components work together to ensure the robot has a smooth and efficient movement.

![image](https://github.com/user-attachments/assets/fbd40ed2-1a61-49ba-8580-67152f42db4c) 

|  Voltage |   Current  |   rpm    |  Torque  |
|----------|------------|----------|----------|
|    3     |    160     |   120    |   0.45   |
|    6     |    220     |   200    |    1.0   |
|   7.2    |    250     |   250    |    1.5   |

We chose this motor because it was viable and the one we had already, other motors we used didn't hold up or didn't have enough power to move the wheels. Although there are way better motors we could've bought, we chose this one for its dual motor and it didn't need a driving axle. This made the building process a bit easier and less complicated.

To connect the motor to the skeleton, we made an opening in the skeleton to fit the motor inside, then we held it up with a bent metal sheet and some screws.

![image](https://github.com/user-attachments/assets/bd00b6b5-922a-49a0-bb43-03d6022214f9)

The design could be perfected if the skeleton was made to skale with the motor or we had chosen a different motor that not only satisfies what the robot needs but also that it fits confortably to the skeleton.

Steering
----
We experimented with many steering mechanisms but the one we found most success was anti-Ackerman steering. Other methods where either too big and complex or didn't turn the right amount. Anti-Ackerman systems are usually used on racing cars where the vehicles must turn at high speeds and the tires might slip, the outer tire’s increased steering angle helps compensate for these slip angles, maximizing grip during high-speed cornering. Even though with this robot we can't reach those speeds where the wheels start slipping, the anti-Ackerman system is still the most effective and simple for this competition.

The steering system is composed of two identicar wheel holders connected with two steering axels, these two axels are then connected to the servo motor in the middle.

![image](https://github.com/user-attachments/assets/c8e9e390-33da-499f-b02f-5bd69cfb3fcb)

Servo motor:
----

![image](https://github.com/user-attachments/assets/c1188e64-4b96-4dbb-88fa-45dc8717d740) 

|  Voltage |   Temperature   |   Angle of Rotation    |    Torque    |  Control signal  |  Type of Servo  |
|----------|-----------------|------------------------|--------------|------------------|-----------------|
|  3.3V~5V |   -30°C~+60°C   |          180           |   1.6KG/cm   |    PWM signal    |  Digital servo  |

For the motor we used the Steren servo motor, it's an okay motor but we chose it because it was the one we had in hand. Although it is a cheap motor, it works perfectly with the design of the robot.

Motherboard
----

![image](https://github.com/user-attachments/assets/badc365a-1382-4089-88d6-2129cc35cae7)

|     Chip     |   Clock   |   ROM   |  SRAM  |  FLASH  |        Interfaces        |  Input voltages  |
|--------------|-----------|---------|--------|---------|--------------------------|------------------|
| ESP-WROOM-32 |   240MHz  |  448KB  |  520KB |   4MB   |  UART , I2C , SPI , CAN  |      6-18V       |

For motor driver, we chose the Acebott ESP32, it's capable of controling not only the motors but the sensors as well.

Skeleton/Chassis
----

This year, instead of making the chassis out of lego, we changed it to 3D printed since it allowed it to be less bulky and lighter unlike the lego version. 

![image](https://github.com/user-attachments/assets/9f6c9e10-1ba4-45d7-8874-0108a5bd213f)

Energy management
----
Battery:
----
![image](https://github.com/user-attachments/assets/71818d84-c5d1-4629-8518-718c7c04b7c8)

Model 18605

3.7 V

Sensors
----

For the robot we used the OpenMV Cam RT62 which allowed the robot to detect walls and the colored blocks more easily. It's a small, low power, microcontroller board which allows you to easily implement applications using machine vision in the real-world. It is a huge improvement from last year's robot since we didn't have access to these type of sensors/camera.

![image](https://github.com/user-attachments/assets/b646f95c-ab16-4efc-8822-66b5377803ac)

Dimentions:

-Length: 45 mm

-Width: 36 mm

-Height: 29 mm

|  Microcontroler |   Flash memory   |  RAM   |    Frequency    |  Resolution  |  FPS  | Weight |
|-----------|------------|----------------|--------------|------------------|-------|-------|
|  ISSI2232  |   32MB   |      512KB       |   600 MHz   |    2592 x 1944    |  40  | 20g |

Multiplexer
----

![image](https://github.com/user-attachments/assets/c48e9adc-9b48-41bf-b452-00561f16c633)


For a multiplexer we chose the TCA9548A I2C multiplexer, which allows you to communicate with up to 8 I2C devices with the same I2C bus.

Main features:

-1 to 8 bidireccional translating switches

-Active-low reset input

-Three address pins—up to 8 TCA9548A devices on the same I2C bus

-Channel selection through an I2C bus

-Operating power supply voltage range: 1.65V to 5.5V

-5V tolerant pins


Circuit diagram
----

![electric diagram WRO (1)](https://github.com/user-attachments/assets/a96c6d7c-2828-4230-81ea-050892f3166e)


Pins used:

![electric diagram WRO (2)](https://github.com/user-attachments/assets/95201ec8-1249-4721-9a51-392f6b8be53a)



Program and source code
----

For programing the robot, we used both Python and Arduino coding languages. Python because the program for the camera required Python usage and it allowed us to have more precise movements, we used Arduino because we wanted to use a ESP32 motor driver which was more viable and more precise than other models.

Code for each component
----

Drive
----

For driving, the code works by constantly making the car move forward and stopping once all three laps of the track are completed.

```python

void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);  // Encender PWM a tope
}

void StopMotor() {
  digitalWrite(PWM1_PIN, LOW);  // Apagar PWM
}
```
Additionaly, a part of the code specifies the maximum amount of time that the code can run.

```python

// Control de tiempo
#define TIEMPO_LIMITE_MS 67000  // 1 minuto, 7 segundos
unsigned long tiempoInicio;
bool detenido = false;
```

Servo motor
----

The servo motor is supported by the distance sensors in both right and left sides of the robot, the servo moves accordingly wether the sensors detect a wall on the left or right, additionaly, at the end it stops for a certain amount of time so the robot does not perform more than 3 laps.

```python

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);

  // Sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(500);
  if (!sensorLeft.init()) {
    Serial.println("Error: sensor izquierdo no detectado.");
    while (1);
  }
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(20000);
  sensorLeft.startContinuous(20);

  // Sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(500);
  if (!sensorRight.init()) {
    Serial.println("Error: sensor derecho no detectado.");
    while (1);
  }
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(50000);
  sensorRight.startContinuous(50);

  Serial.println("Sistema listo.");

  // Tiempo inicial
  tiempoInicio = millis();
}

void loop() {
  // Verificar si se superó el tiempo límite
  if (!detenido && millis() - tiempoInicio >= TIEMPO_LIMITE_MS) {
    Serial.println("Tiempo límite alcanzado. Deteniendo todo.");
    StopMotor();
    miServo.write(SERVO_CENTER);

```

The sensors detect the distance from the wall to the robot and responds accordingly, the servo motor will activate if the robot is 80cm or closer to the wall.

```python

  // Leer sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  int distLeft = sensorLeft.read();
  if (sensorLeft.timeoutOccurred()) {
    Serial.println("Timeout sensor izquierdo");
    distLeft = 0;
  }

  // Leer sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  int distRight = sensorRight.read();
  if (sensorRight.timeoutOccurred()) {
    Serial.println("Timeout sensor derecho");
    distRight = 0;
  }

  Serial.print("Izquierdo: "); Serial.print(distLeft);
  Serial.print(" mm | Derecho: "); Serial.println(distRight);

  // Reacción del servo con prioridad
  if (distLeft > OBSTACLE_THRESHOLD) {
    Serial.println("Distancia izquierda > 80 cm → girar a la izquierda");

  StopMotor();  // Prioriza el servo
    delay(100);
    miServo.write(SERVO_LEFT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(200);
    MoveForward();  // Reanuda motor
  } 
  else if (distRight > OBSTACLE_THRESHOLD) {
    Serial.println("Distancia derecha > 80 cm → girar a la derecha");

```

Obstacle round
----

For the obstacle round, the camera was the main component. It is capable of detecting colors and objects from a distance and act accordingly, the distance sensors also play the same role and are still in use for this round. 

The camera detects the green and red blocks and the robot then knows where to turn and when, then it checks the distance sensors to see if it has space or the need to turn, the rest of the code is mostly the same with some slight modifications so the camera could work. 

```python

void loop() {
  // UART desde cámara: color detectado
  if (Serial1.available() && !enGiroPorColor) {
    String color = Serial1.readStringUntil('\n');
    color.trim();

    if (color == "ROJO") {
      Serial.println("Color ROJO detectado → giro a la derecha");
      ejecutarGiroColor(SERVO_RIGHT, SERVO_LEFT);
    }
    else if (color == "VERDE") {
      Serial.println("Color VERDE detectado → giro a la izquierda");
      ejecutarGiroColor(SERVO_LEFT, SERVO_RIGHT);
    }
  }

  MoveForward();  // Siempre avanza a media velocidad

  // Lectura sensores de distancia
  selectOnlyOneMux(MUX_LEFT_ADDR);
  int distLeft = sensorLeft.read();
  if (sensorLeft.timeoutOccurred()) {
    Serial.println("Timeout sensor izquierdo");
    distLeft = 0;
  }

  selectOnlyOneMux(MUX_RIGHT_ADDR);
  int distRight = sensorRight.read();
  if (sensorRight.timeoutOccurred()) {
    Serial.println("Timeout sensor derecho");
    distRight = 0;
  }

```

This last part is to ensure the robot does not crash into any wall or block after turning or overturning. It also checks with the distance sensors one more time so it does not misalign from the track's path.

```python

  Serial.print("Izquierdo: "); Serial.print(distLeft);
  Serial.print(" mm | Derecho: "); Serial.println(distRight);

  if (!enGiroPorColor) {
    if (distLeft > OBSTACLE_THRESHOLD) {
      Serial.println("Distancia izquierda > 100 cm → giro a la izquierda");
      StopMotor();
      delay(100);
      miServo.write(SERVO_LEFT);
      delay(2800);
      miServo.write(SERVO_CENTER);
      delay(200);
      MoveForward();
    } else if (distRight > OBSTACLE_THRESHOLD) {
      Serial.println("Distancia derecha > 100 cm → giro a la derecha");
      StopMotor();
      delay(100);
      miServo.write(SERVO_RIGHT);
      delay(2800);
      miServo.write(SERVO_CENTER);
      delay(200);
      MoveForward();
    }
  }

  delay(100);
}
```

Camera
----

The camera is programmed to detect the red and green colors, the camera has other functions but for the sake of simplicity we only used in to detect colors. The camera was programmed with Arduino

```arduino

from machine import UART
import sensor
import image
import time

UART a ESP32 (TX en P4)
uart = UART(1, baudrate=115200)

Configuración de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)
sensor.set_framesize(sensor.HD720)
sensor.skip_frames(time=2000)
sensor.set_auto_gain(False)
sensor.set_auto_whitebal(False)

Umbrales
red_threshold = (30, 100, 15, 127, 15, 127)
green_threshold = (30, 100, -127, -15, 15, 127)

clock = time.clock()

while True:
    clock.tick()
    img = sensor.snapshot()

    # Detectar rojo (máximo 1)
    rojos = img.find_blobs([red_threshold], pixels_threshold=200, area_threshold=200, merge=True)
    verdes = img.find_blobs([green_threshold], pixels_threshold=200, area_threshold=200, merge=True)

    if len(rojos) > 0:
        blob = rojos[0]
        img.draw_rectangle(blob.rect(), color=(255, 0, 0))
        img.draw_cross(blob.cx(), blob.cy(), color=(255, 0, 0))
        uart.write("ROJO\n")
        print("ROJO")
    elif len(verdes) > 0:
        blob = verdes[0]
        img.draw_rectangle(blob.rect(), color=(0, 255, 0))
        img.draw_cross(blob.cx(), blob.cy(), color=(0, 255, 0))
        uart.write("VERDE\n")
        print("VERDE")

    time.sleep_ms(300)  # Da tiempo al ESP32 a leer sin saturarse

```

