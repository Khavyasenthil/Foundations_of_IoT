# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT6 |
| **DATE** | 20/08/2026 |
| **NAME OF EXP** | UART Character Receive and Echo |
| **HARDWARE SETUP / PLATFORM** | AT89S52; USB-to-TTL converter and PC terminal; 9600 baud 8-N-1; 11.0592 MHz crystal; +5 V. |
| **TASK NO** | TASKB |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware waits for a received UART character and transmits that same character back. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware waits for a received UART character and transmits that same character back.

### Core Logic
1. The firmware waits for a received UART character and transmits that same character back.

### Project Files
- `CAT6-Task2.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `lab6part2.c`

### Hardware Connections
- P3.1/TXD connects to converter RXD; P3.0/RXD connects to converter TXD.
- Connect converter and MCU grounds; VCC is shown at +5 V.
- The diagram specifies 9600 baud, 8 data bits, no parity, one stop bit.


---

## Inference

The firmware implements a serial character echo loop.

