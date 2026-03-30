# TempGuard - Analog DC Temperature Control Module
**(純類比直流溫控模組)**

[![Hardware License](https://img.shields.io/badge/Hardware%20License-CERN--OHL--S%20v2.0-blue.svg)](LICENSE-HARDWARE.txt)
[![Doc License](https://img.shields.io/badge/Doc%20License-CC%20BY--SA%204.0-green.svg)](LICENSE-DOCS.txt)

## 📌 Project Overview (專案簡介)
TempGuard is an industrial-grade, pure analog DC temperature control module designed for auxiliary temperature regulation. It operates entirely without microcontrollers (MCU) or firmware, ensuring zero risk of system crashes and high resistance to electromagnetic interference. 

TempGuard 是一款專為工控系統設計的純類比直流溫控輔助模組 。採用無 MCU、無韌體的純類比電路架構，確保永不死機，並具備極高的抗干擾能力 。

## 🛡️ Hardware Advantages & Safety (硬體優勢與安全性)
* **No Software Overhead (零軟體負擔):** Pure analog circuit on FR4 PCB. No coding or debugging required.
* **Flame Retardant (最高阻燃標準):** The enclosure is made of UL94 V-0 flame-retardant ABS/PC.
* **Environmental Protection (環境防護):** IP54 rating (when the case is closed), providing reliable protection against dust ingress and water splashes.
* **Derating Design (主動降額設計):** Utilizes a 10A Songle relay, actively derated to a 2.5A continuous load to maximize mechanical lifespan (>50,000 cycles).
* **Smart Hysteresis (智慧回差):** Built-in 5.2~8.0°C hysteresis to prevent frequent relay toggling near the target temperature.

## ⚙️ Core Specifications (技術規格)
| Specification (項目) | Details (規格) |
| :--- | :--- |
| **Control Range (控溫範圍)** | 10~69°C (Adjustable via potentiometer)  |
| **Power Input (輸入電源)** | 12V DC Only (Strictly NO AC)  |
| **Output (輸出規格)** | 0~30V DC / Continuous 2.5A Max  |
| **Relay Type (繼電器接點)** | SPDT (NO / NC / COM)  |

## 🔌 Wiring & Applications (接線與應用)
*(Note: Please insert your diagram images here / 請在此處插入您的接線圖)*
* **Cooling Mode (高溫散熱):** Connect to `COM` + `NO`. Relay conducts when Temp > Setpoint.
* **Heating/Protection Mode (低溫加熱/高溫保護):** Connect to `COM` + `NC`. Relay disconnects when Temp > Setpoint.

## 📜 Certifications & Open Source Licenses (認證與開源授權)
This project embraces the open-source hardware philosophy:
* **Hardware Design:** [CERN-OHL-S v2.0](LICENSE-HARDWARE.txt) 
* **Documentation & Images:** [CC BY-SA 4.0](LICENSE-DOCS.txt) 
Original Design by: **TSAI, AN-HSIANG (2026)** 
