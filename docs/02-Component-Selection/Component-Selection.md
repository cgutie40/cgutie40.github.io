---
title: Component Selection
---

## Humidity / Temperature Sensors

| Image | Solution (Price) | Pros | Cons | Link |
|:------|:-----------------|:-----|:------|:------|
| ![sensor1](sensor1.png) | **SHT31-ARP-B** <br> $4.32/unit | - Fits preferred voltage supply <br> - Parallel measurement of temperature and humidity <br> - Analog Voltage output <br> - Simple application circuit <br> - Sensirion datasheet contains useful application info | - Tiny 2.5mm × 2.5mm <br> - Exposed pads (no actual pins) | [Link to Product](https://www.digikey.com/en/products/detail/sensirion-ag/SHT31-ARP-B/5872251?gclsrc=aw.ds&gad_source=1&gad_campaignid=120565755&gbraid=0AAAAADrbLlghcdkRDNUkNksnhJdizNYYQ&gclid=EAIaIQobChMIyaDUvfXDkAMVNFR_AB1A9gBTEAAYASAAEgIRzPD_BwE) |
| ![sensor2](sensor2.png) | **HDC2080DMBR** <br> $1.94/unit | - Less expensive <br> - Slightly bigger (easier to solder) <br> - Texas Instruments <br> - Good sensor documentation | - I²C output (not introduced in class) <br> - Exposed pads (no actual pins) | [Link to Product](https://www.digikey.com/en/products/detail/texas-instruments/HDC2080DMBR/9692560?_gl=1*18c5c7d*_up*MQ..*_gs*MQ..&gclid=EAIaIQobChMIyaDUvfXDkAMVNFR_AB1A9gBTEAAYASAAEgIRzPD_BwE&gclsrc=aw.ds&gbraid=0AAAAADrbLlghcdkRDNUkNksnhJdizNYYQ) |
| ![sensor3](sensor3.png) | **10142048-32** <br> $2.70/unit | - Fits preferred voltage supply <br> - Analog <br> - Less expensive than SHT31 | - Exposed pads (no actual pins) <br> - Limited datasheet information <br> - Tiny 2.5mm × 2.5mm | [Link to Product](https://www.digikey.com/en/products/detail/te-connectivity-measurement-specialties/10142048-32/15188988) |

**Choice:** `SHT31-ARP-B`  
**Rationale:**  
Despite being relatively costly, Sensirion sensors are known for their excellent reliability and comprehensive documentation, simplifying circuit development. The SHT31 is compact yet precise ; ideal for the environmental conditions expected in our water-leak detection design. Its ability to operate two signal lines simultaneously enables flexibility in end-user applications. The primary purpose of this sensor is to detect humidity changes caused by potential water leaks.

---

## Voltage Regulators

| Image | Solution (Price) | Pros | Cons | Link |
|:------|:-----------------|:-----|:------|:------|
| ![vr1](vr1.png) | **LM7805T** <br> $0.33 (100-unit qty) | - Readily available in lab <br> - Familiar component <br> - Well-protected <br> - Through-hole pins (easy to solder) | - Limits flexibility for designs outside 5V | [Link to Product](https://www.digikey.com/en/products/detail/taejin/LM7805T/22237260) |
| ![vr2](vr2.png) | **L7805CV** <br> $0.50/unit | - Good alternative if LM7805T unavailable <br> - Through-hole pins (easy to solder) <br> - Protection features | - May require heatsink | [Link to Product](https://www.digikey.com/en/products/detail/stmicroelectronics/L7805CV/585964) |
| ![vr3](vr3.png) | **MC7805CDT** <br> $0.46/unit | - Through-hole pins (easy to solder) <br> - Well-protected <br> - Compact SMT | - Outputs 1A (harder to cool) <br> - Requires large copper area <br> - Current limitations may affect design | [Link to Product](https://www.digikey.com/en/products/detail/onsemi/MC7805CDTRKG/921037) |

**Choice:** `LM7805T`  
**Rationale:**  
The LM7805T is a well-rounded and reliable choice. It offers solid protection features and a through-hole package that’s easy to handle and solder. Though it limits flexibility in voltage options, its performance suits this subsystem’s parameters and is easily replaceable due to local availability.

---

## Operational Amplifiers (Op-Amps)

| Image | Solution (Price) | Pros | Cons | Link |
|:------|:-----------------|:-----|:------|:------|
| ![oa1](oa1.png) | **MCP6004** <br> $0.59/unit | - Readily available in lab <br> - Familiar component <br> - Through-hole pins (easy to solder) <br> - 4 op-amps <br> - Works at 5V | - 1 MHz GBW and modest precision/noise (not ideal for high-bandwidth or precision tasks) | [Link to Product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060) |
| ![oa2](oa2.png) | **AD8694** <br> $4.50/unit | - Precision quad op-amps <br> - Low offset & noise <br> - Best performance for design | - High power consumption <br> - Expensive <br> - Limited stock | [Link to Product](https://www.digikey.com/en/products/detail/analog-devices-inc/AD8694ARZ/998016) |
| ![oa3](oa3.png) | **TLV9164** <br> $2.75/unit | - Good bandwidth (11 MHz) <br> - 4 op-amps <br> - RRIO and wide supply voltage range | - Higher quiescent current <br> - More power consumption than MCP6004 <br> - Larger 14-pin package | [Link to Product](https://www.digikey.com/en/products/detail/texas-instruments/TLV9164IPWR/15856935) |

**Choice:** `MCP6004`  
**Rationale:**  
The MCP6004 offers solid efficiency and availability, making it a practical choice. While not the most precise quad op-amp, it provides excellent performance for low-power signal conditioning near the sensors. Higher-end alternatives offer marginal benefits at significantly higher cost and power usage, making the MCP6004 the most balanced option.






