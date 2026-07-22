# BMI088 Custom Breakout Board

<img width="449" height="237" alt="IMG_5351(1)" src="https://github.com/user-attachments/assets/ebdc03cc-5f4d-4d3a-94fc-7fca6bcbc01c" />

## Design Overview:
Designed as a first PCB layout project and hand-assembled via hotplate reflow. Built to test IMU functionality and to integrate into a thrust vector control (TVC) gimbal control loop. Existing domestic BMI088 breakouts either require expensive application boards to interface with, or expose only I²C. This design breaks out both I²C and SPI, with components selected in part for domestic sourcing and tariff avoidance. Full assembly process shown in link below:

https://youtube.com/shorts/Hh-Zr3-ZTfY?feature=share

- **Schematic:** 

<img width="562" height="397" alt="image" src="https://github.com/user-attachments/assets/096da997-67e0-4f5e-b6a8-ccc31216b62b" />

- **Board layout:** 

<img width="562" height="453" alt="Screenshot from 2026-05-26 21-09-24" src="https://github.com/user-attachments/assets/e29138b0-1996-406f-976a-b0913ec5136f" />

## Features:
- Onboard 3.3V LDO — Vin tolerant from 3.3 V to 6 V
- I²C and SPI accessible via standard 2.54mm pin headers
- Power indicator LED

## Bill of Materials:
| Ref | Package | Part | Qty |
|-----|---------|------|-----|
| U1 | LGA-16 | Bosch BMI088 IMU | 1 |
| U2 | SOT-23 | MCP1700-3302 LDO | 1 |
| C1–C2 | 0402 | 0.1 µF | 2 |
| C3–C4 | 0603 | 0.1 µF | 2 |
| R1–R2 | 0603 | 4.7 kΩ (I²C pull-ups) | 2 |
| R3 | 0603 | 2.2 kΩ | 1 |
| R4 | 0603 | 10 kΩ | 1 |
| D2 | 0603 | LED | 1 |

## Repository Structure:
- `hardware/` — KiCad project files (schematic, PCB layout)
- `gerbers/` — Manufacturing files (Gerbers, drill files) ready to send to a fab
