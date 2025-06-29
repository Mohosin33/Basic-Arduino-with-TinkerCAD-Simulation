# Breathing LED with Arduino 💡

Breathing an LED with Arduino creates a smooth fading effect by gradually increasing and decreasing the LED's brightness using PWM (analogWrite). This simulates a natural “breathing” pattern, often used in status indicators.

---

## 🔧 Required Components

- Arduino Uno R3

- Red LED

- 1kΩ Resistor

- Breadboard

- Jumper wires

---

## 💡 How it works

The breathing LED effect works by using PWM (Pulse Width Modulation) to smoothly adjust the LED brightness:

- analogWrite(pin, value) sends a rapidly switching signal where the "on time" is varied from 0 (off) to 255 (fully on).

- In a loop, the brightness value is gradually increased and decreased using a small delay between steps, creating a smooth fade in and fade out — like a slow, rhythmic breathing motion.

---

## 📦 Applications

- Power Indicator

- Aesthetic Lighting

- Medical Simulation
