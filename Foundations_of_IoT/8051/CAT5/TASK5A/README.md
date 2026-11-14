# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT5 |
| **DATE** | 13/08/2026 |
| **NAME OF EXP** | Timer-Based LED Toggle Using Timer 0 |
| **HARDWARE SETUP / PLATFORM** | AT89S52; Timer 0 in 16-bit mode; LED on P3.1 through 330 Ω; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASK5A |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | Timer 0 overflows are counted. At 600 overflows the firmware toggles the LED on P3.1 and resets the count. |

---

## Core Logic / Pseudocode / Code Base

### Overview
Timer 0 overflows are counted. At 600 overflows the firmware toggles the LED on P3.1 and resets the count.

### Core Logic
1. Timer 0 overflows are counted
2. At 600 overflows the firmware toggles the LED on P3.1 and resets the count.

### Project Files
- `STARTUP.A51`
- `firmware.hex`
- `lab5.uvproj`
- `timer.c`

### Hardware Connections
- P3.1 drives the LED through a 330 Ω resistor.
- The diagram shows an 11.0592 MHz crystal and 30 pF capacitors.
- AT89S52 uses +5 V and ground.


---

## Inference

Timer overflow counting provides the delay for blinking the P3.1 LED.

