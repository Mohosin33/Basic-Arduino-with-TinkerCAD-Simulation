# 🔴🟢🔵Interfacing NeoPixel strip _4 with Arduino

This project involves connecting a NeoPixel RGB LED strip to an Arduino to control individual LEDs with precise color and brightness. Using a single data pin, the Arduino sends color data to the strip, enabling dynamic lighting effects, animations, and customized color patterns.

---

## 🔧 Required Components

- Arduino Uno R3

- NeoPixel Strip 4

- Jumper wires

---

## 💡 How it works

- **The NeoPixel strip** is connected to **pin 6** of the Arduino.

- The strip has **4 RGB LEDs**, each **individually addressable**.

- The Arduino uses the **Adafruit_NeoPixel library** to control the LEDs.

- Colors are defined using strip.Color(R, G, B) for **RED, GREEN, BLUE**.

- In each step of the loop, **specific LEDs are set to specific colors**.

- The strip.show() function sends color data to the LEDs.

- The color pattern **shifts from left to right** every 100 ms.

- After 6 color steps, all LEDs are turned **OFF** in step 7.

---

## 📦 Applications

- 🎉 **Decorative lighting** for rooms, costumes, or events.

- 🎨 **LED color sequencing demo** to understand RGB transitions.

- 🌈 **Custom light patterns** for art and design.
