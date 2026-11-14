# Experiment Documentation

| Field | Description |
| :--- | :--- |
| **EXP** | CAT5 |
| **DATE** | 13/08/2026 |
| **NAME OF EXP** | Stepper Motor Rotation and Direction Control |
| **HARDWARE SETUP / PLATFORM** | AT89S52; four-channel stepper driver; four-phase stepper motor; +5 V logic and external motor supply. |
| **TASK NO** | TASK5C |
| **Circuit Diagram** | [Open circuit diagram](circuit.png) |
| **Core Logic / Pseudocode / Code Base** | The firmware drives four control signals on P3.0–P3.3 through a motor driver to step the motor and select direction. |

---

## Core Logic / Pseudocode / Code Base

### Overview
The firmware drives four control signals on P3.0–P3.3 through a motor driver to step the motor and select direction.

### Core Logic
1. The firmware drives four control signals on P3.0–P3.3 through a motor driver to step the motor and select direction.

### Project Files
- `Motor_stepper.uvproj`
- `STARTUP.A51`
- `firmware.hex`
- `motor.c`

### Hardware Connections
- P3.0–P3.3 connect to driver inputs IN1–IN4.
- Driver outputs OUT1–OUT4 connect to the four-phase stepper motor.
- The diagram shows +5 V logic power and a separate external motor supply; use common ground.


---

## Inference

The output sequence is intended to rotate the stepper motor through the driver.

