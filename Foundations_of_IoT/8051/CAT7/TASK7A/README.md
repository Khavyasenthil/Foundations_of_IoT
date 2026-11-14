# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT7 |
| **DATE** | 27/08/2026 |
| **NAME OF EXP** | 16×2 LCD Initialization and Character Display |
| **HARDWARE SETUP / PLATFORM** | AT89S52; HD44780-compatible 16×2 LCD in 4-bit mode; contrast potentiometer; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASK7A |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware initializes the LCD using Port 3 control/data pins and writes character data. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware initializes the LCD using Port 3 control/data pins and writes character data.

### Core Logic
1. The firmware initializes the LCD using Port 3 control/data pins and writes character data.

### Project Files
- `LCD.c`
- `Lab 7.uvproj`
- `STARTUP.A51`
- `firmware.hex`

### Hardware Connections
- LCD RS=P3.2, E=P3.3, and D4–D7=P3.4–P3.7.
- Contrast uses a 10 kΩ potentiometer; connect LCD power and ground as shown.
- AT89S52 uses +5 V and ground.


---

## Inference

The code demonstrates LCD initialization and character output using a 4-bit interface.

