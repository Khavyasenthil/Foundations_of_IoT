# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT4 |
| **DATE** | 06/08/2026 |
| **NAME OF EXP** | Keypad-Based LED Control and Seven-Segment Display |
| **HARDWARE SETUP / PLATFORM** | AT89S52; 4×4 keypad; four LEDs; seven-segment display; +5 V. |
| **TASK NO** | Not specified |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware scans the keypad, selects LED patterns, and decodes keypad values for seven-segment display. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware scans the keypad, selects LED patterns, and decodes keypad values for seven-segment display.

### Core Logic
1. The firmware scans the keypad, selects LED patterns, and decodes keypad values for seven-segment display.

### Project Files
- `STARTUP.A51`
- `blabla.c`
- `firmware.hex`
- `seven_segment.uvproj`

### Hardware Connections
- Keypad rows and columns connect to P2.0–P2.7.
- Four LED outputs use P1.0–P1.3 with 330 Ω resistors.
- Seven-segment lines connect to Port 0 through 330 Ω resistors; common is shown grounded.
- AT89S52 powered from +5 V with ground.


---

## Inference

The program combines keypad input, LED patterns, and hexadecimal digit display.

