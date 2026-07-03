# BMI088-BOB

A breakout board for the Bosch BMI088 6-axis IMU (3-axis accelerometer + 3-axis gyroscope) commonly used in drones, robotics, and other 
motion-sensing applications where accuracy and low noise matter. This board breaks out all pads onto standard pin headers.

<img width="449" height="237" alt="IMG_5351(1)" src="https://github.com/user-attachments/assets/ebdc03cc-5f4d-4d3a-94fc-7fca6bcbc01c" />

## Getting Started
1. Clone this repo
2. Open `hardware/BMI088-BOB.kicad_pro` in KiCad to view/edit the design
3. Use the files in `gerbers/` if you just want to order the board as-is
4. Vin is 3.3V to 6V tolerant.  

## Components
-   C1 & C2: [0402] 0.1uF capacitors
-   C3 & C4: [0603] 0.1uF capacitors
-   R1 & R2: [0603] 4.7kOh resistors
-   R3: [0603] 2.2 kOh resistor
-   R4: [0603] 10.0 kOh resistor
-   D2: [0603] LED
-   U1: [LGA-16] BMI088
-   U2: [SOT-23] MCP1700x-330xxTT

## Repository Structure
- `hardware/` — KiCad project files (schematic, PCB layout)
- `gerbers/` — Manufacturing files (Gerbers, drill files) ready to send to a fab
