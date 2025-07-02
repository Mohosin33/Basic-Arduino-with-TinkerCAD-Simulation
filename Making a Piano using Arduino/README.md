# 🎹🔊Making a Piano using Arduino

This project creates a simple digital piano using push buttons and a buzzer, where each button plays a different musical tone. When a button is pressed, the Arduino generates a specific frequency sound through the buzzer to mimic piano keys.

---

## 🔧 Required Components

- Arduino Uno R3

- Pushbutton

- Piezo

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- **8 push buttons** are connected to **digital pins 2–9**, and each one acts as a piano key.

- A **buzzer** is connected to **pin 13**, which produces sound based on the input.

- In setup(), all buttons are set as **input**, and the buzzer pin is set as **output**.

- In the loop(), the Arduino constantly checks if any button is pressed using digitalRead() for each pin.

- If a button is pressed (digitalRead == 1), the tone() function is used to play a specific **frequency (Hz)** on the buzzer.

- Each button is mapped to a different tone (e.g., 300 Hz to 1000 Hz), creating different musical notes.

- A short delay (delay(10)) is added at the end of the loop to reduce bouncing and repeat speed.

- This process repeats continuously, allowing users to press any button and hear a corresponding note — just like a mini piano.

---

## 📦 Applications

- 🎵 **DIY Mini Electronic Piano** – Create a basic musical instrument for learning and fun.

- 🧠 **Educational Tool** – Teach students about sound frequency, tone generation, and digital input handling.

- 🎶 **Music Learning Projects** – Help beginners understand the relationship between button input and musical notes.

- 🔊 **Custom Alert Systems** – Adapt the code to play different tones for different system alerts or events.

