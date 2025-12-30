# 🤖 ATtiny45 Motor Driver & 3x3 LED Matrix

![Project Type](https://img.shields.io/badge/Project-Educational_Hardware-yellow)
![MCU](https://img.shields.io/badge/MCU-ATtiny45-blue)

## 📌 Overview
This project is an **educational hardware circuit** designed to demonstrate the fundamentals of embedded systems. It integrates a custom-built DC motor driver, a visual LED matrix, and audio feedback, all controlled by the compact **ATtiny45 microcontroller**.

> [!NOTE]
> This project focuses exclusively on **Hardware Design**. The software implementation/firmware is not included as part of this specific repository.

---

## 🎯 Features

* **Custom H-Bridge:** Controls a DC motor using a discrete transistor-based H-Bridge (4x NPN).
* **Visual Display:** A **3x3 LED Matrix** for displaying patterns or status indicators.
* **Audio Output:** Integrated **Buzzer** for sound notifications or alerts.
* **Efficient Control:** All peripherals are managed by the 8-bit ATtiny45.
* **Power Management:** External power input with a dedicated manual toggle switch.

---

## 🧩 Components Used

| Component | Specification | Purpose |
| :--- | :--- | :--- |
| **Microcontroller** | ATtiny45 | The "Brain" of the system. |
| **Transistors** | 4x BC547 (NPN) | Used to build the discrete H-Bridge. |
| **DC Motor** | Standard Small DC | Mechanical output/Motion. |
| **LED Matrix** | 3x3 Configuration | Visual output/Pattern display. |
| **Buzzer** | Active/Passive | Sound generation. |
| **Switch** | SPST Toggle/Slide | Master power control. |
| **Power Source** | Battery / DC Adapter | System energy supply. |

---

## ⚙️ Circuit Design Logic

### 🔄 Transistor H-Bridge
Instead of using an integrated circuit (like the L298N), this project utilizes a **manual H-Bridge** built from four **BC547 NPN transistors**. This allows students to understand how current direction is toggled to change motor rotation.


### 🧠 ATtiny45 Integration
Despite the limited I/O pins of the ATtiny45, the circuit is optimized to handle:
1.  **Motor Direction:** Signal pins sent to the H-Bridge.
2.  **Matrix Multiplexing:** Controlling 9 LEDs efficiently.
3.  **Frequency Output:** Driving the buzzer.

### 🔌 Power Flow
The circuit is designed to handle external power, with the switch acting as a safety cut-off between the source and the components.

---

## 🎓 Educational Purpose
This project was developed as a learning tool to showcase:
* **Discrete Component Design:** Building motor drivers from scratch using transistors.
* **Multiplexing Concepts:** Managing an LED matrix with limited GPIO pins.
* **Minimalist Embedded Design:** Maximizing the utility of low-pin-count microcontrollers.

---

## 📜 License
This project is shared for **educational purposes only**. You are free to use, modify, and study the hardware design for your own learning or teaching needs.
