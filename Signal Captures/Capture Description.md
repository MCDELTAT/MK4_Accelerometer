## Experiment Setup
I used a premade cable assembly, tinned the stranded wire, and inserted that into my breadboard. I used my multimeter to buzz out the correct pins and cables, and inserted them in order Pins 1-6 from the MK4 Board. I then hooked up my Logic Analyzer to each of those pins, and it should have been numbered correctly. Pulseview and/or most Logic Analyzers are zero indexed, but just think of them in order. I.E. this was the pinout from board to LA.

| MK4 Board Pin | Logic Analyzer Pin |
| ------------- | ------------------ |
| Pin 1         | D0                 |
| Pin 2         | D1                 |
| Pin 3         | D2                 |
| Pin 4         | D3                 |
| Pin 5         | D4                 |
| Pin 6         | GND                |

I've provided the raw capture files to look at if you have Pulseview or other similar software set up, or screenshots of what is basically the only important fields.

Image 1:
This shows the printers idle state, with the first changes happening when the M959 command is issued. The payload shown in image 2 is the grouping where D1-D4 are all active.

Image 2:
This shows the payload response, zoomed in from image 1. None of the channels are the same, which seems to indicate it is not a 3-Pin SPI setup. I currently have MK4 Pin 4 (D3 here) disconnected because I'm not sure where it can be wired to on the board. The only remaining pins are INT1 and INT2 on the Sparkfun Breakout Board.

Image 3:
This is zoomed out to show that D1 is the SCL pin because it's the only one with regularly occuring writes.
