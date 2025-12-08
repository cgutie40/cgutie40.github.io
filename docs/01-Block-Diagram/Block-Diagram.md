---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview of Block Diagram

This block diagram shows the Humidity and Temperature Subsystem, which supports two key product requirements:

- **Requirement 2:** Detect water leaks within the device’s area.  
- **Requirement 3:** Measure the temperature of the surrounding environment or water.

---

## Voltage Regulator (LM7805T)

The LM7805T provides a stable 5 V supply to the sensor and microcontroller.

**Requirement support:** Stable power allows accurate humidity and temperature readings needed for leak detection (Req. 2) and temperature measurement (Req. 3).

---

## Humidity & Temperature Sensor (SHT31)

The SHT31 outputs analog humidity and temperature signals.

**Requirement support:**  
- Humidity increases indicate possible water leaks (Req. 2).  
- Temperature output allows the system to measure water/air temperature (Req. 3).

---

## Microcontroller (PIC18F57Q43)

The MCU reads the sensor signals using its ADC. If humidity exceeds a threshold, it sends a digital leak alert to the alarm subsystem.

**Requirement support:**  
- Performs leak detection logic and triggers alarms (Req. 2).  
- Converts temperature readings to Fahrenheit (Req. 3).

---

## Team Connector

Carries the digital leak alert and sensor data to the main subsystem.

**Requirement support:** Provides communication needed for leak detection and temperature reporting.

---

## Debug Components (LED + Pushbutton)

Used for testing sensor readings and verifying alarm behavior.

**Requirement support:** Helps validate that the subsystem meets Requirements 2 and 3.

---

![Block Diagram](BOMUPD1.png)
