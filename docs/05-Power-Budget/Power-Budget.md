---
title: Power Budget
---

## Overview

![Power Budget](UPBD1.png){style width:"350" height:"300;"}

## Conclusion

The power budget shows the +5 V rail needs about 675.25 mA with a 25% safety margin included. That’s well under the LM7805T’s 1.5 A rating, so the regulator can comfortably power everything without hitting thermal or electrical limits.

I chose a 9 V, 3 A wall adapter, which provides plenty of headroom for regulator dropout and conversion losses. That leaves spare current for stable operation and future expansion.
All major active parts : SHT31-ARP-B sensor, MCP6004 op amp, PIC18F57Q43 Curiosity Nano, and the LED load — are within their voltage and current specs and are all tied to the +5 V rail to keep the design simple.

In short: the power system has healthy margins, clean rail assignments, and appropriate regulation and supply choices. It’s electrically sound and ready for implementation.


## Resouces

The power budget as a PDF download is available [*here*](FPB1.pdf), and a Microsoft Excel Sheet [*here*](UPB1.xlsx).
