---
description: Some useful skills I picked up from Robotics
---

# Skills I Picked Up

## Mechanical Design

Mechanical Design refers to designing the mechanism and the more physical aspect of the robots. For example, I learnt how to prototype our robot parts by 3D Modelling them using CAD (computer-aided design) software.

![Fig. 3.3.1: Screenshot of CAD Software (AutoCAD 2023) with RoboCup Robot](<../.gitbook/assets/image (5).png>)

Making analyses of mechanical parts is another important skill.

_Spring plot code:_

```
x = [1, 2, 3, 4, 5, 6]
y = [0.3, 1.3, 1.8, 2.8, 3.3, 4.3]
y = [x/100 for x in y]
x = np.array(x)
y = np.array(y)

plotGraph(x,y)
```

![Fig 3.3.2: Spring strength analysis](../.gitbook/assets/image\_2022-05-22\_113204558.png)

I also learnt how to use the 3D printer that our CCA owns.

![Fig. 3.3.3: Screenshot of 3D Priting Slicing Software (Ultimaker CURA)](<../.gitbook/assets/image (6) (1).png>)

_**insert 3d printed parts here**_

Some of the tools I use for mechanical design, robot assembly etc.

![Fig. 3.2.5: Left to Right: Screwdriver Kit & Case, Screwdriver, Electric Screwdriver, Penknife, Exacto Blade, Tweezers, Digital Vernier Calipers](<../.gitbook/assets/20220522\_103955 (1).jpg>)

## Electrical Design

Electrical design refers to the designing of custom PCBs (Printed Circuit Boards) using design software like Autodesk EAGLE. This allows us to design custom circuits that fit our robot. I believe that this is an important skill and is very useful. I also get to learn about how electrical components work.

Fig. 3.2.5 and 3.2.6 shows one of the many PCB designs from 2021 - 2022's RoboCup Lightweight Competition.

![Fig. 3.2.6: Screenshot of Layer 1 PCB .brd design in PCB Design Software (EAGLE)](<../.gitbook/assets/image (1).png>)

![Fig. 3.2.7: Screenshot of Layer 1 PCB .sch design in PCB Design Software (EAGLE)](<../.gitbook/assets/image (3).png>)

Another skill I picked up is the skill of using a soldering iron. Soldering is a process in which two or more items are joined together by melting and putting a filler metal at high temperatures (\~350°C) into the joint, the filler metal having a lower melting point than the adjoining metal.

![Fig 3.2.8: Google image of soldering process](<../.gitbook/assets/image (6).png>)

_**insert cca soldering station here**_

## Coding & Programming

Being part of robotics also allowed me to be able to learn new programming languages to program my robot. This involves coming up with complex algorithms and making my mechanisms come to life. My team codes our robot with a programming language called C++ or CPP. Below is an example of our code.

_Motor spin test code:_

```
#include <Arduino.h>
#include <i2c_t3.h>
#include <Adafruit_Sensor.h>
#include <Adafruit_BNO055_t3.h>
#include <utility/imumaths.h>
#include <math.h>

void setup(){
    // PWM 22
    // DIR 21
    pinMode(21,OUTPUT);
    pinMode(22,OUTPUT);
}

void loop(){
    analogWrite(21,255);
    digitalWrite(22,HIGH);
    delay(1000);
}
```
