# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT5 |
| **DATE** | 13/08/2026 |
| **NAME OF EXP** | Timer-Based LED Fading Using Software PWM |
| **HARDWARE SETUP / PLATFORM** | AT89S52; Timer 0; LED on P3.1 through 330 Ω; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASK5B |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware varies timer-controlled LED on/off intervals to create a software PWM fading effect. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware varies timer-controlled LED on/off intervals to create a software PWM fading effect.

### Core Logic
1. The firmware varies timer-controlled LED on/off intervals to create a software PWM fading effect.

### Project Files
- `PWM.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `pwm.c`

### Hardware Connections
- P3.1 drives the LED through a 330 Ω resistor.
- The diagram shows an 11.0592 MHz crystal with 33 pF capacitors.
- AT89S52 uses +5 V and ground.


---

## Inference

The program is intended to vary LED brightness by changing the software PWM duty cycle.

