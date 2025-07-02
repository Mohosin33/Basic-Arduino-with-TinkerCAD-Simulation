# 🌞💡Light Intensity Measurement using LDR sensor and Arduino

This project reads light intensity using an LDR connected to an analog pin and displays the value on the Serial Monitor. The brightness of an LED is adjusted automatically based on the ambient light level using PWM output.

---

## 🔧 Required Components

- Arduino Uno R3

- Red LED

- Photoresistor

- Voltage Multimeter

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- The **LDR (Light Dependent Resistor)** is connected to **analog pin A0**, where it senses the ambient light level.

- In the setup(), the Serial Monitor is initialized and **pin 8** is set as an output to control an LED.

- Inside the loop(), the Arduino reads the LDR’s analog value using analogRead(A0). This value ranges from **0 (bright light)** to **1023 (dark)**.

- The LDR value is printed to the Serial Monitor for real-time observation.

- The map() function scales the LDR value to a range of **0–255**, which matches the PWM range used by analogWrite().

- The scaled value is sent to **pin 8**, changing the brightness of an LED based on light intensity — **brighter in dark, dimmer in light**.

- The process repeats every 500 milliseconds, continuously updating the LED based on current light conditions.

---

## 📦 Applications

- 💡 **Automatic Street Lighting** – Turns lights on at night and off during the day based on ambient light.

- 📱 **Screen Brightness Control** – Adjusts display brightness in phones, laptops, or devices using surrounding light.

- 🌞 **Smart Window Blinds** – Opens or closes blinds depending on sunlight intensity.

- 🌿 **Greenhouse Light Monitoring** – Measures sunlight levels to manage plant lighting conditions.
