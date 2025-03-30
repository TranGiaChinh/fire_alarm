# 🔥 Fire Alarm System Based on ESP32

## 📌 Overview
This project builds a fire alarm system using **ESP32**, integrating multiple sensors to detect smoke, gas, infrared motion, temperature, and humidity (**DHT11**). The system sends real-time data via **WiFi** to a **Node.js server** for local monitoring.

## 🚀 Features
- **Sensors:**
  - 🔥 Smoke Sensor (**MQ-2** or similar)
  - 💨 Gas Sensor (**MQ-5** or similar)
  - 🏃 Infrared Motion Sensor
  - 🌡️ Temperature & Humidity Sensor (**DHT11**)
- **Alarm System:**
  - 🔊 Activates **buzzer** when fire is detected.
  - 🔘 Manual activation via **push button**.
- **WiFi Connectivity:**
  - Sends sensor data to the **server via HTTP POST**.
- **Web Interface:**
  - Displays real-time sensor data using **HTML & WebSocket**.

## 🛠 Hardware Requirements
- **ESP32 Dev Module** (e.g., ESP32-WROOM-32)
- **MQ-2 Smoke Sensor**
- **MQ-5 Gas Sensor**
- **Infrared Motion Sensor**
- **DHT11 Temperature & Humidity Sensor**
- **Buzzer** (for alarm notifications)
- **Push Button** (for manual activation)
- **Power Supply 3.3V/5V** (USB or battery)

## 📂 Project Structure
```
fire-alarm-system/
 ├── esp32/          # ESP32 Code
 │   └── fire_alarm.ino  # Arduino source file for ESP32
 ├── server/        # Node.js Server Code
 │   ├── server.js      # Main server file
 │   ├── public/       # Web interface folder
 │   │   └── index.html  # Web dashboard
 │   └── package.json   # Node.js dependencies
 └── README.md      # This documentation
```

## ⚙️ How to Set Up & Run
### 1️⃣ ESP32 Setup
1. Install **Arduino IDE** and add ESP32 board support.
2. Connect the sensors to the ESP32 following the **wiring diagram**.
3. Upload `fire_alarm.ino` to the ESP32.

### 2️⃣ Server Setup
1. Install **Node.js** on your computer.
2. Navigate to the `server/` folder and run:
   ```sh
   npm install  # Install dependencies
   node server.js  # Start the server
   ```
3. Open `http://localhost:3000` in your browser to monitor sensor data.

## 🎯 Expected Results
- The system continuously monitors smoke, gas, temperature, and motion.
- If a fire is detected, the **buzzer** is triggered and data is sent to the **server**.
- The **web dashboard** displays real-time sensor values.

