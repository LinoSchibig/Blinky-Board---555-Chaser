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

## Schematic

### Schematic
<img width="1343" height="925" alt="Screenshot 2026-06-28 221641" src="https://github.com/user-attachments/assets/9aadf022-bb48-4322-bf45-ea1c14272e14" />
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
