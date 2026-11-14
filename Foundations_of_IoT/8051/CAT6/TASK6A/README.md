# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT6 |
| **DATE** | 20/08/2026 |
| **NAME OF EXP** | UART Initialization and Serial Character Transmission |
| **HARDWARE SETUP / PLATFORM** | AT89S52; USB-to-TTL converter and PC terminal; 9600 baud 8-N-1; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASK6A |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware configures UART and Timer 1, then repeatedly sends a fixed string character by character. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware configures UART and Timer 1, then repeatedly sends a fixed string character by character.

### Core Logic
1. The firmware configures UART and Timer 1, then repeatedly sends a fixed string character by character.

### Project Files
- `STARTUP.A51`
- `UART.c`
- `UART.uvproj`

### Hardware Connections
- P3.1/TXD connects to converter RXD; P3.0/RXD connects to converter TXD.
- Connect converter and MCU grounds; VCC is shown at +5 V.
- Source contains `TMOD9 = 0x20`; verify this likely typo in the Timer 1 setup before compiling.


---

## Inference

The code intends to send a repeated string to a PC serial terminal; verify the Timer 1 register line.

