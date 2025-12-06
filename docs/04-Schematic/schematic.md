---
title: Schematic
---

## Overview

**Schematic Overview — Humidity & Temperature Subsystem**

The schematic depicts the complete electrical design of the Humidity & Temperature Subsystem, showing how power, sensing, buffering, and digital communication are integrated.

A linear voltage regulator (LM7805T) provides a stable 5 V supply to all components within the subsystem, including the SHT31-ARP-B sensor, MCP6004 operational amplifier, Microchip PIC18F57Q43 Curiosity Nano, red LED, and debug pushbutton circuit.

*Sensor & Signal Amplification*

The SHT31-ARP-B sensor outputs two analog signals:

- Relative Humidity (RH) signal

- Temperature (T) signal

Each signal is routed through the MCP6004’s op-amp channels, configured as as two non-inverting amplifiers (Gain ≈ 1.2) to condition SHT31-ARP-B-Temperature & Humidity signals around a 2.5V mid-supply reference for 0-5 V ADC use.Expected outputs: Temp ≈ 0.44-4.7 V, RH ≈ 0.1-4.9 V from inputs 0.77-4.34 V and 0.5-4.5 V respectively.

*Microcontroller Interface*

Buffered signals are fed into the PIC18F57Q43 via its analog input pins:

- RA0 (ADC1) → Humidity signal input

- RA1 (ADC1) → Temperature signal input

The microcontroller continuously monitors these readings.
If the humidity exceeds a preset threshold (indicating a potential water leak), the firmware outputs a digital HIGH signal from RD5/RD7, routed to pin 3 of the team connector, which communicates with the alarm subsystem to activate the speaker.

*Indicators & Debug Features*

- A red LED, driven by PWM pin RF4, serves as a visual alert or status indicator.

- A pushbutton debug circuit provides manual input testing for system verification.

*Power Distribution*

All components operate from the regulated 5 V rail supplied by the LM7805T.
Decoupling capacitors are included near key ICs to reduce noise and allow stable analog readings.

![schematic](SCHEMF.png){style width:"350" height:"300;"}

## Resouces

The schematic as a PDF download is available [*here*](CGE_Subsystem.pdf), and the Zip folder of the project [*here*](CGE_Subsystem.zip).
