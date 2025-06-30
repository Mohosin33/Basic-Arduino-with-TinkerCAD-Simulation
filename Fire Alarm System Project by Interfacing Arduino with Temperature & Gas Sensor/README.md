# Fire Alarm System Project by Interfacing Arduino with Temperature and Gas Sensor 🚨

This project monitors gas concentration with a gas sensor and temperature with a temperature sensor[TMP36]. When gas levels rise, a piezo buzzer sounds an alarm, and when temperature crosses a threshold, an LED lights up to indicate overheating.

---

## 🔧 Required Components

- Arduino Uno R3

- Red LED

- Piezo

- Temperature Sensor[TMP36]

- 1 kΩ Resistor

- Gas Sensor

- Breadboard

- Jumper wires

---

## 💡 How it works

- **Sensors measure environmental data:**

     1. Gas Sensor detects gas concentration (smoke, LPG, methane).

     2. TMP36 measures ambient temperature.

- **Arduino reads sensor outputs** using analogRead() on sensor pins.

- **Data is compared to preset thresholds** for gas and temperature levels.

- **If gas level is too high**, Arduino activates the **piezo buzzer** to sound an alarm.
  
- **If temperature exceeds the limit**, Arduino turns on an **LED** to signal overheating.
  
- **Continuous monitoring** runs in a loop, providing real-time alerts to prevent fire hazards.

---

## 📦 Applications

- **🏠 Home safety systems** – Detect gas leaks and overheating in kitchens or living areas

- **🏢 Industrial safety** – Monitor hazardous gas levels and equipment temperature in factories

- **🏫 School or lab safety** – Alert for fire risks during experiments or equipment use

- **🚗 Vehicle safety** – Detect gas leaks or engine overheating in cars or garages

- **🛠️ DIY smart fire alarm** – Low-cost, customizable fire detection system for personal projects
