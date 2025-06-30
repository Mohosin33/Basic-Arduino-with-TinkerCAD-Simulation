# Dimmer Circuit using Arduino 💡

A dimmer circuit using Arduino allows you to control the brightness of an LED or lamp by adjusting the output voltage through PWM (Pulse Width Modulation). This enables smooth, real-time brightness control using components like a potentiometer, IR remote, or sensor.

---

## 🔧 Required Components

- Arduino Uno R3

- Light bulb

- 250 kΩ Potentiometer

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## 💡 How it works

- **Input device (e.g., potentiometer)** provides a variable analog signal.

- **Arduino reads the analog input** using analogRead().

- **Value is mapped to PWM range (0–255)** to match brightness levels.

- **PWM signal is sent to output pin** using analogWrite() to control LED or lamp brightness.

- **Brightness adjusts smoothly** based on input value, allowing real-time dimming.

---

## 📦 Applications

- 💡 Smart lighting systems

- 🖥️ Backlight control

- 🧪 Lab equipment

- 🛠️ DIY lamp projects
