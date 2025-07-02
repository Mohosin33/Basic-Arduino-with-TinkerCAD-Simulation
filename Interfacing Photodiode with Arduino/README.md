# 📟Interfacing Photodiode with Arduino

**Interfacing a photodiode with Arduino** allows detection of light intensity by converting light into a varying voltage signal. The Arduino reads this signal through an analog pin and displays the value in real time via the Serial Monitor.

---

## 🔧 Required Components

- Arduino Uno R3

- Photodiode

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- sensorPin is set to A0, where the photodiode is connected as an analog input.

- In setup(), the Arduino initializes serial communication at 9600 baud rate and sets the pin mode.

- In the loop(), the Arduino reads analog voltage from the photodiode using analogRead(sensorPin).

- The sensor value, which changes with light intensity, is printed to the Serial Monitor.

- Higher light levels usually give higher analog values (depending on the circuit).

---

## 📦 Applications

- 🔆 **Light Intensity Measurement** – Detects ambient light level in smart lighting systems.

- ⏱️ **Line Following Robots** – Differentiates between black and white surfaces using light reflection.

