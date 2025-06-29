# Controlling LEDs using IR Remote and Arduino UNO 💡

Controlling LEDs using an IR remote and Arduino UNO allows you to wirelessly switch LEDs on or off using an IR remote control. It uses an IR receiver to decode signals and trigger corresponding LED actions based on button presses.

---

## 🔧Required Components

- Arduino Uno R3

- Red LED

- Green LED

- Blue LED

- IR Sensor

- 1kΩ Resistor

- IR Remote

- Breadboard

- Jumper wires

---

## 💡How it works

- **IR Remote sends signals:** Each button on the IR remote emits a unique infrared code.

- **IR Receiver receives signal:** The IR sensor connected to Arduino receives the signal as pulses.

- **Arduino decodes the signal:** Using the IRremote library, Arduino decodes the pulses into a hexadecimal code.

- **Code matches command:** The decoded signal is compared with predefined values for each button.

- **LED reacts:** Based on the matched code, Arduino turns ON, OFF, or toggles the connected LED(s).

- **Loop continues:** Arduino continuously listens for IR signals in the loop() function.

---

## 📦Applications

- Remote-controlled room light

- IR-based LED decoration

- TV or PC backlight control

- IR remote-controlled toy or robot light

- Wireless status indicator system

---
