# Blinky Board - 555 Chaser

## Description
The Blinky Board is an LED chaser circuit developed for the Stasis High School Hardware Hackathon. It is based on a classic NE555 timer and CD4017 decade counter combination, creating a sequential LED animation effect.

This project was chosen as a way to understand fundamental digital electronics and timing circuits through a hands-on PCB design process.

---

## Features
- 8 sequential LEDs forming a chasing light pattern  
- Adjustable speed using a 50k potentiometer  
- Fully custom PCB designed in KiCad  
- Simple through-hole construction for easy assembly and debugging  

---

## How It Works
The NE555 timer operates in astable mode and generates a continuous square wave clock signal. This signal is fed into the CD4017 decade counter, which advances one output per pulse.

Each output activates a corresponding LED, creating a visible "running light" effect. The speed of the sequence can be controlled by adjusting the potentiometer, which changes the timing of the 555 oscillator.

---

## Why I Built This Project
I started this project to move beyond theoretical electronics and actually understand how timing circuits and counters behave in real hardware.

I also wanted to learn how a full PCB design workflow works, from schematic creation to layout and production files.

---

## Difficulties
- Understanding the correct wiring between the NE555 and CD4017 was initially confusing  
- Debugging LED behavior when outputs didn’t match expected sequence  
- Managing PCB layout constraints while keeping signal paths clean  
- Fixing incorrect timing values caused by miscalculating capacitor/resistor combinations  

---

## What I Learned
- How an astable 555 timer generates clock signals  
- How a CD4017 decade counter sequences outputs  
- Basic PCB design principles in KiCad  
- Importance of correct grounding and stable power routing  
- How small component value changes affect timing behavior significantly  

---

## Schematics & PCB Design

### Schematic
![Schematic](schematic.png)

### PCB Layout
![PCB Layout](pcb.png)

---

## Bill of Materials (BOM)

| Component | Quantity | Supplier | Link |
|----------|----------|----------|------|
| NE555P Timer IC | 1 | DigiKey | https://www.digikey.com/en/products/detail/texas-instruments/NE555P/ |
| CD4017BE Counter | 1 | DigiKey | https://www.digikey.com/en/products/detail/texas-instruments/CD4017BE/ |
| LED (5mm) | 8 | Mouser | https://www.mouser.com/ |
| Resistors (assorted) | ~10 | Local / DigiKey | https://www.digikey.com/ |
| Capacitors | 2–3 | DigiKey | https://www.digikey.com/ |
| 50k Potentiometer | 1 | DigiKey | https://www.digikey.com/ |
| Pin Headers | 1 set | AliExpress / Mouser | https://www.mouser.com/ |

---

## Notes
All PCB fabrication files (Gerber ZIP) are included in the repository under `/pcb/production_files/`.
