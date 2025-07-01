# 🏃💡Interfacing PIR Sensor with Arduino

In this project, a **PIR sensor** is connected to an **Arduino** to detect motion based on infrared radiation. When the sensor detects movement, it sends a **HIGH signal** to the Arduino, which in turn turns **ON an LED** as an alert or indicator. This simple yet effective setup is ideal for motion-activated lighting and basic security systems.

---

## 🔧 Required Components

- Arduino Uno R3

- PIR Sensor

- Blue LED

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- **PIR sensor OUT pin** is connected to digital **pin 13** of the Arduino.

- An **LED** is connected to **pin 7**.

- In setup(), the Arduino sets the **PIR pin as INPUT** and the **LED pin as OUTPUT**.

- The Arduino continuously **reads the PIR sensor** output using digitalRead(pirPin).

- If **motion is detected** (motion == HIGH):

     - The LED on pin 7 is turned **ON** using digitalWrite(ledPin, HIGH).

     - A message “**Motion Detected!**” is printed on the **Serial Monitor**.

- If **no motion is detected** (motion == LOW):

- The LED is turned **OFF** using digitalWrite(ledPin, LOW).

- A **1-second delay** stabilizes the output and avoids rapid blinking.

---

## 📦 Applications

- 💡 **Automatic lighting systems** – Turn lights ON when someone enters a room.

- 🚪 **Smart door alerts** – Notify when someone is at the door or passes by.

- 🛏️ **Bedroom light automation** – Auto turn on soft lighting during night movement.

- 🤖 **Motion-activated robots** – Trigger robot actions based on human presence.

- 🏢 **Office energy saving** – Automatically switch off devices when no motion is detected.
