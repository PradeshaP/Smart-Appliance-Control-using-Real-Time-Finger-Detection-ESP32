# 🖐️ Smart Appliance Control using Real-Time Finger Detection & ESP32

Control appliances like lights or fans with just your **fingers** using **computer vision** and an **ESP32 microcontroller**. This project detects the number of fingers shown via a webcam using Python (OpenCV + MediaPipe), and sends the count over USB serial to the ESP32, which activates the appropriate appliance.

---

## 🎯 Project Objective

Create a **hands-free appliance control system** by detecting finger gestures using a webcam and controlling physical devices like LEDs or relays using ESP32 GPIOs.

---

## 📸 How It Works

Webcam ──▶ Python (OpenCV + MediaPipe) ──▶ Finger Count ──▶ Serial to ESP32 ──▶ LED / Relay Control
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



