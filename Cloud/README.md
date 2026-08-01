# Cloud Module Documentation

## Overview

The cloud platform serves as the central communication and monitoring system for IntelliFlow.

It stores traffic information, enables AI processing, synchronizes multiple intersections, and provides a dashboard for real-time monitoring.

---

## Responsibilities

- Store traffic information
- Maintain historical traffic records
- Receive MQTT messages
- Share data with AI module
- Send optimized recommendations to ESP32 controllers
- Provide monitoring dashboard

---

## Cloud Platform

- Firebase

---

## Communication Protocol

### MQTT

Purpose

- Publish traffic information
- Subscribe to AI recommendations
- Real-time communication

---

## Data Stored

Each traffic junction uploads:

- Junction ID
- Vehicle density
- Queue length
- Waiting time
- Signal status
- Timestamp

---

## Dashboard Features

- Live traffic density
- Signal status
- Historical traffic trends
- AI recommendations
- Junction monitoring

---

## Cloud Workflow

ESP32

↓

MQTT

↓

Firebase

↓

AI Processing

↓

Optimized Signal Recommendation

↓

ESP32

---

## Future Improvements

- City-wide deployment
- Multi-user dashboard
- Traffic analytics
- Cloud alerts
- Mobile application

---
