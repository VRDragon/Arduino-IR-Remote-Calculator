# Arduino IR Remote Calculator

**Infrared Remote Controlled Calculator with TM1650 7-Segment Display**

## Overview

Arduino IR Remote Calculator is an experimental embedded electronics project demonstrating how to build a simple calculator controlled by an infrared (IR) remote control.

The project uses an Arduino microcontroller to receive and decode infrared signals, process numerical input and basic arithmetic operations, and display values on a four-digit seven-segment display driven by the TM1650 controller.

Originally developed as an experimental Arduino project, it demonstrates the integration of hardware peripherals, infrared communication and basic embedded C/C++ programming.

## Features

- Infrared remote control input
- Decoding of IR remote control signals
- Numerical input (0–9)
- Basic arithmetic operations:
  - Addition (+)
  - Subtraction (-)
- Four-digit seven-segment display
- TM1650 display controller
- Serial communication for debugging

## Hardware Components

| Component | Description |
|---|---|
| Arduino | Microcontroller platform |
| IR Receiver | Infrared signal reception |
| IR Remote Control | User input |
| TM1650 | Seven-segment display controller |
| 4-digit Display | Numerical output |

## Pin Configuration

| Arduino Pin | Component | Function |
|---|---|---|
| D2 | TM1650 | Display communication |
| D3 | TM1650 | Display communication |
| D4 | IR Receiver | Infrared signal input |

## Software and Libraries

The project uses the following Arduino libraries:

- `TM1650.h` – communication with the TM1650 display controller.
- `IRSendRev.h` – infrared signal reception and decoding.

Programming language: **Arduino C/C++**

## How It Works

The program follows a simple processing sequence:

1. The IR receiver captures a signal from the remote control.
2. The received data is decoded into a numerical value or an operation command.
3. The calculator logic processes the input.
4. The numerical value is converted into a seven-segment display representation.
5. The result is displayed on the four-digit display.

## Project Structure

```text
Arduino-IR-Remote-Calculator/
│
├── Arduino-IR-Remote-Calculator.ino
└── README.md
```

## Project Status

**Legacy / Experimental Project**

This repository preserves an earlier experimental implementation of an Arduino-based infrared remote-controlled calculator.

The original source code is retained for historical and educational purposes. The current implementation contains incomplete calculator logic and may require modifications before successful compilation and operation.

## Learning Objectives

The project demonstrates practical implementation of:

- Embedded C/C++ programming
- Arduino microcontroller development
- Infrared communication protocols
- Digital signal decoding
- Seven-segment display control
- Basic arithmetic processing
- Hardware and software integration

## Author

**Vratislav Režo**

GitHub: [@VRDragon](https://github.com/VRDragon)

---

*An experimental embedded systems project exploring infrared remote control, Arduino programming and digital display interfaces.*
