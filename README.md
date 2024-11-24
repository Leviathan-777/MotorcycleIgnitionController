| Supported Targets | ESP32 | ESP32-C2 | ESP32-C3 | ESP32-S2 | ESP32-S3 |
| ----------------- | ----- | -------- | -------- | -------- | -------- |

# Motorcycle Remote Start and Immobilizer System using ESP32

A project that transforms a classic Honda CB500 motorcycle into a modern, tech-enabled machine by implementing a **remote start system** and an **immobilizer feature** using an ESP32 microcontroller. This system allows users to remotely control their motorcycle via an Android phone and includes advanced security measures.

---

## Features

- **Remote Start System**: Start the motorcycle engine wirelessly using a smartphone.
- **Immobilizer**: Adds an additional layer of security to prevent unauthorized access.
- **Bluetooth Communication**: Enables seamless communication between the Android app and the ESP32.
- **Custom Android App Integration**: Control the system with a dedicated app for a better user experience.
- **Failsafe Design**: Ensures the safety and integrity of the motorcycle's electrical system.
- **Separate Power Source**: Independent power supply for the ESP32 to avoid interference with the motorcycle's main 12V battery.

---

## Technologies Used

- **ESP32-WROOM Microcontroller**: The core of the system, providing GPIO, Bluetooth, and processing capabilities.
- **ESP-IDF Framework**: Used for programming the ESP32 with low-level C APIs.
- **Bluetooth Low Energy (BLE)**: For secure communication with the Android app.
- **Custom PCB Design**: For the final prototype with optimized component layout.
- **Electronic Relays**: To control the ignition and starter circuit.
- **Android App Development**: For remote control and user interface.
- **12V to 5V Buck Converter**: To power additional components.
- **Additional Sensors** (e.g., tilt or impact sensors): For future security enhancements (optional).

---

## Components

- **ESP32-WROOM Module**
- **Relay Modules**
- **Separate Rechargeable Power Source for ESP32**
- **12V to 5V DC-DC Buck Converter**
- **Custom Android App**
- **Prototyping Components**: Breadboard, jumper wires, resistors, etc.

---

## Project Setup

### Hardware Connections

1. **Relay Setup**:
   - Connect relays to the ESP32 GPIO pins to control ignition and starter circuits.
   - Use optocouplers for safety and isolation.

2. **ESP32 Power Supply**:
   - The ESP32 is powered by a separate rechargeable battery.
   - Use a buck converter to step down the voltage to 5V if needed.

3. **Motorcycle Wiring**:
   - Use the wiring diagram to identify and safely tap into ignition, starter, and kill switch circuits.
   - Ensure connections do not interfere with the bike’s normal operation.

4. **Immobilizer**:
   - Use GPIO pins to cut off the ignition circuit when unauthorized access is detected.
