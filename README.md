# FanCTRL

Controls the fan speed using an additional PCB, especially for fans with a 4-pin connector (plus, minus, PWM, tacho).

## Features

* **4-Pin Fan Support:** Full control over standard 4-pin cooling fans, utilizing all signals:
  * **Power:** `V+` (Plus)
  * **Ground:** `GND` (Minus)
  * **PWM:** Precise speed control via Pulse Width Modulation.
  * **Tacho:** RPM feedback interpretation (Tachometer signal).
* **Dedicated Hardware:** Designed to offload fan management to a custom, additional PCB.
* **Efficient Control:** Optimized timing and frequency handling for silent and reliable fan operation.

## Pinout & Signals

| Pin | Description | Signal Type |
| :--- | :--- | :--- |
| **+** / **V+** | Power Supply | Input (e.g., 12V) |
| **-** / **GND**| Ground | Reference |
| **PWM** | Pulse Width Modulation | Control Input (Target Speed) |
| **TACHO** | Tachometer / FG | Output (RPM Feedback) |

## Hardware Setup

Connect the 4-pin fan connector directly to the designated header on the FanCTRL PCB. Ensure that the logic level of the microcontroller (e.g., 3.3V or 5V) matches the PWM input specifications of your fan or is properly shifted on the PCB.

## Getting Started

1. Clone the repository:
   ```bash
   git clone [https://github.com/Code99it/FanCTRL.git](https://github.com/Code99it/FanCTRL.git)
