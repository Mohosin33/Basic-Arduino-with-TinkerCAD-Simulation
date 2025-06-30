# Creating Digital Voltmeter using Arduino

Creating a digital voltmeter using Arduino allows us to measure and display voltage levels from analog inputs in real time. It reads voltage using `analogRead()` and converts it into a readable voltage value displayed on a serial monitor or LCD.

---

## 🔧 Required Components

- Arduino Uno R3

- LCD 16 x 2

- Power Supply

- 1kΩ Resistor

- Breadboard

- Jumper wires

---

## 💡 How it works

- **Analog voltage input** – A voltage signal is connected to an analog pin (e.g., A0).

- **Arduino reads analog value** – analogRead() captures values from 0 to 1023 (10-bit).

- **Value is converted to voltage** – The analog value is mapped to 0–5V using a formula.

- **Calculated voltage is displayed** – The voltage is shown on Serial Monitor or LCD.

- **Continuous monitoring** – The loop keeps updating the voltage reading in real time.

---

## 📦 Applications

- 🔋 Battery voltage monitoring

- ⚡ Power supply voltage check

- 🔧 DIY electronics testing

- 📟 Real-time voltage display in circuits

- 🧪 Lab experiments and student projects
