# Smart Home Automation System

A Wi-Fi-based Smart Home Automation System built using ESP32, enabling users to control and monitor home appliances through a web interface without requiring an external router. The ESP32 acts as a standalone hotspot and web server, providing real-time device control, status monitoring, and customizable device management.

## Features

### Device Control

* Control up to four connected appliances using ESP32 GPIO pins.
* Real-time ON/OFF switching through a responsive web interface.
* Instant status synchronization across connected clients.

### Wi-Fi Hotspot Mode

* ESP32 operates as a standalone Wi-Fi Access Point.
* No internet connection or external router required.
* Custom SSID and password configuration.

### Real-Time Updates

* Live device status updates using Server-Sent Events (SSE).
* Immediate synchronization of device states across connected users.

### Device Customization

* Rename connected switches/appliances dynamically.
* Device names are stored permanently in ESP32 memory.

### Device Discovery

* Automatic ESP32 discovery using UDP communication.
* Simplifies connection and setup for client applications.

### Persistent Storage

* Stores Wi-Fi credentials and device names using ESP32 Preferences.
* Retains settings even after power cycles.

### Connection Monitoring

* Detects connected clients in real time.
* LED status indicator shows network connectivity state.

## Technology Stack

* ESP32
* Arduino Framework
* ESPAsyncWebServer
* AsyncTCP
* WiFiUDP
* Preferences Library
* HTML/CSS/JavaScript

## System Architecture

ESP32 hosts a local web server and Wi-Fi hotspot. Users connect directly to the hotspot and access the control dashboard through a browser. Commands are sent via HTTP requests, while real-time status updates are delivered through Server-Sent Events (SSE).

## Project Structure

```text
├── ESP32 Firmware
│   ├── Device Control Logic
│   ├── UDP Discovery Service
│   ├── Web Server APIs
│   ├── Preferences Storage
│   └── Event Streaming
│
├── Web Dashboard
│   ├── Device Controls
│   ├── Status Monitoring
│   ├── Device Naming
│   └── Network Configuration
```

## Applications

* Smart Lighting Control
* Home Appliance Automation
* Smart Office Systems
* IoT Learning Projects
* Local Network Automation Solutions

## Future Enhancements

* Mobile Application Integration
* Voice Assistant Support
* MQTT Connectivity
* Energy Consumption Monitoring
* Scheduling and Automation Rules
* Cloud Synchronization

## Author

Chandan Deshani
B.Tech Computer Engineering | AI & IoT Enthusiast
