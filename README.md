Mustangs Down
====

<p align="center">
  <img src="files/Header NewMustang (3).gif" alt="Demo animation">
</p>


This repository contains the documentation for the Mustangs Down team's robot for the 2025 World Robot Olympiad Future Engineers category competition. The robot was designed and built by a team of three.

Table of contents
----

- [The Team](#the-team)
- [The Competition](#the-competition)
- [Photos of the robot](#photos-of-the-robot)
  - [Video](#video)
- [Motors, sensors and systems](#motors-sensors-and-systems)
  - [Movement](#movement)
- [Steering](#steering)
  - [Servo Motor](#servo-motor)
- [Motherboard](#motherboard)
- [Skeleton/Chassis](#skeleton/chassis)
- [Energy Management](#energy-management)
  - [Battery](#battery)
- [Sensors](#sensors)
  - [Multiplexer](#multiplexer)
- [Circuit Diagram](#circuit-diagram)
- [Program and Source Code](#program-and-source-code)
  - [Drive](#drive)
  - [Open Round](#open-round)
  - [Obstacle Round](#obstacle-round)
  - [Camera](#camera)

    
## The team
----

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

Hello, I'm Victor Sanchez, robotics profesor with experience in educational programming with LEGO SPIKE in Panamerican School, I've led the robotics scholar proyect for 4 years with the goal of becoming national champion in Panama and solid at an international scale. I enjoy woodworking and playing videogames.

----

Team photo

(inset picture)

[Back to table of contents](#table-of-contents)

The competition
----

Unlike the structured missions of other WRO categories, Future Engineers presents a broad problem (often related to autonomous vehicles, smart systems, or complex automation), and teams must engineer a full solution. Teams work within defined technical limits (size, cost, sensors, etc.) that mimic real-life engineering conditions. This challenge has two main tasks, the first round which tests the robot's progamming of being able to drive many laps without crashing. The second round adds obstacles that the robot must avoid crashing into and a parking space where the robot should finish.

This challenge emphasizes all aspects of the engineering process, including:

- Mobility: Developing efficient vehicle movement.

- Obstacle managing: Detecting and dodging the different obstacles (Green and Red blocks) with effiency.

- Documentation: Showcasing engineering progress, design planning, and collaboration though a GitHub repository.

Points are awarded based on the performance of the robot. In the first round, points are awarded if the robot does not crash or stop during the round. In the second round, points are awarded for every obstacle the robot is able to detect and avoid, bonus points are rewarded if the robot can succesfully finish in the designated parking space.

[Back to table of contents](#table-of-contents)

## Photos of the robot
----

| Top | Bottom |
|--------|---------|
| ![WhatsApp Image 2025-06-30 at 15 49 33_9f3bbfec](https://github.com/user-attachments/assets/43aaa545-8b6f-4e37-bc9e-2e6eea242892) |![WhatsApp Image 2025-06-30 at 15 49 33_6a293fe1](https://github.com/user-attachments/assets/cedce72b-bcb6-45e5-8ab6-52f743984c7b) |

| Left | Right |
|--------|---------|
| ![WhatsApp Image 2025-06-30 at 15 49 33_56ea4051](https://github.com/user-attachments/assets/e097a6ab-d837-4754-b5e6-7f1f7045d6de)|![WhatsApp Image 2025-06-30 at 15 49 33_4cf76fe9](https://github.com/user-attachments/assets/52f4f881-262d-4f04-9244-fb63604a4117) |

| Front | Back |
|--------|---------|
|![WhatsApp Image 2025-06-30 at 15 49 33_d7e21712](https://github.com/user-attachments/assets/a18d05f4-239c-4867-8839-75a2133e14b0)|![WhatsApp Image 2025-06-30 at 15 49 33_67d5e010](https://github.com/user-attachments/assets/7c809ffd-461f-4f71-b14a-5659f50b11cb)


## Video
---

Video of the robot on Youtube: [Video](https://youtu.be/vqMiVIuP070)

[Back to table of contents](#table-of-contents)

## Motors, sensors and systems
----

The robot operates with multiple motors and sensors which will be showcased here.

## Movement
----
The robot uses motors for drving and steering, these components work together to ensure the robot has a smooth and efficient movement.

![image](https://github.com/user-attachments/assets/fbd40ed2-1a61-49ba-8580-67152f42db4c) 

|  Voltage |   Current  |   rpm    |  Torque  |
|----------|------------|----------|----------|
|    3     |    160     |   120    |   0.45   |
|    6     |    220     |   200    |    1.0   |
|   7.2    |    250     |   250    |    1.5   |

We chose this motor because it was viable and the one we had already, other motors we used didn't hold up or didn't have enough power to move the wheels. Although there are way better motors we could've bought, we chose this one for its dual motor and it didn't need a driving axle. This made the building process a bit easier and less complicated.

The motor works by converting electrical energy into mechanical energy, specifically rotational motion, through the interaction of magnetic fields. It uses the principle that a current-carrying conductor experiences a force within a magnetic field. This force causes a rotor to spin, which then drives a shaft, producing mechanical work. This is then connected to the wheels with two jammed axles.

To connect the motor to the skeleton, we made an opening in the skeleton to fit the motor inside, then we held it up with a bent metal sheet and some screws.

![image](https://github.com/user-attachments/assets/bd00b6b5-922a-49a0-bb43-03d6022214f9)

The design could be perfected if the skeleton was made to skale with the motor or we had chosen a different motor that not only satisfies what the robot needs but also that it fits confortably to the skeleton.

## Steering
----
We experimented with many steering mechanisms but the one we found most success was anti-Ackerman steering. Other methods where either too big and complex or didn't turn the right amount. Anti-Ackerman systems are usually used on racing cars where the vehicles must turn at high speeds and the tires might slip, the outer tire’s increased steering angle helps compensate for these slip angles, maximizing grip during high-speed cornering. Even though with this robot we can't reach those speeds where the wheels start slipping, the anti-Ackerman system is still the most effective and simple for this competition.

The steering system is composed of two identicar wheel holders connected with two steering axels, these two axels are then connected to the servo motor in the middle.

![image](https://github.com/user-attachments/assets/c8e9e390-33da-499f-b02f-5bd69cfb3fcb)

## Servo motor:
----

![image](https://github.com/user-attachments/assets/c1188e64-4b96-4dbb-88fa-45dc8717d740) 

|  Voltage |   Temperature   |   Angle of Rotation    |    Torque    |  Control signal  |  Type of Servo  |
|----------|-----------------|------------------------|--------------|------------------|-----------------|
|  3.3V~5V |   -30°C~+60°C   |          180           |   1.6KG/cm   |    PWM signal    |  Digital servo  |

For the motor we used the Steren servo motor, it's an okay motor but we chose it because it was the one we had in hand. Although it is a cheap motor, it works perfectly with the design of the robot.

## Motherboard
----

![image](https://github.com/user-attachments/assets/badc365a-1382-4089-88d6-2129cc35cae7)

|     Chip     |   Clock   |   ROM   |  SRAM  |  FLASH  |        Interfaces        |  Input voltages  |
|--------------|-----------|---------|--------|---------|--------------------------|------------------|
| ESP-WROOM-32 |   240MHz  |  448KB  |  520KB |   4MB   |  UART , I2C , SPI , CAN  |      6-18V       |

For motor driver, we chose the Acebott ESP32, it's capable of controling not only the motors but the sensors as well.

## Skeleton/Chassis
----

This year, instead of making the chassis out of lego, we changed it to 3D printed since it allowed it to be less bulky and lighter unlike the lego version. 

![image](https://github.com/user-attachments/assets/9f6c9e10-1ba4-45d7-8874-0108a5bd213f)

## Energy management
----
## Battery:
----
![image](https://github.com/user-attachments/assets/71818d84-c5d1-4629-8518-718c7c04b7c8)

Model 18605

3.7 V

## Sensors
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

## Multiplexer
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

[Back to table of contents](#table-of-contents)

## Circuit diagram
----

![electric diagram WRO (1)](https://github.com/user-attachments/assets/a96c6d7c-2828-4230-81ea-050892f3166e)


Pins used:

![electric diagram WRO (2)](https://github.com/user-attachments/assets/95201ec8-1249-4721-9a51-392f6b8be53a)

[Back to table of contents](#table-of-contents)

## Program and source code
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

## Open Round
----

At the start of the round and after every turn, the robot ignores any readings that are one meter or further for two seconds. The sensor has to read a distance of more than 1.2 meters to make a turn, if the sensor on the left detects a distance of more than 1.2 meters, the robot will turn left. After three laps the robot will stop in the same spot that it started, at the start of the round the robot is given a number value of 0 and it increases by 1 every time it makes a lap, after 12 laps (sections) the robot will stop at the position that the value of 0 was given. By using this method, the robot is more stable when it comes to making the turns and also avoids getting too close to the walls.

```python

Ronda abierta
#include <Wire.h>
#include <VL53L1X.h>
#include <ESP32Servo.h>
#include "Arduino.h"

// Multiplexores
#define MUX_LEFT_ADDR  0x70
#define MUX_RIGHT_ADDR 0x74
#define MUX_CHANNEL_0  0

// Sensores
VL53L1X sensorLeft;
VL53L1X sensorRight;

// Servo Steam
#define SERVO_PIN 25
#define SERVO_LEFT     15
#define SERVO_CENTER   37
#define SERVO_RIGHT    55
Servo miServo;

// Motor control con shift register
#define SHCP_PIN 18
#define EN_PIN   16
#define DATA_PIN 5
#define STCP_PIN 17
#define PWM1_PIN 19
int M1_Forward = 128;

// Umbral: 1000 mm
#define OBSTACLE_THRESHOLD 1000

int contadorGiros = 0;
bool detenido = false;
unsigned long tiempoInicioRecta = 0;

void selectOnlyOneMux(uint8_t muxAddr) {
  Wire.beginTransmission(MUX_LEFT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(MUX_RIGHT_ADDR); Wire.write(0x00); Wire.endTransmission();
  Wire.beginTransmission(muxAddr); Wire.write(1 << MUX_CHANNEL_0); Wire.endTransmission();
  delay(2);
}

void MoveForward() {
  digitalWrite(EN_PIN, LOW);
  digitalWrite(STCP_PIN, LOW);
  shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, M1_Forward);
  digitalWrite(STCP_PIN, HIGH);
  digitalWrite(PWM1_PIN, HIGH);
}

void StopMotor() {
  digitalWrite(PWM1_PIN, LOW);
}

int lecturaFiltrada(VL53L1X &sensor, uint8_t muxAddr, unsigned long referencia) {
  selectOnlyOneMux(muxAddr);
  int lectura = sensor.read();
  if (lectura <= 0) return 0;
  if ((millis() - referencia < 1800) && lectura > OBSTACLE_THRESHOLD) return 0;
  return lectura;
}

void setup() {
  Serial.begin(115200);
  Wire.begin();

  // Pines motor
  pinMode(SHCP_PIN, OUTPUT);
  pinMode(EN_PIN, OUTPUT);
  pinMode(DATA_PIN, OUTPUT);
  pinMode(STCP_PIN, OUTPUT);
  pinMode(PWM1_PIN, OUTPUT);

  // Servo
  miServo.setPeriodHertz(50);
  miServo.attach(SERVO_PIN, 500, 2400);
  miServo.write(SERVO_CENTER);

  // Sensor izquierdo
  selectOnlyOneMux(MUX_LEFT_ADDR);
  sensorLeft.setTimeout(250);
  sensorLeft.init();
  sensorLeft.setDistanceMode(VL53L1X::Long);
  sensorLeft.setMeasurementTimingBudget(33000);
  sensorLeft.startContinuous(33);

  // Sensor derecho
  selectOnlyOneMux(MUX_RIGHT_ADDR);
  sensorRight.setTimeout(250);
  sensorRight.init();
  sensorRight.setDistanceMode(VL53L1X::Long);
  sensorRight.setMeasurementTimingBudget(33000);
  sensorRight.startContinuous(33);

  tiempoInicioRecta = millis();
  Serial.println("Sistema listo.");
}

void loop() {
  if (detenido) return;

  int distLeft = lecturaFiltrada(sensorLeft, MUX_LEFT_ADDR, tiempoInicioRecta);
  int distRight = lecturaFiltrada(sensorRight, MUX_RIGHT_ADDR, tiempoInicioRecta);

  Serial.print("Izquierdo: "); Serial.print(distLeft); Serial.print(" mm | ");
  Serial.print("Derecho: "); Serial.println(distRight);

  bool giroRealizado = false;

  if (distLeft > OBSTACLE_THRESHOLD) {
    Serial.println("→ Gira a la izquierda");
    StopMotor();
    delay(100);
    miServo.write(SERVO_LEFT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(150);
    MoveForward();
    contadorGiros++;
    tiempoInicioRecta = millis();  // Reinicia tiempo de filtro
    giroRealizado = true;
  }

  if (distRight > OBSTACLE_THRESHOLD) {
    Serial.println("→ Gira a la derecha");
    StopMotor();
    delay(100);
    miServo.write(SERVO_RIGHT);
    delay(2800);
    miServo.write(SERVO_CENTER);
    delay(150);
    MoveForward();
    contadorGiros++;
    tiempoInicioRecta = millis();  // Reinicia tiempo de filtro
    giroRealizado = true;
  }

  if (!giroRealizado) {
    MoveForward();
  }

  if (contadorGiros >= 12) {
    Serial.println("✔ 12 giros completados. Avanzando y deteniendo...");
    MoveForward();
    delay(1000);
    StopMotor();
    miServo.write(SERVO_CENTER);
    digitalWrite(STCP_PIN, LOW);
    shiftOut(DATA_PIN, SHCP_PIN, MSBFIRST, 0x00);
    digitalWrite(STCP_PIN, HIGH);
    digitalWrite(PWM1_PIN, LOW);
    detenido = true;
  }

  delay(60);  // Lecturas rápidas
}

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

(Update) The information that the camera recieves is passed to UART, then the camera only looks for green and red blocks and only detects the color that is closest, that information is then passed to UART

```python

from machine import UART
import sensor, image, time

uart = UART(1, baudrate=115200)

sensor.reset()
sensor.set_pixformat(sensor.RGB565)
sensor.set_framesize(sensor.QQVGA)  # Baja calidad para más FPS
sensor.skip_frames(time=2000)
sensor.set_auto_gain(False)
sensor.set_auto_whitebal(False)

red_threshold = (30, 100, 15, 127, 15, 127)
green_threshold = (30, 100, -127, -15, 15, 127)

ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # 10 segundos

while True:
    img = sensor.snapshot()

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True)

    blob_rojo = max(rojos, key=lambda b: b.pixels(), default=None)
    blob_verde = max(verdes, key=lambda b: b.pixels(), default=None)

    color_detectado = ""
    if blob_rojo and not blob_verde:
        color_detectado = "ROJO"
    elif blob_verde and not blob_rojo:
        color_detectado = "VERDE"
    elif blob_rojo and blob_verde:
        if blob_rojo.pixels() > blob_verde.pixels():
            color_detectado = "ROJO"
        else:
            color_detectado = "VERDE"

    if color_detectado:
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no hay detección

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

(Update) This part of the code trades fps for quality to make it easier to detect the color blocks, it uses the inferior part of the camera so it can see the ground and it ignores the the servo motor because the range of the camera can see the motor and the motor is colored so it could interfer with the reading.

```python

from machine import UART
import sensor, image, time

# Configuración de UART para enviar los datos al ESP32
uart = UART(1, baudrate=115200)

# Inicialización del sensor de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)  # Formato de color RGB
sensor.set_framesize(sensor.QVGA)  # Resolución más baja para mejorar FPS (160x120)
sensor.skip_frames(time=2000)  # Esperar 2 segundos para estabilizar la cámara
sensor.set_auto_gain(False)  # Desactivar ganancia automática para controlar la exposición
sensor.set_auto_whitebal(False)  # Desactivar balance de blancos automático

# Umbrales ajustados para evitar la confusión con naranja
red_threshold = (40, 100, 15, 127, 15, 127)  # Umbral rojo más restringido
green_threshold = (30, 100, -127, -15, 15, 127)  # Umbral verde

# Variables para controlar el envío de datos
ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # Intervalo de 10 segundos entre envíos de color

# Función para ajustar la exposición y mejorar la detección bajo diferentes condiciones de luz
def ajustar_iluminacion():
    img = sensor.snapshot()
    promedio = 0
    for pixel in img:
        promedio += pixel[0]  # Tomar un valor de la componente R (Rojo)
    promedio = promedio // (img.width() * img.height())  # Promedio de la imagen

    # Ajustar la ganancia en función de la iluminación
    if promedio < 100:  # Condición de poca luz
        sensor.set_auto_gain(True)
    else:
        sensor.set_auto_gain(False)

# Función para detectar los colores usando find_blobs (más eficiente)
def detectar_color_blobs(img):
    # Limitar la región a la parte superior de la imagen (evitar la franja en el piso)
    region_superior = (0, 0, img.width(), img.height() // 2)  # Tomar solo la mitad superior de la imagen

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    return rojos, verdes

while True:
    # Ajustar la iluminación según el entorno
    ajustar_iluminacion()

    # Capturar una nueva imagen
    img = sensor.snapshot()

    # Detectar rojo y verde usando blobs (más eficiente)
    rojos, verdes = detectar_color_blobs(img)

    # Filtrar los blobs para encontrar los que tengan un tamaño adecuado (aproximadamente 10 cm de alto)
    rojos_validos = [blob for blob in rojos if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto
    verdes_validos = [blob for blob in verdes if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto

    # Determinar el color detectado
    color_detectado = ""
    if len(rojos_validos) > len(verdes_validos):
        color_detectado = "ROJO"
    elif len(verdes_validos) > len(rojos_validos):
        color_detectado = "VERDE"

    # Enviar el color detectado si ha cambiado o si ha pasado el intervalo de tiempo
    if color_detectado:
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")  # Enviar el color por UART
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no se detecta ningún color

```

(Update) Now it only sees half of its visor and it only detects the color closest to it

```python

from machine import UART
import sensor, image, time

# Configuración de UART para enviar los datos al ESP32
uart = UART(1, baudrate=115200)

# Inicialización del sensor de la cámara
sensor.reset()
sensor.set_pixformat(sensor.RGB565)  # Formato de color RGB
sensor.set_framesize(sensor.QVGA)  # Resolución más baja para mejorar FPS (320x240)
sensor.skip_frames(time=2000)  # Esperar 2 segundos para estabilizar la cámara
sensor.set_auto_gain(False)  # Desactivar ganancia automática para controlar la exposición
sensor.set_auto_whitebal(False)  # Desactivar balance de blancos automático

# Umbrales ajustados para evitar la confusión con naranja
red_threshold = (30, 100, 15, 127, 15, 127)  # Umbral rojo más restringido
green_threshold = (30, 100, -127, -15, 15, 127)  # Umbral verde

# Variables para controlar el envío de datos
ultimo_color = ""
tiempo_ultimo_envio = time.ticks_ms()
intervalo = 10000  # Intervalo de 10 segundos entre envíos de color

# Función para ajustar la exposición y mejorar la detección bajo diferentes condiciones de luz
def ajustar_iluminacion():
    img = sensor.snapshot()
    promedio = 0
    for pixel in img:
        promedio += pixel[0]  # Tomar un valor de la componente R (Rojo)
    promedio = promedio // (img.width() * img.height())  # Promedio de la imagen

    # Ajustar la ganancia en función de la iluminación
    if promedio < 100:  # Condición de poca luz
        sensor.set_auto_gain(True)
    else:
        sensor.set_auto_gain(False)

# Función para detectar los colores usando find_blobs (más eficiente)
def detectar_color_blobs(img):
    # Limitar la región a los 3/4 superiores de la imagen (evitar la franja en el piso)
    region_superior = (0, 0, img.width(), img.height() // 2)  # Usar solo la mitad superior de la imagen

    rojos = img.find_blobs([red_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    verdes = img.find_blobs([green_threshold], pixels_threshold=100, area_threshold=100, merge=True, roi=region_superior)
    return rojos, verdes

# Función para obtener el blob más cercano
def obtener_blob_mas_cercano(rojos, verdes):
    # Verificar que haya blobs en ambos colores
    if not rojos and not verdes:
        return None, None

    # Encontrar el blob más cercano (el que tiene el valor de 'y' más bajo)
    rojo_cercano = min(rojos, key=lambda b: b[1], default=None)  # Minimo valor de 'y' para los rojos
    verde_cercano = min(verdes, key=lambda b: b[1], default=None)  # Minimo valor de 'y' para los verdes

    # Comparar cuál de los dos colores está más cerca
    if rojo_cercano and verde_cercano:
        if rojo_cercano[1] < verde_cercano[1]:  # Si el rojo está más cerca
            return "ROJO", rojo_cercano
        else:  # Si el verde está más cerca
            return "VERDE", verde_cercano
    elif rojo_cercano:  # Si solo se detecta rojo
        return "ROJO", rojo_cercano
    elif verde_cercano:  # Si solo se detecta verde
        return "VERDE", verde_cercano
    return None, None

while True:
    # Ajustar la iluminación según el entorno
    ajustar_iluminacion()

    # Capturar una nueva imagen
    img = sensor.snapshot()

    # Detectar rojo y verde usando blobs (más eficiente)
    rojos, verdes = detectar_color_blobs(img)

    # Filtrar los blobs para encontrar los que tengan un tamaño adecuado (aproximadamente 10 cm de alto)
    rojos_validos = [blob for blob in rojos if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto
    verdes_validos = [blob for blob in verdes if blob[3] >= 10]  # Filtrar bloques que sean al menos 10 píxeles de alto

    # Obtener el blob más cercano
    color_detectado, blob_detectado = obtener_blob_mas_cercano(rojos_validos, verdes_validos)

    # Si se ha detectado un color, dibujar el marco y enviar el color
    if color_detectado and blob_detectado:
        # Dibujar un rectángulo alrededor del blob más cercano
        img.draw_rectangle(blob_detectado[0], blob_detectado[1], blob_detectado[2], blob_detectado[3], color=(255, 0, 0))  # Rojo
        img.draw_string(blob_detectado[0], blob_detectado[1] - 10, color_detectado, color=(255, 0, 0))  # Etiqueta con el color

        # Enviar el color detectado si ha cambiado o si ha pasado el intervalo de tiempo
        tiempo_actual = time.ticks_ms()
        if (color_detectado != ultimo_color) or (time.ticks_diff(tiempo_actual, tiempo_ultimo_envio) > intervalo):
            uart.write(color_detectado + "\n")  # Enviar el color por UART
            print("Color enviado:", color_detectado)
            ultimo_color = color_detectado
            tiempo_ultimo_envio = tiempo_actual
    else:
        ultimo_color = ""  # Reiniciar si no se detecta ningún color

```

[Back to table of contents](#table-of-contents)


