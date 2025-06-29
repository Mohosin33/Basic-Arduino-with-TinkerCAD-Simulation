# Controlling the brightness of LED using Attiny85 💡

Controlling the brightness of an LED using ATtiny85 and a potentiometer allows real-time dimming based on analog input. The potentiometer sets a voltage level, which the ATtiny85 reads and converts to a PWM signal for the LED.

---

## 🔧 Required Components

- Coil Cell 3V Battery

- ATtiny

- 250 kΩ Potentiometer

- 1 kΩ Resistor

- Green LED

- Breadboard

- Jumper wires

---

## 💡 How It Works
- **Potentiometer varies voltage** – Turning the knob changes voltage between 0–5V.

- **ATtiny85 reads analog input** – It uses analogRead() to measure the potentiometer's output.

- **Value is mapped to PWM range** – The analog value (0–1023) is scaled to 0–255 for PWM.

- **PWM controls LED brightness** – analogWrite() sends a PWM signal to the LED pin.

- **LED dims or brightens** – As the potentiometer turns, brightness changes smoothly.

---

## 📦 Applications

- Dimmer switch for lamps or LEDs

- Battery-powered lighting control

- Light level adjustment in art installations
