# 📡📏 Interfacing Ultrasonic Sensor with Arduino

This project uses an ultrasonic sensor to measure distance by sending and receiving sound waves. The Arduino triggers the sensor, calculates the time taken for the echo to return, and then converts it into a distance value displayed or used for obstacle detection.

---

## 🔧 Required Components

- Arduino Uno R3

- Ultrasonic Distance Sensor(4-pin)

- jumper wires

---

## ⚙️ How It Works

- The ultrasonic sensor has two pins: **TRIG_PIN (pin 9)** and **ECHO_PIN (pin 10)**.

- In setup(), the trigger pin is set as output and the echo pin as input; serial communication is started to send data to the Serial Monitor.

- In the loop(), first the trigger pin is cleared (set LOW) briefly to prepare for the next pulse.

- Then, the trigger pin is set HIGH for **10 microseconds** to send an ultrasonic pulse.

- The sensor emits an ultrasonic sound wave and waits for the echo to return.

- The Arduino measures the **duration** of the echo pulse using pulseIn() on the echo pin, which returns the time (in microseconds) it took for the sound to travel to the obstacle and back.

- The distance is calculated with:
    distance = duration * 0.034 / 2;

  - 0.034 cm/µs is the speed of sound in air.

  - Dividing by 2 accounts for the round trip (to the obstacle and back).

- The calculated distance (in cm) is printed to the Serial Monitor.

- The program waits for 500 milliseconds and repeats the measurement continuously.

---

## 📦 Applications

- 🚗 **Obstacle Avoidance in Robots** – Detects nearby objects to prevent collisions in autonomous vehicles.

- 🏠 **Smart Parking Systems** – Measures distance to help guide cars in tight parking spaces.

- 📏 **Digital Distance Measurement Tools** – Acts as a contactless ruler for short-range measurements.

- 🚪 **Automatic Door Control** – Detects when a person approaches to open doors automatically.

