# EaSyPower32

EaSyPower32 is an ESP32-S3 development board with USB-C and a connection for a TP4056 charger module. It is designed to make battery-powered ESP32 projects easier to prototype.

![EaSyPower32 board render](image.png)

## Features

- ESP32-S3-WROOM-1 module (N16R2)
- USB-C connection
- AP2112K 3.3 V regulator
- Reset and boot buttons
- Status LED and SK6812 RGB LED
- Breakout pins for connecting a TP4056 charger module

The TP4056 itself is not included on the PCB; install a compatible charger module in the board's battery-power connection.

## Design files

KiCad source files are in [`kicad files/`](kicad%20files/). The schematic and board previews are shown below.

| Schematic | PCB layout | Board view |
| --- | --- | --- |
| ![Schematic](image-1.png) | ![PCB layout](image-2.png) | ![Board view](image-3.png) |

## Manufacturing

Ready-to-upload Gerber and drill files are in [`Production Files/`](Production%20Files/). The original fabrication bundle is [`EaSyPower32_v1.zip`](Production%20Files/EaSyPower32_v1.zip). It contains the copper, solder mask, paste, silkscreen, board outline, and plated/non-plated drill files. The matching BOM and placement files are included as CSVs in the same folder.

For a new or modified board revision, open `breadESP32.kicad_pcb` in KiCad and regenerate fabrication outputs from that board before ordering. Check the board outline and manufacturer design rules against your chosen fabricator.

## Bill of materials

Assembly quantities are for one board and match the [assembly BOM](Production%20Files/EaSyPower32_v1_bom.csv). Unit prices vary with order quantity and stock; each LCSC listing shows the current price.

| Part / reference(s) | Quantity | Unit price | Buying link |
| --- | ---: | ---: | --- |
| 10 µF capacitor, C2/C5/C13 | 3 | See listing | [LCSC C49678](https://www.lcsc.com/product-detail/C49678.html) |
| 1 µF capacitor, C3/C4/C11 | 3 | See listing | [LCSC C5199872](https://www.lcsc.com/product-detail/C5199872.html) |
| 100 nF capacitor, C6/C7/C8/C12 | 4 | See listing | [LCSC C14663](https://www.lcsc.com/product-detail/C14663.html) |
| 1N5819WS Schottky diode, D1 | 1 | See listing | [LCSC C5451629](https://www.lcsc.com/product-detail/C5451629.html) |
| TVS diode, D2/D3/D4 | 3 | See listing | [LCSC C7519](https://www.lcsc.com/product-detail/C7519.html) |
| Indicator LED, D5 | 1 | See listing | [LCSC C19171390](https://www.lcsc.com/product-detail/C19171390.html) |
| SK6812 RGB LED, D6 | 1 | See listing | [LCSC C5378720](https://www.lcsc.com/product-detail/C5378720.html) |
| USB-C receptacle, J1 | 1 | See listing | [LCSC C165948](https://www.lcsc.com/product-detail/C165948.html) |
| 5.1 kΩ resistor, R2/R3 | 2 | See listing | [LCSC C2907044](https://www.lcsc.com/product-detail/C2907044.html) |
| 75 Ω resistor, R4 | 1 | See listing | [LCSC C17820](https://www.lcsc.com/product-detail/C17820.html) |
| 10 kΩ resistor, R5/R6/R7 | 3 | See listing | [LCSC C98220](https://www.lcsc.com/product-detail/C98220.html) |
| Tactile push button, SW1/SW2 | 2 | See listing | [LCSC C273499](https://www.lcsc.com/product-detail/C273499.html) |
| AP2112K-3.3 regulator, U1 | 1 | See listing | [LCSC C51118](https://www.lcsc.com/product-detail/C51118.html) |
| ESP32-S3-WROOM-1-N16R2, U3 | 1 | See listing | [LCSC C2913205](https://www.lcsc.com/product-detail/C2913205.html) |

See [`BOM.md`](BOM.md) for the full component list. The TP4056 charger module is external and is not included in this assembly BOM. The project journal is in [`JOURNAL.md`](JOURNAL.md), and the `Firmware/` folder contains a minimal Arduino sketch.
