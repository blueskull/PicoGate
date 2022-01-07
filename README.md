# PicoGate
A tiny FPGA core module featuring GW1NZ-LV1.

This module contains a Gowin GW1NZ-LV1 FPGA in 6mm\*6mm QFN48 package, a WCH CH552 USB MCU in 3mm\*3mm QFN16 package, and a Dialog Semiconductor (formerly SiLego) SLG46580 PMIC in 2mm\*3mm QFN20 package. The FPGA has 23 IOs brought out, referenced at a programmable IO voltage (by default, 1.8V and 3.3V switchable), with an additional of 2 fixed 3.3V IOs and 3 high voltage (5V) IOs, expanded through SLG46580. The MCU provides USB-JTAG and USB-SPI bridging, clock generation and supply voltage supervision, while the PMIC provides 1.2V, 3.3V and programmable VIO as well as 5V logic level shifting.

The entire module is packaged in a space saving 9.0mm\*10.0mm BGA package with 23+2+3 digital IO pads, 1.2V/3.3V/VIO regulator output pads, 5V and USB pads and ample of ground pads. As of early-2022, the budgetary 1kpcs BOM cost is around $2.5, making it ideal for adding simple custom logics to any existing designs.

The hardware and GreenPak firmware designs are licensed under the unlicense license, meaning you can basically do whatever you'd like with it, but the author kindly asks you to do good things and give more then you take. The MCU firmware is stored in my ch552-jtag repository and is licensed accordingly.
