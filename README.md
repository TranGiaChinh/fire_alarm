# 🔥 Fire Alarm System Based on ESP32

## 📌 Overview
This project builds a fire alarm system using **ESP32**, integrating multiple sensors to detect smoke, gas, infrared motion, temperature, and humidity (**DHT11**). The system sends real-time data via **WiFi** to a **Node.js server** for local monitoring.

## 🚀 Features
- **Sensors:**
  - 🔥 Smoke Sensor (**MQ-2** or similar)
  - 💨 Gas Sensor (**MP-2** or similar)
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
- **MP-2 Gas Sensor**
- **Infrared Motion Sensor**
- **DHT11 Temperature & Humidity Sensor**
- **Buzzer** (for alarm notifications)
- **Push Button** (for manual activation)
- **Power Supply 3.3V/5V** (USB or battery)

## 🎯 Expected Results
- The system continuously monitors smoke, gas, temperature, and motion.
- If a fire is detected, the **buzzer** is triggered and data is sent to the **server**.
- The **web dashboard** displays real-time sensor values.

