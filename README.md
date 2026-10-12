# EaSyPower32
ESP32 S3 dev kit with an (easy) place to slot in a TP4056 charger module(power) [woahh creative name]
![Render of devboard](image.png)

I started this project both to learn more about making PCBs as well as get some experience with SMD components. I also really hated when I had to make my whole own powering system for esp32, especially when space was limited, so I wanted a quick and simple way to power my esp32 projects with batteries.

# The PCB works in two parts, the basic normal ESP32 dev board, and pins which connect easily to a TP4056 chip, allowing for easy battery power.

![Schematic!](image-1.png)

![PCB](image-2.png)

![alt text](image-3.png)


Comment	Designator	Footprint	JLCPCB Part
ESP32-S3-WROOM-1-N16R2	U3	ESP32-S3-WROOM-1	C2913205
AP2112K-3.3	U2	SOT-23-5	C51118
1N5819WS	D1	SOD-323	C5451629
USBLC6-2SC6	D2	SOT-23-6	C7519
5V unidirectional TVS	D4	SOD-323	C51898314
SK6812	D6	SK6812 5050 PLCC-4	C5378720
0603 LED (your colour)	D5	LED0603	C19171390
TYPE-C-31-M-12	J1	USB-C receptacle (16 pin)	C165948
6mm SMD tactile switch	SW1,SW2	6mm tactile SMD	C273499
5.1kΩ 0603	R2,R3	R0603	C2907044
10kΩ 0603	R5,R6,R7	R0603	C98220
75Ω 0805	R4	R0805	C17820
10µF 0805 X7R	C2,C5,C13	C0805	C49678
1µF 0603 X7R	C3,C4,C11	C0603	C5199872
100nF 0603 X7R	C6,C7,C8,C12	C0603	C14663
The LCSC numbers are provided for easy purchase.