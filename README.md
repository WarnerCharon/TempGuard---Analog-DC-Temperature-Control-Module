# TempGuard - Analog DC Temperature Control Module
**(純類比直流溫控模組)**

[![Hardware License](https://img.shields.io/badge/Hardware%20License-CERN--OHL--S%20v2.0-blue.svg)](LICENSE-HARDWARE.txt)
[![Doc License](https://img.shields.io/badge/Doc%20License-CC%20BY--SA%204.0-green.svg)](LICENSE-DOCS.txt)

## 📌 Project Overview (專案簡介)
[cite_start]TempGuard is an industrial-grade, pure analog DC temperature control module designed for auxiliary temperature regulation[cite: 7]. [cite_start]It operates entirely without microcontrollers (MCU) or firmware, ensuring zero risk of system crashes and high resistance to electromagnetic interference. 

[cite_start]TempGuard 是一款專為工控系統設計的純類比直流溫控輔助模組 [cite: 7][cite_start]。採用無 MCU、無韌體的純類比電路架構，確保永不死機，並具備極高的抗干擾能力 。

## 🛡️ Hardware Advantages & Safety (硬體優勢與安全性)
* **No Software Overhead (零軟體負擔):** Pure analog circuit on FR4 PCB. [cite_start]No coding or debugging required.
* [cite_start]**Flame Retardant (最高阻燃標準):** The enclosure is made of UL94 V-0 flame-retardant ABS/PC.
* [cite_start]**Environmental Protection (環境防護):** IP54 rating (when the case is closed), providing reliable protection against dust ingress and water splashes.
* [cite_start]**Derating Design (主動降額設計):** Utilizes a 10A Songle relay, actively derated to a 2.5A continuous load to maximize mechanical lifespan (>50,000 cycles)[cite: 10, 16].
* [cite_start]**Smart Hysteresis (智慧回差):** Built-in 5.2~8.0°C hysteresis to prevent frequent relay toggling near the target temperature.

## ⚙️ Core Specifications (技術規格)
| Specification (項目) | Details (規格) |
| :--- | :--- |
| **Control Range (控溫範圍)** | [cite_start]10~69°C (Adjustable via potentiometer)  |
| **Power Input (輸入電源)** | [cite_start]12V DC Only (Strictly NO AC) [cite: 9, 16] |
| **Output (輸出規格)** | [cite_start]0~30V DC / Continuous 2.5A Max  |
| **Relay Type (繼電器接點)** | [cite_start]SPDT (NO / NC / COM)  |

## 🔌 Wiring & Applications (接線與應用)
*(Note: Please insert your diagram images here / 請在此處插入您的接線圖)*
* **Cooling Mode (高溫散熱):** Connect to `COM` + `NO`. [cite_start]Relay conducts when Temp > Setpoint[cite: 20].
* **Heating/Protection Mode (低溫加熱/高溫保護):** Connect to `COM` + `NC`. [cite_start]Relay disconnects when Temp > Setpoint[cite: 20].

## 📜 Certifications & Open Source Licenses (認證與開源授權)
[cite_start]This project embraces the open-source hardware philosophy[cite: 161, 162]:
* [cite_start]**Hardware Design:** [CERN-OHL-S v2.0](LICENSE-HARDWARE.txt) [cite: 159, 162]
* [cite_start]**Documentation & Images:** [CC BY-SA 4.0](LICENSE-DOCS.txt) [cite: 178, 179]
[cite_start]Original Design by: **TSAI, AN-HSIANG (2026)** [cite: 17, 153]
