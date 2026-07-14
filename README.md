# Blinky Board - 555 Chaser

## Description
The Blinky Board is an LED chaser circuit developed for Stasis. It works with a NE555 timer and CD4017, creating a cicle of LEDs blinking.

I choose this project because it was recommeneded as beginner project

---

## Features
- 8 sequential LEDs forming a chasing light pattern  
- Adjustable speed using a potentiometer  
- Custom PCB designed in KiCad

---

## How It Works
The NE555 timer operates in astable mode and generates a continuous signal. This signal is fed into the CD4017, which gives one output per pulse.

Each output activates a LED, creating a "running light" effect. The speed of the pulse can be controlled by adjusting the potentiometer, which changes the timing of the NE555 timer.

---

## Why I Built This Project
Since quite some time ago, I have been interested in electronics and robotics. I saw an ad on Instagram and thought I should give it a try. I learned how to use Stasis and KiCad and started this recommended beginner project.

---

## Difficulties
- Understanding the correct wiring between the NE555 and CD4017 was confusing   
- Managing PCB layout constraints while keeping signal paths clean   

---

## What I Learned
- Basic PCB design principles in KiCad  
- Importance of correct grounding and stable power routing  

---

## Images

### Schematic
<img width="1343" height="925" alt="Screenshot 2026-06-28 221641" src="https://github.com/user-attachments/assets/9aadf022-bb48-4322-bf45-ea1c14272e14" />

### PCB Design
<img width="1050" height="635" alt="Screenshot 2026-07-14 152624" src="https://github.com/user-attachments/assets/559f7fdb-361f-45d9-beaf-377558cba7a7" />

### 3D-View
<img width="1267" height="796" alt="3D_View_Screenshot" src="https://github.com/user-attachments/assets/f7dab8cc-1e49-41ac-84bb-a4adace358f2" />


---

# BOM (Bill of Materials)

This is the list of components used for the project.

| Description | Reference | Qty | Value | Footprint | Source | Price |
|-------------|-----------|-----|-------|-----------|--------|-------|
| Unpolarized capacitor | C1 | 1 | 0.01 µF | Capacitor_THT:CP_Radial_D5.0mm_P2.00mm | DigiKey | $0.27 |
| Polarized capacitor | C2 | 1 | 1 µF | Capacitor_THT:C_Disc_D7.5mm_W2.5mm_P5.00mm | Distrelec | CHF 4.61 |
| Resistor | R2 | 1 | 470 Ω | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal | DigiKey | $0.10 |
| Resistor | R1 | 1 | 1 kΩ | Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P7.62mm_Horizontal | DigiKey | $0.10 |
| Johnson Counter (10 outputs) | U1 | 1 | CD4017BE | CD4017BE:DIP794W45P254L1969H508Q16 | DigiKey | $1.39 |
| Potentiometer | RV1 | 1 | 50 kΩ | Potentiometer_THT:Potentiometer_Vishay_T93YA_Vertical | DigiKey | $18.78 |
| Generic connector (1x01 socket) | J2 | 1 | Conn_01x01_Socket | Connector_PinHeader_2.54mm:PinHeader_1x01_P2.54mm_Vertical | DigiKey | $6.15 |
| Generic connector (1x02 socket) | J1 | 1 | Conn_01x02_Socket | Connector_PinHeader_2.54mm:PinHeader_1x02_P2.54mm_Vertical | DigiKey | $6.15 |
| Light emitting diode | D1, D2, D4, D5, D6, D7, D9, D10 | 8 | LED | LED_THT:LED_D3.0mm | Conrad | $3.95 |
| Precision Timer (555 compatible) | U2 | 1 | NE555P | Package_DIP:DIP-8_W7.62mm | Reichelt | $0.30 |


---

## Notes
All PCB fabrication files (Gerber ZIP) are included in the repository under `/pcb/production_files/`.
