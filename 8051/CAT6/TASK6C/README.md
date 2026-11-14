# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT6 |
| **DATE** | 20/08/2026 |
| **NAME OF EXP** | Interrupt-Driven UART Receive and Echo |
| **HARDWARE SETUP / PLATFORM** | AT89S52; USB-to-TTL converter and PC terminal; UART with Timer 1 baud generation; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASKC |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | A UART receive interrupt places bytes into a 16-byte circular buffer; the main loop reads and echoes them. |

---

## Core Logic / Pseudocode / Code Base

### Overview
A UART receive interrupt places bytes into a 16-byte circular buffer; the main loop reads and echoes them.

### Core Logic
1. A UART receive interrupt places bytes into a 16-byte circular buffer; the main loop reads and echoes them.

### Project Files
- `CAT6-Task3.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `lab6part3.c`

### Hardware Connections
- P3.1/TXD connects to converter RXD; P3.0/RXD connects to converter TXD.
- Connect converter and MCU grounds; VCC is shown at +5 V.
- The diagram shows a 11.0592 MHz clock and UART interface.


---

## Inference

The interrupt handler and circular buffer separate reception from main-loop echoing.

