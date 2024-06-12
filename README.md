# Snake Game

This project has the topic of embedded systems, specifically about snake game on ledmatrix using arduino uno.
_The final project will look like this_

![image](https://drive.google.com/file/d/1UyZ3_CvR8rco-Wumczf8Fr224vgEFuWD/view?usp=drive_link)

# Table of contents

- [Introduction](#introduction)
- [Instruction](#instruction)
- [Bill of Material](#bill-of-material)
- [Hardware Schematic](#hardware-schematic)
- [Software Concept](#software-concept)
- [Author](#author)

# Introduction

Features

- Control the snake with the joystick to eat food
- Increase snake speed using potentiometer
- Displays the player's score after finishing the game
- Also displays some other messages such as `snake` and `game over`

# Instruction

Setup instructions follow these steps:

1. Install [Arduino IDE](https://www.arduino.cc/en/software), then install LedControl.h library
2. Set up hardware as [Hardware Schematic](#hardware-schematic) part
3. Upload the program in this github to arduino uno using Arduino IDE
4. Let's play it!

This is a _[demo video of snake game](https://youtu.be/zl4Zn1ty6aY)_

# Bill of Material

| Component name | Quantity |                            Purchase link                             |
| :------------: | :------: | :------------------------------------------------------------------: |
|  Arduino Uno   |    1     |   https://banlinhkien.com/kit-arduino-uno-r3-ch340g-p6649363.html    |
|    JoyStick    |    1     |      https://banlinhkien.com/arduino-ps2-joystick-p6652695.html      |
|   Led Matrix   |    1     | https://banlinhkien.com/diy-led-matrix-8x8-3mm-max7219-p6649623.html |
| Potentiometer  |    1     |       https://banlinhkien.com/triet-ap-don-b1m-p22682414.html        |

# Hardware Schematic

![image](https://drive.google.com/file/d/1sXE36T01lGSweIY69g824HhyEPciCu2n/view?usp=drive_link)

# Software Concept

Data enters the led matrix via DIN signal, then messages, snakes and food can be displayed. Control data is taken from the joystick via VRX and VRY signals so the snake can move in up, down, left, right directions. The potentiometer provides a value from 0 to 1023 via Sig signal, arduino reads this value from pin A5, then maps it to snake's speed, so we can adjust the snake's speed arbitrarily.

# Author

|    Full name     | Student code |
| :--------------: | :----------: |
|  Hoàng Ngọc Hải  |   20204741   |
| Trần Thanh Quang |   20204777   |
|  Trần Công Lập   |   20204760   |
