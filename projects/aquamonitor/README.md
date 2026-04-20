# AquaMonitor: Smart Water Management System

## Project Overview
**AquaMonitor** is an intelligent, IoT-enabled water monitoring and management system designed to optimize water usage and ensure water safety. The system uses an ESP32 microcontroller to interface with various sensors and provides real-time data to a cloud-based dashboard.

### Key Objectives
- **Conservation:** Minimize water waste through precise measurement and leak detection.
- **Safety:** Monitor water quality parameters like pH and Turbidity.
- **Automation:** Automatically manage water pumps based on tank levels to prevent dry-running or overflows.

## System Architecture

### Hardware Components
1. **Microcontroller:** ESP32 (for Wi-Fi connectivity and dual-core processing).
2. **Level Sensor:** HC-SR04 Ultrasonic Sensor (non-contact distance measurement).
3. **Quality Sensors:** Analog pH Sensor and Turbidity Sensor.
4. **Output Devices:** 16x2 I2C LCD Display, Piezo Buzzer for alerts.
5. **Actuator:** 5V Relay module for pump control.
6. **Power Supply:** 9V DC Adapter or Lithium-Polymer battery with voltage regulation.

### Software Stack
- **Firmware:** Written in C++/Arduino framework.
- **Communication:** MQTT protocol for data transmission.
- **Dashboard:** Node-RED or Adafruit IO for visualization.

## Features
- **Real-time Monitoring:** View water levels and quality on the LCD and remote dashboard.
- **Intelligent Pumping:** Pump activates when water falls below 20% and stops at 95%.
- **Safety Alerts:** Audible and visual alerts if water quality drops below safe thresholds.
- **Historical Data:** Logs consumption patterns over time for analysis.

---
*Developed as part of the AFRETEC Embedded Systems Training.*
