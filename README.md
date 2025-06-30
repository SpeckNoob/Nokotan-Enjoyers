Mustangs Down
====

This repository contains the documentation for the Mustangs Down team's robot for the 2025 World Robot Olympiad Future Engineers category competition. The robot was designed and built by a team of three.

The team
======

Mark Chen, Age: 16

![image](https://github.com/user-attachments/assets/263bca30-1d4f-4f59-a675-890829c32520)

School: Panamerican School of Panama, PAS

Hi!, I'm Mark from Panama with Chinese origin born in February 8 2009. I've been participating in WRO since 2022 and this is my second year participating in the Future Engineers category. I enjoy playing piano and I am a part of a school band, other hobbies include cubing (Rubik's cube competitions), gaming, drawing and writing.

----

Juan Pablo Gomez, Age: 16

![image](https://github.com/user-attachments/assets/b9244ac9-54e1-4af8-89d1-042ac478571a)

School: Panamerican School of Panama, PAS

lorem ipsum

----

Julio Chong, Age: 16

![image](https://github.com/user-attachments/assets/39dfb391-f71d-4759-b822-fce67cd3f061)

School: Panamerican School of Panama, PAS

My name is Julio Chong, a panamenian teen with chinese antescedents who was born in August 24, 2008. I've been into robotics since 9th grade on 2023. My hobbies are playing the guitar, cooking, coding, learning new languages and also doing lots of exercise or sport, especially contact sports such as jiujitsu.

----

Victor Sanchez (Coach), Age: 35

(insert picture)

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

Photos of the robot
====

(Insert picture) (Insert picture)

(Insert picture) (Insert picture)

(Insert picture) (Insert picture)

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

Motor Driver
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

The servo motor is supported by the distance sensors in both right and left sides of the robot, the servo moves accordingly wether the sensors detect a wall on the left or right, additionaly, at the end it checks if it passed the time limit for the code to function.

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

