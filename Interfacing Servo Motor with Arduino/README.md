# 🔄📐 Interfacing Servo Motor with Arduino

This project demonstrates how to control the position of a servo motor using Arduino by sending angle commands through a digital pin. It enables precise movement of the servo shaft to preset angles with timed delays, useful in robotics and automation applications.

---

## 🔧 Required Components

- Arduino Uno R3

- Positional Micro Servo

- Jumper wires

---

## ⚙️ How It Works

- The **Servo library** is included to simplify controlling servo motors.

- A servo object is created and attached to **digital pin 7**, where the servo signal wire is connected.

- Inside the loop(), the servo motor is rotated to **0°, 90°, and 180°**, each followed by a **2-second delay**.

- These angles represent different shaft positions, and the servo holds each position before moving to the next.

- The cycle repeats continuously, causing the servo to sweep between the set angles.

---

## 📦 Applications

- 🤖 **Robotic Arms** – Precise control of joints for picking, placing, or moving objects.

- 🚪 **Automatic Door or Lock Systems** – Servo opens or closes mechanisms based on signals.

- 📷 **Camera Gimbals & Pan-Tilt Systems** – Adjust camera angles smoothly for surveillance or filming.

- 🛰️ **Solar Panel Tracking Systems** – Servo moves panels to follow the sun.

