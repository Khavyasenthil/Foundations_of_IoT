# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT7 |
| **DATE** | 27/08/2026 |
| **NAME OF EXP** | LCD Character Movement with a 4×4 Keypad |
| **HARDWARE SETUP / PLATFORM** | AT89S52; 16×2 LCD in 4-bit mode; 4×4 keypad; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASKC |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware scans the keypad and moves an asterisk on the LCD: 2/up, 8/down, 4/left, 6/right. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware scans the keypad and moves an asterisk on the LCD: 2/up, 8/down, 4/left, 6/right.

### Core Logic
1. The firmware scans the keypad and moves an asterisk on the LCD: 2/up, 8/down, 4/left, 6/right.

### Project Files
- `DAY6TASK1.uvproj`
- `LCD.c`
- `STARTUP.A51`
- `delay.c`
- `firmware.hex`
- `keypad.c`

### Hardware Connections
- Keypad rows connect to P2.7–P2.4 and columns to P2.3–P2.0.
- LCD RS=P3.2, E=P3.3, and D4–D7=P3.4–P3.7.
- AT89S52 uses +5 V and common ground.
- The archive omits the referenced `delay.h` and `keypad.h` headers.


---

## Inference

The program intends to move an asterisk using keypad direction keys; the source references two header files absent from the archive.

