# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT3 |
| **DATE** | 30/07/2026 |
| **NAME OF EXP** | Four-Mode LED Control with Button Input |
| **HARDWARE SETUP / PLATFORM** | AT89S52; four LEDs on Port 1; button input on Port 2; +5 V. |
| **TASK NO** | Not specified |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The source runs four LED patterns: a moving light, binary count, and two alternating patterns. A Port 2 input advances the selected mode. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The source runs four LED patterns: a moving light, binary count, and two alternating patterns. A Port 2 input advances the selected mode.

### Core Logic
1. The source runs four LED patterns: a moving light, binary count, and two alternating patterns
2. A Port 2 input advances the selected mode.

### Project Files
- `STARTUP.A51`
- `firmware.hex`
- `lab2prog.c`
- `lab2prog.uvproj`

### Hardware Connections
- LEDs are shown on P1.1–P1.4 through 330 Ω resistors.
- The diagram shows switches on Port 2; source scans P2.5 and P2.0 for mode input.
- AT89S52 uses +5 V and common ground.


---

## Inference

The firmware cycles among four LED patterns in response to button input. The diagram shows two switches; the source scans one row/column pair.

