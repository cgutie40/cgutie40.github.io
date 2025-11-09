---
title: Schematic
---

## Overview

**Schematic Overview — Humidity & Temperature Subsystem**

The schematic depicts the complete electrical design of the Humidity & Temperature Subsystem, showing how power, sensing, buffering, and digital communication are integrated.

A linear voltage regulator (LM7805T) provides a stable 5 V supply to all components within the subsystem, including the SHT31-ARP-B sensor, MCP6004 operational amplifier, Microchip PIC18F57Q43 Curiosity Nano, red LED, and debug pushbutton circuit.

*Sensor & Signal Buffering*

The SHT31-ARP-B sensor outputs two analog signals:

- Relative Humidity (RH) signal

- Temperature (T) signal

Each signal is routed through one of the MCP6004’s op-amp channels, configured as unity-gain voltage followers (buffers).
These buffers provide signal isolation and stability, making sure the sensor outputs are not affected by the input impedance of the microcontroller’s ADC.

*Microcontroller Interface*

Buffered signals are fed into the PIC18F57Q43 via its analog input pins:

- RA0 (ADC1) → Temperature signal input

- RA1 (ADC1) → Humidity signal input

The microcontroller continuously monitors these readings.
If the humidity exceeds a preset threshold (indicating a potential water leak), the firmware outputs a digital HIGH signal from RD5/RD7, routed to pin 3 of the team connector, which communicates with the alarm subsystem to activate the speaker.

*Indicators & Debug Features*

- A red LED, driven by PWM pin RF4, serves as a visual alert or status indicator.

- A pushbutton debug circuit provides manual input testing for system verification.

*Power Distribution*

All components operate from the regulated 5 V rail supplied by the LM7805T.
Decoupling capacitors are included near key ICs to reduce noise and allow stable analog readings.

![schematic](UpdatedCGEschem.png){style width:"350" height:"300;"}

## Resouces

The schematic as a PDF download is available [*here*](CGE_Subsystem%20(1).pdf), and the Zip folder of the project [*here*](Updated_CGE_Subsystem.zip).
