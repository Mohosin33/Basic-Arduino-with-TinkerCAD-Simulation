# 🌈➡️LED Flowing lights using Arduino

This project creates a flowing or chasing light effect by sequentially turning on and off 8 LEDs connected to pins 1 through 8. It simulates a wave-like motion by lighting LEDs in order with timed delays, commonly used in visual displays and decorations.

---

## 🔧 Required Components

- Arduino Uno R3

- Red LED

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- In the setup(), a for loop sets **digital pins 1 to 8 as OUTPUT**, preparing them to control LEDs.

- In the loop(), the **first for loop** turns each **LED ON one by one** from pin 1 to 8 with a **300 ms delay** between each — creating a forward flowing effect.

- The **second for loop** then turns **each LED OFF in the same order** with the same delay, clearing the LEDs.

- This process **repeats continuously**, creating a **right-to-left LED flowing or chasing pattern**.

- The delay between each step creates the illusion of movement, making it visually appealing for effects and display systems.

---

## 📦 Applications

- 💡 **LED Decoration Projects** – Creates eye-catching flowing effects for lighting decorations or events.

- 🚗 **Automotive Turn Signals** – Simulates sequential LED indicators in cars or bikes.

- 🖥️ **Visual Status Indicators** – Shows progress, activity, or status in machines or systems.

- 🧠 **Microcontroller Learning** – Helps beginners understand pin control, loops, and timing in Arduino.

