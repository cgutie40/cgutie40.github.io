---
title: Welcome 
tags:
- tag1
- tag2
---
<center>
<font size= "6">(Cristopher Gutierrez) Datasheet</font><br>
as part of<br>
<font size= "8">Water Detector System: Humidity & Temperature Sensor</font><br>
for<br>
<font size= "5"> Team 208 </font><br>

**Submission: December, 08, 2025**
</center>

## Introduction

This system is designed to detect potential water leaks using three specialized sensors : pressure, water puddle, and humidity. Each sensor subsystem works together to ensure early and reliable detection of leaks.

My subsystem focuses exclusively on humidity and temperature measurement, providing crucial environmental data that helps identify leaks before they cause damage.

### Project Summary

The overall Water Leak Detection System integrates multiple sensing technologies connected to a PIC18F57Q43 microcontroller. The complete system monitors changes in pressure, the presence of standing water, and fluctuations in humidity and temperature. When abnormal readings are detected, the system triggers an audible alarm to alert the user.

A comprehensive Team Block Diagram is included to illustrate how each subsystem interacts — showing data and power flow between the sensors, the microcontroller, and the alarm output. This diagram highlights the communication paths and power distribution throughout the design.

[Team Block Diagram](https://asu-egr304-2025-f-208.github.io/ASU-EGR-304-Team-208/06-team-block-diagram/)


### My Contribution

My subsystem uses the SHT31-ARP-B sensor to continuously measure humidity and temperature. When the humidity exceeds a set threshold (indicating a possible water leak), the sensor outputs a digital signal to the main subsystem, which then activates an alarm speaker.

Within this datasheet, I document the following sections related to my work:

- Component Selection: Comparison of potential sensor options, including pros and cons, reference links, part numbers, costs, and visual aids — culminating in my final component choice and rationale.

- Schematic: A detailed circuit diagram illustrating the electrical connections of the humidity and temperature sensor with the system.

- Power Budget: Analysis of supply voltage and current consumption, including power drawn by major components, voltage regulator efficiency, and overall power source considerations.

- Bill of Materials (BOM): This section will provide a comprehensive list of all components used.
