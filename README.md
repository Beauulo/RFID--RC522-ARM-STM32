# RFID-RC522-ARM-STM32
# 🔐 STM32 RFID Door Lock System

A secure and real-time door locking system using an **STM32F446RE** microcontroller, **RC522 RFID reader**, **servo motor**, and **I2C LCD display**. Built entirely using **STM32CubeIDE** with **HAL drivers**, this project demonstrates SPI, I2C, and PWM peripheral integration for embedded access control applications.

---

## 📸 Demo
Found on my linkedin Profile 

---

## 🛠️ Hardware Used

| Component              | Function                             |
|------------------------|--------------------------------------|
| STM32F446RE            | Main microcontroller (NUCLEO board)  |
| RC522 RFID Module      | Reads RFID/NFC cards (SPI interface) |
| 2x16 LCD Display (I2C) | Displays access status               |
| Servo Motor (SG90)     | Controls door lock (PWM signal)      |
| RFID Tags/Cards        | Authentication tokens                |
| Power Supply           | 5V Breadboard Power Supply           |
| Jumper Wires           | Connections                          |
| Breadboard             | Prototyping                          |

---

## ⚙️ Features

- Detects authorized RFID cards using the **RC522 module (SPI)**
- Displays status ("Access Granted"/"Access Denied") on an **I2C LCD**
- Opens the door by rotating a **servo motor** on successful authentication
- Uses **HAL drivers** in **STM32CubeIDE** for clean, modular embedded code

---

## 🧠 What I Learned

- Initializing and using **SPI, I2C, and PWM** on STM32
- Structuring embedded code with **HAL API**
- Real-world debugging and hardware-software interfacing
- Creating an embedded system from scratch with real-time feedback

---

## 🔄 System Workflow

1. RFID card is scanned by the RC522 module.
2. STM32 compares card UID to a list of authorized IDs.
3. If UID is authorized:
   - LCD displays "Access Granted"
   - Servo rotates to unlock the door
4. If UID is not authorized:
   - LCD displays "Access Denied"
   - Servo remains locked



