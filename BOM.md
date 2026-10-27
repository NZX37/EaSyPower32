# EaSyPower32 bill of materials

This assembly list matches the JLCPCB BOM CSV in `Production Files/`. Quantities are for one board. LCSC numbers are included where provided by the design files; verify stock and package compatibility before ordering.

| Reference(s) | Qty. | Value / description | Footprint | LCSC part |
| --- | ---: | --- | --- | --- |
| C2, C5, C13 | 3 | 10 µF capacitor | 0805 | C49678 |
| C3, C4, C11 | 3 | 1 µF capacitor | 0805 | C5199872 |
| C6, C7, C8, C12 | 4 | 100 nF capacitor | 0603 | C14663 |
| D1 | 1 | 1N5819WS Schottky diode | SOD-323 | C5451629 |
| D2, D3, D4 | 3 | TVS diode (as listed in assembly BOM) | SOD-323 | C7519 |
| D5 | 1 | Indicator LED | 0603 | C19171390 |
| D6 | 1 | SK6812 RGB LED | PLCC-4, 5 × 5 mm | C5378720 |
| J1 | 1 | TYPE-C-31-M-12 USB-C receptacle | USB-C, 16-pin | C165948 |
| R2, R3 | 2 | 5.1 kΩ resistor | 0603 | C2907044 |
| R4 | 1 | 75 Ω resistor | 0805 | C17820 |
| R5, R6, R7 | 3 | 10 kΩ resistor | 0603 | C98220 |
| SW1, SW2 | 2 | Tactile push button | SMD, B3S-1000 style | C273499 |
| U1 | 1 | AP2112K-3.3 regulator | SOT-23-5 | C51118 |
| U3 | 1 | ESP32-S3-WROOM-1-N16R2 module | ESP32-S3-WROOM-1 | C2913205 |

**Total: 27 components.** The TP4056 charger module is not included in this assembly list; it is an external module connected to the board.

The assembly files are `Production Files/EaSyPower32_v1_bom.csv`, `EaSyPower32_v1_designators.csv`, and `EaSyPower32_v1_positions.csv`.
