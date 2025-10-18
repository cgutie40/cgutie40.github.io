---
title: Component Selection
---
## Humidity / Temperature Sensors

| Image | Solution (with price) | Pros | Cons | Link to Product |
|-------|-----------------------|------|------|-----------------|
|![SHT31 sensor](option1sensor)  | **SHT31-DIS-F2.5KS — $5.39/unit** | - 2.15–5.5 V voltage range (perfect) <br> - Measures both humidity and temperature <br> - In stock and good delivery time <br> - High accuracy / good stability | - More expensive <br> - Needy with maintenance | [Link to product](https://www.digikey.com/en/products/detail/sensirion-ag/SHT31-DIS-F2-5KS/6212134) |
|  [BMP384 sensor](option2sensor)  | **BMP384 — $3.35/unit** | - Low power consumption <br> - Compact package | - Primarily designed for drones <br> - Some features not a primary focus for the product in development | [Link to product](https://www.digikey.com/en/products/detail/bosch-sensortec/BMP388/8322638) |
| [MPR121QR2 sensor](option3sensor) | **MPR121QR2 — $0.59/unit** | - Multiple channels (supports up to 12 electrodes) <br> - Sleep/standby modes | - Comes in bulk orders only <br> - Limited availability | [Link to product](https://www.digikey.com/en/products/detail/nxp-usa-inc/MPR121QR2/2186527) |

**Choice:** Option 1 — SHT31-DIS-F2.5KS  
**Rationale:** This sensor best matches the project requirements. Despite its higher cost, it offers high accuracy, excellent stability, and dual humidity/temperature readings that provide valuable user data.

---

## Voltage Regulator

| Image | Solution (with price) | Pros | Cons | Link to Product |
|-------|-----------------------|------|------|-----------------|
|  | **TPS63030DSKR — $2.14/unit** | - Recommended for 2–3 AA battery-powered designs <br> - Well-documented buck-boost solution | - More layout parts than some alternatives <br> - Layout could become bulky | [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TPS63030DSKR/1972182) |
|  | **ISL9120IRTAZ-T7A — $2.44/unit** | - Very compact <br> - Fewer layout parts needed | - Smaller size makes soldering more difficult | [Link to product](https://www.digikey.com/en/products/detail/renesas-electronics-corporation/ISL9120IRTAZ-T7A/6097375) |
|  | **RT5707 / RT5707A — $1.15/unit** | - Efficient buck converter <br> - Low quiescent current (preserves battery life in sleep) | - No buck-boost (fails if VIN < VOUT) <br> - Voltage range limited vs others | [Link to product](https://www.richtek.com/Products/Switching%20Regulators/DC_DC%20StepDown%20Convertor/RT5707RT5707A) |

**Choice:** Option 1 — TPS63030DSKR  
**Rationale:** Well-suited for a three-AA-battery design. It meets the system’s power requirements and offers strong efficiency at a reasonable price, despite requiring a slightly larger layout.

---

## OLED Screen

| Image | Solution (with price) | Pros | Cons | Link to Product |
|-------|-----------------------|------|------|-----------------|
|  | **DIY0141 0.96 Inch OLED Display Blue/Yellow — $9.99 (2 units)** | - I²C connectivity (compatible with PIC) <br> - Fastest delivery (2 days) <br> - Good deal (comes with 2 units) <br> - 3.3–5 V Voltage <br> - 2 colors | - Slightly bulky compared to other OLEDs | [Link to product](https://www.amazon.com/Wishiot-Display-Self-Luminous-Compatible-Raspberry/dp/B0D1CCHRHW/ref=sr_1_1_sspa?crid=2NXUX32J4XGK1&dib=eyJ2IjoiMSJ9.02CYgV0cwBlIFXJ_E-oMvKJhf2IDVKqSJf6wUIl6pc1o1ktfPX7DvnlfsZjNUn2SM3TIGEcGFmhTq4kUNLDraTgYCGEBEynDMBXt6dM5piYM8smDrvY5aYvt-exm-0m-qqPOjXBFr_jjbXrJScshKV4DRSBKZoRRCueRJhVRY4Z03Elp_l5JhSnIbpnXRVRxcU4VPJV5mB76Vlx_q7Fy-QsKbz1Z1QjNRGPvmDU2vY4.HsEscKoACkI8M1oaUV_CZpSse_JS1nN4t6LCA4yZDyw&dib_tag=se&keywords=0.96%2Binch%2BOLED%2B128%C3%9764%2BSSD1306%2Bmodule&qid=1760750777&sprefix=0.96%2Binch%2Boled%2B128%2B64%2Bssd1306%2Bmodule%2Caps%2C354&sr=8-1-spons&sp_csd=d2lkZ2V0TmFtZT1zcF9hdGY&th=1) |
|  | **U602602 — $6.99/unit** | - I²C connectivity (compatible with PIC) <br> - 3.3–5 V Voltage | - Longer delivery time <br> - Only one unit per order <br> - Most expensive per unit | [Link to product](https://www.amazon.com/UCTRONICS-SSD1306-Self-Luminous-Display-Raspberry/dp/B072Q2X2LL/ref=pd_ci_mcx_di_int_sccai_cn_d_sccl_1_4/132-4994263-9298217?pd_rd_w=kUFXT&content-id=amzn1.sym.751acc83-5c05-42d0-a15e-303622651e1e&pf_rd_p=751acc83-5c05-42d0-a15e-303622651e1e&pf_rd_r=0GZ11NE4PX3CGZW1R9MR&pd_rd_wg=DGBZr&pd_rd_r=de354205-f6ca-4b5c-83d8-39aae13d9228&pd_rd_i=B072Q2X2LL&psc=1) |
|  | **YELUFT B0FKYVZ9W8 — $15.99 (5 OLEDs) / $8.99 (2 OLEDs)** | - I²C connectivity (compatible with PIC) <br> - 2nd fastest delivery (5 days) <br> - Best deal per unit <br> - 3.3–5 V Voltage | - Slightly longer delivery <br> - Only one color | [Link to product](https://www.amazon.com/dp/B0FKYVZ9W8/ref=sspa_dk_detail_0?pd_rd_i=B0FKYVZ9W8&pd_rd_w=jsBYG&content-id=amzn1.sym.30062d3d-2c31-47f3-af26-55177a669bb5&pf_rd_p=30062d3d-2c31-47f3-af26-55177a669bb5&pf_rd_r=V18EFV1PA1P7MM85NRM4&pd_rd_wg=ILOoQ&pd_rd_r=20971833-a070-408a-8b4f-1221b090edf5&sp_csd=d2lkZ2V0TmFtZT1zcF9kZXRhaWxfdGhlbWF0aWM&th=1) |

**Choice:** Option 3 — YELUFT B0FKYVZ9W8  
**Rationale:** Provides the best value per unit and meets all compatibility needs. Its compact shape saves space, making it the most practical option for this design.

---

## MOSFET

| Image | Solution (with price) | Pros | Cons | Link to Product |
|-------|-----------------------|------|------|-----------------|
|  | **NTR4101PT1G P-CH 20 V 1.8 A SOT23-3 — $0.36/unit** | - Good balance between specs <br> - Easy to solder | - Slightly wider than other MOSFETs | [Link to product](https://www.digikey.com/en/products/detail/onsemi/NTR4101PT1G/687096) |
|  | **BSS84 P-CH 50 V 130 mA SOT23-3 — $0.0798/unit** | - Cheapest option <br> - Can handle up to 50 V (overkill but functional) | - Overspecified for the intended application | [Link to product](https://www.digikey.com/en/products/detail/onsemi/BSS84/244213) |
|  | **DMP3068L-7 P-CH 30 V 3.3 A SOT23 — $0.36/unit** | - High current switch (~700 mW, overkill) | - Bulkier compared to other MOSFETs | [Link to product](https://www.digikey.com/en/products/detail/diodes-incorporated/DMP3068L-7/5223214) |

**Choice:** Option 1 — NTR4101PT1G P-CH 20 V 1.8 A SOT23-3  
**Rationale:** Offers the most balanced performance without excessive current or voltage capacity. Ideal for controlling the OLED’s power consumption efficiently.



