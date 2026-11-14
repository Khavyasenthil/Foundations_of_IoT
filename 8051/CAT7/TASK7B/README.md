# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT7 |
| **DATE** | 27/08/2026 |
| **NAME OF EXP** | 16×2 LCD Counter Display |
| **HARDWARE SETUP / PLATFORM** | AT89S52; HD44780-compatible 16×2 LCD in 4-bit mode; contrast potentiometer; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASKB |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware prints a counter label, updates the second row with an incrementing integer, and wraps after 99999. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware prints a counter label, updates the second row with an incrementing integer, and wraps after 99999.

### Core Logic
1. The firmware prints a counter label, updates the second row with an incrementing integer, and wraps after 99999.

### Project Files
- `CAT7-Task2.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `lab7part2.c`

### Hardware Connections
- LCD RS=P3.2, E=P3.3, and D4–D7=P3.4–P3.7.
- The diagram shows a 10 kΩ contrast potentiometer and LCD power/ground.
- AT89S52 uses +5 V and ground.


---

## Inference

The counter value is intended to update continuously on the LCD.

