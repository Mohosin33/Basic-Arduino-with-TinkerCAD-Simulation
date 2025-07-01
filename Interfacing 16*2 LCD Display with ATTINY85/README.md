# 📟 Interfacing 16*2 LCD Display with ATTINY85 

Interfacing a 16x2 LCD with ATTINY85 (without I2C) allows us to display custom messages using 6 digital pins in 4-bit mode. It's perfect for showing simple text or alerts in small embedded applications.

---

## 🔧 Required Components

- LCD 16 x 2

- ATtiny

- 1 kΩ Resistor

- Battery

- Breadboard

- Jumper wires

---

## 💡 How it works

- ATTINY85 sends each character of the sentence in 4-bit mode using 6 pins.

- LCD is initialized, then characters are sent one by one using digital signals.

- RS pin is set high to send data (letters), and EN is pulsed to latch each character.

- Sentences are stored as strings in code and printed using lcd.print() function.

- The LCD shows the sentence across 2 lines (16 characters each).

---

## 📦 Applications

- ✅ **Mini digital message boards** for simple notifications.

- 📟 **Status display** in small embedded systems (e.g., “System Ready”, “Error!”).

- 🌡️ **Sensor-based alerts**, like “Temp High” or “Gas Detected”.

- 🔐 **Security systems**, displaying “Access Granted” or “Wrong Password”.

- 🔋 **Battery or power indicators**, showing “Low Battery” or “Charging”.

- 🛠️ **DIY projects** like clocks, counters, or timers with text output.

- 🚪 **Smart home modules** displaying room status or control messages.
