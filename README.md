
- 📷 **Webcam** captures hand gesture in real-time.
- 🧠 **MediaPipe** detects and tracks hand landmarks.
- ✌️ **Finger count** is interpreted (1, 2, or 0 fingers).
- 🔁 **Serial data** is sent to the ESP32.
- 💡 **ESP32** turns ON/OFF appliances (LEDs/Relays) via GPIO.

---

## 🧰 Components Used

| Component              | Quantity | Description                                     |
|------------------------|----------|-------------------------------------------------|
| ESP32 Microcontroller  | 1        | Receives commands from PC and controls devices |
| USB Cable              | 1        | Connects PC to ESP32 (power & serial)          |
| LED or Relay Module    | 1        | Simulates appliance control                    |
| Jumper Wires           | ~5       | Wiring between ESP32 and components            |
| Webcam                 | 1        | Captures live video for gesture detection      |
| Computer (Python 3.x)  | 1        | Runs detection and sends serial commands       |

---

## 🧠 Technologies Used

- **Python 3.x**
- **OpenCV** – Video processing
- **MediaPipe** – Real-time hand & finger tracking
- **PySerial** – Serial communication with ESP32
- **Arduino IDE** – ESP32 programming

---

## 🔌 Circuit Diagram Description

- **LED Setup:**
  - Connect LED1 to **GPIO 23** via a resistor.
  - Connect LED2 to **GPIO 22** via a resistor.
  - Both LED cathodes go to **GND**.
- **Relay (Optional):**
  - IN → GPIO pin
  - VCC → 5V
  - GND → ESP32 GND

---



