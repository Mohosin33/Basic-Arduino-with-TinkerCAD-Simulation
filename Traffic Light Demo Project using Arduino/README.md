# 🚦Traffic Light Demo Project using Arduino

This project simulates a basic traffic light sequence controlled by a button input. When pressed, it cycles through red (Stop), yellow (Get Ready), and green (Start) LEDs, displaying each state for a fixed time.

---

# 🔧 Required Components

- Arduino Uno R3

- Red LED

- Yellow LED

- Green LED

- Pushbutton

- 1 kΩ Resistor

- Breadboard

- Jumper wires

---

## ⚙️ How It Works

- Three LEDs (Red, Yellow, Green) are connected to **pins 10, 9, and 8**, and a push button is connected to **pin 5** with an internal pull-up resistor.

- In setup(), all LEDs are set as outputs, and the button pin is set as an input with pull-up, so it reads **HIGH (1)** when not pressed and **LOW (0)** when pressed.

- In the loop(), the Arduino continuously reads the state of the button using digitalRead(buttonPin).

- When the button is pressed (buttonState == 1), it starts **the traffic light sequence**:

    - 🟥 **Red LED ON** – Displays "Stop" and waits 2 seconds.

    - 🟨 **Yellow LED ON** – Turns off red, turns on yellow, shows "Get Ready", and waits 2 seconds.

    - 🟩 **Green LED ON** – Turns off yellow, turns on green, shows "Start", and waits 2 seconds.

- After completing the cycle, all LEDs are turned off.

- The program waits until the button is **released** before allowing another cycle, preventing accidental repeats.

---

## 📦 Applications

- 🚦 **Traffic Light Simulation for Education** – Teaches students how real traffic lights work using simple electronics.

- 🧠 **Embedded Systems Learning** – Introduces control logic using LEDs, delays, and button input.

- 🎮 **Game or Toy Traffic Setups** – Adds realistic signaling to mini traffic or racing games.

- 🏠 **Smart Home Projects** – Can be adapted for driveway exit alerts or home vehicle gates.
