## Prusa MK4 Accelerometer v0.2

🛑 Status: Design complete, have ordered PCBs, have not tried on a real printer.

This board design fixes a large error made in the last revision, namely, the pinout is correct for a stock cable purchased from Digikey. Thus you should be able to buy cables from them, and immediately plug it into your printer. I also moved a silkscreen around the LIS2DH chip for hopefully better visual alignment. Finally, as reported in issue #1 of the repo, a 2.2K may be added to make this circuit compatible with 0.3.7 and 0.4.4 boards.

This is the bare minimum reference circuit as provided by STMicroelectronics, with an LED for reference.

BOM:
| Label | Digikey Part Num       | Quantity | Description                        |
| ----- | ---------------------- | -------- | ---------------------------------- |
| C1    | 1292-0201X104K250CT-ND | 1        | 0603 100nF Ceramic Capacitor       |
| C2    | CL10A106MQ8NNNC        | 1        | 0603 10uF Ceramic Capacitor        |
| D1    | IN-S63AT5G             | 1        | 0603 Green LED 525nm               |
| R1    | RC0603FR-07120RL       | 1        | 0603 120Ohm Resistor 1/10W         |
| R2    | ERJ-H3GJ222V           | 1        | 0603 2.2K Resistor Panasonic 1/8W  |
| J1    | 5025840670             | 1        | Molex Clickmate 6Pin SMT Connector |
| U1    | LIS2DHTR               | 1        | LIS2DHTR MEMS Accelerometer        |

When aligning the LIS2DHTR by hand, make sure the circle is in the top right corner, matching the stars near the LGA-12 pads.