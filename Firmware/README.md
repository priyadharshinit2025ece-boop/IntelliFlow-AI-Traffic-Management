# Firmware Documentation

## Overview

The firmware is responsible for controlling the traffic junction using the ESP32 microcontroller. It collects traffic data from sensors, communicates with neighboring intersections, exchanges data with the cloud, and controls the traffic lights based on optimized signal timings.

---

## Responsibilities

- Read data from Ultrasonic and IR sensors
- Calculate vehicle density
- Estimate queue length
- Communicate with nearby intersections using ESP-NOW
- Publish traffic data to the cloud using MQTT
- Receive optimized signal timing recommendations
- Control Red, Yellow, and Green traffic signals
- Handle Emergency Vehicle Priority Override

---

## Planned Firmware Modules

### Sensor Module
- Read Ultrasonic Sensor
- Read IR Sensor
- Filter noisy sensor readings

### Traffic Analysis Module
- Calculate vehicle density
- Estimate queue length
- Determine local traffic conditions

### Communication Module
- ESP-NOW communication
- MQTT communication
- Wi-Fi connection management

### Traffic Signal Controller
- Green signal control
- Yellow signal timing
- Red signal timing
- Safety timing validation

### Emergency Mode
- Detect emergency vehicle signal
- Temporarily override normal traffic operation
- Resume density-based control after emergency clearance

---

## Communication Flow

Sensors

↓

ESP32

↓

Neighboring Junctions (ESP-NOW)

↓

Firebase Cloud (MQTT)

↓

AI Recommendation

↓

Traffic Signal Controller

---

## Current Status

- System architecture completed
- Firmware design in progress
- Implementation in progress

---

## Future Improvements

- Camera integration
- Edge AI processing
- OTA firmware updates
- Sensor fault detection
