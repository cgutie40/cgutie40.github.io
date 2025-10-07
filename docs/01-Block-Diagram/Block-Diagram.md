---
title: Individal Block Diagram
tags:
- tag1
- tag2
---
## Overview of Block Diagram

This block diagram shows how the water leak detection system is put together, including power, sensors, actuators, and team connections. It helps explain how everything communicates with the PIC18F57Q43 and how power flows through the system.

### Purpose
The diagram is meant to make it clear how each component works together, how sensors and actuators connect, and how team member modules interface with the system. It’s a quick reference for building, testing, and understanding the project.

### Power
- **Battery:** 9 V  
- **Voltage Regulation:** 3.3 V Buck switching regulator (`MP2307DN-LF-Z`) to supply the PIC, sensors, OLED, and LED  
- **Battery Monitoring:** `VOLT-01` module tracks battery life  
- **Indicators:** Red LED lights up if there’s a problem  

### Sensors
- **Analog:** Water pressure sensor from a team member on pin 6  
- **Digital:** Moisture sensor from a team member on pin 1  

### Actuators
- **Speaker:** From a team member on pin 2  
- **Red LED:** Local indicator for system status  

### Display
- **OLED Screen:** `IPBOLD-96`, connected via I²C, shows battery life and system status  

### Team Connections
- Signals from other team members include analog and digital inputs/outputs. The block diagram shows which microcontroller pins each connection uses so everything integrates smoothly.


![Block Diagram](Images/Cristopher_G_Team_208_INDV.drawio (1).png)
