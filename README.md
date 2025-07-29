Great, thanks for the details. Here’s a professional and clean `README.md` tailored for your IRO project repository (`iro`):

---

```markdown
# IRO Line-Tracing Robot Code (Probot)

This repository contains code developed for the **International Robotics Olympiad (IRO)**, using the **Probot** robotics platform and the `pro.aps` environment. The code is written in **C** (compatible with AVR Studio 4.18 / WinAVR) and is designed to perform precise **line-tracing**, **servo manipulation**, and **object handling** tasks on Roborobo's **Black Line ProR** hardware.

## 🧠 Overview

- Designed for the **ATmega64A** microcontroller.
- Includes advanced **line following**, **turning**, **servo control**, and **object pickup/drop** logic.
- Built specifically for the International Robotics Olympiad challenges.
- Uses a series of macros and function definitions for clean abstraction and readability.

## 📦 Environment

- **MCU**: ATmega64A
- **IDE**: AVR Studio 4.18 (Build 692)
- **Compiler**: WinAVR 20100110 or later
- **Robot**: Roborobo Probot (Black Line ProR)
- **OS Support**: Windows XP / Vista / 7

## 🧩 Features

- Multi-speed line tracing using front/rear sensors.
- 90-degree and curved turning macros.
- Servo-based object grabbing, releasing, and lifting.
- Abstracted motor/servo sequences for easy task composition.
- Cross detection and error handling logic.
- Modular movement patterns like `circleback`, `circlego`, etc.

## 🚀 Usage

1. Install AVR Studio 4.18 and WinAVR (20100110 or later).
2. Flash the compiled binary to your Probot robot via the ISP interface.
3. Ensure sensor calibration and servo alignment before use.
4. Trigger specific challenge routines via `main()`'s behavior tree.
```


````
> Note: You must have `proBase.h` and other dependencies from the Roborobo SDK.

## 🔧 Sample Macros

```c
#define circlego __rr1; motor(10, 10, 200); __rt_90; ...
#define turnl lturn(0,13);
#define closes servo1(35); servo2(11);
````

## 📷 Media

> Coming soon: photos and demo videos of the robot in action!

## 📜 License

This repository is intended for **educational and competition use only**. Please respect Roborobo’s original copyrights.

---

**Author:** WhateversOnMyMind
**Competition:** International Robotics Olympiad
**Robot:** Roborobo Probot (Black Line ProR)
