# Blinky Board - 555 Chaser

## Description

The Blinky Board is an LED chaser circuit designed for the Stasis High School Hardware Hackathon. It uses a NE555 timer and a CD4017 decade counter to light eight LEDs in sequence.

## Features

* 8 sequential LEDs
* Adjustable speed using a 50k potentiometer
* Custom PCB designed in KiCad
* Simple through-hole components

## How It Works

The NE555 timer generates clock pulses that are sent to the CD4017 counter. Each pulse advances the active output, causing the LEDs to light up one after another and creating a chasing effect.

## Components

* NE555P timer IC
* CD4017BE decade counter
* 8 LEDs
* Resistors
* Capacitors
* 50k potentiometer
* Pin headers

A complete bill of materials with prices and links can be found in `bom.csv`.


<img width="1174" height="701" alt="Screenshot_3D_View" src="https://github.com/user-attachments/assets/64ede4fa-df68-4c70-adb9-212a4db76818" />

