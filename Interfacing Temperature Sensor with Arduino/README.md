# 🌡️📟 Interfacing Temperature Sensor with Arduino

This project reads analog data from an LM35 temperature sensor, converts it to voltage, and calculates the temperature in both Celsius and Fahrenheit. The temperature values are displayed in real-time on the Serial Monitor for continuous monitoring.

---

## 🔧 Required Components

- Arduino Uno R3

- Temperature Sensor[TMP36]
- Jumper wires

---

## ⚙️ How It Works

- The sensor is connected to analog pin A0 (tempPin = A0).

- In setup(), serial communication starts with Serial.begin(9600) to send data to the Serial Monitor.

- In the loop(), the Arduino reads the analog voltage from the TMP36 sensor using analogRead(tempPin). This gives a value between 0 and 1023.

- The analog reading is converted to voltage with:
voltage = (analogValue * 5.0) / 1024.0;
Here, 5.0 is the reference voltage and 1024 is the ADC resolution.

- The voltage is converted to temperature in Celsius using the TMP36 formula:
temperatureC = (voltage - 0.5) * 100;
(0.5V corresponds to 0°C, and each 0.01V corresponds to 1°C)

- Celsius is converted to Fahrenheit:
temperatureF = (temperatureC * 9.0 / 5.0) + 32.0;

- Finally, all values — analog reading, voltage, Celsius, and Fahrenheit — are printed to the Serial Monitor with Serial.print() and Serial.println().

- The delay(1000) pauses the program for 1 second before repeating the process.

---

## 📦 Applications

- 🌡️ **Room Temperature Monitoring** — Measure and log ambient temperature in homes or offices.

- 🧪 **Environmental Data Logging** — Collect temperature data for scientific experiments.

- 🔥 **Overheat Protection Systems** — Detect high temperatures in devices or motors to trigger cooling.

- 🌿 **Agricultural Automation** — Monitor greenhouse or soil temperature to optimize plant growth.
