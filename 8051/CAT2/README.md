# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT2 |
| **DATE** | 23/07/2026 |
| **NAME OF EXP** | Bare-Metal LED Blinking Using the 8051 Microcontroller |
| **HARDWARE SETUP / PLATFORM** | 8051-family MCU; Keil project selects AT89S52 while the diagram labels AT89C51; P1.7 LED and 330 Ω resistor; 11.0592 MHz crystal; +5 V and reset network. |
| **TASK NO** | Not specified |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware alternates P1.7 high and low with a nested-loop software delay. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware alternates P1.7 high and low with a nested-loop software delay.

### Core Logic
1. The firmware alternates P1.7 high and low with a nested-loop software delay.

### Project Files
- `Day 1.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `led.c`

### Hardware Connections
- P1.7 drives the LED through 330 Ω.
- The diagram shows an 11.0592 MHz crystal, 33 pF capacitors, +5 V, ground, and a 10 µF/10 kΩ reset network.
- The project selects AT89S52 but the diagram labels AT89C51; confirm the board model.


---

## Inference

The source is intended to blink the P1.7 LED. Project and diagram specify different MCU models.

