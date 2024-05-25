## Prusa MK4 Accelerometer v0.1

🛑 This board was submitted for reference, but it won't work without a custom cable. This is because I got the pins backwards on the Click-mate connector because I had crimped my own. When trying with a stock cable from Digikey, I noticed the error. This will be fixed in the next revision. In other words: don't try to make this one.

This is the bare minimum reference circuit as provided by STMicroelectronics, with an LED for reference.

BOM:
| Digikey Part Num       | Quantity | Description                        |
| ---------------------- | -------- | ---------------------------------- |
| 1292-0201X104K250CT-ND | 1        | 0603 100nF Ceramic Capacitor       |
| CL10A106MQ8NNNC        | 1        | 0603 10uF Ceramic Capacitor        |
| IN-S63AT5G             | 1        | 0603 Green LED 525nm               |
| RC0603FR-07120RL       | 1        | 0603 120Ohm Resistor 1/10W         |
| 5025840670             | 1        | Molex Clickmate 6Pin SMT Connector |
| LIS2DHTR               | 1        | LIS2DHTR MEMS Accelerometer        |

When aligning the LIS2DHTR by hand, make sure the circle is in the top right corner, matching the stars near the LGA-12 pads.