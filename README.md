# solstice-core-starfire-pcb
Solstice Design System —  *Starfire* Core —  Eagle PCB

PCB files for the **Circuit Monkey** *StarFire*  **Solstice Core** *Module*

Format is EagleCAD 9.x schematic and board layout

*StarFire* is one of the first *Solstice Core* modules.

For more details, check out the product page at

  * https://www.circuitmonkey.com/product/0701   ( [404 - not found] this link is not yet active)

<img src="images/pcb-image.png" width="360">

### Revision Notes
* Rev. 0 - Initial board design.  This revision was made for evaluation and only
one unit ever made.

* Rev. A - First revision meant for human consumption.
  * Swapped Vin and GND pins on HaLo connector.   Vin was dangerously close to GND mounting hole.
  * Changed WS2812B (5x5mm) LEDs to smaller SK6812(3.5x3.5mm LEDs)
  * SK6812 LED chain is driven by SCK pin.  Was MISO pin on Rev.0 and pattern would scramble when ISP programming the board.
  * Reset switch changed to slightly larger type.
  * Mounting holes on corners changed from 2mm pan head-style to 3mm socket head type.  2mm hardware is harder to source.
  * Added Umbra connector.  A Umbra is 20-pin micro-shield that is approx. 1x1 inch and can mount under the regular shield(HaLo).
  * Added Umbra hardware mounting points throughout PCB.
  * Added mounting holes to support light pipe option at the PWR and D13 LEDs.

* Rev. B - Production version.
  * Added EN_PIXELS solder jumper on bottom of PCB to allow disabling of built-in RGB LEDs.
  * Added test points at bottom of PCB to allow externally extending the 16 on-board LEDs.
  * Added 330ohm serial resistor to external pixel output.
  * USB connector footprint issue addressed.  Footprint was correct, Seeed part number was incorrect.

#### Rev A. Issues:
 * USB connector footprint does not match physical connector sourced using Seeed library information.


## Designed by Circuit Monkey in Las Vegas, Nevada, USA
Creative Commons Attribution, Share-Alike license, check license.txt for more information. Derivative of "Arduino Leonardo Reference design" (http://www.arduino.cc/en/Main/ArduinoBoardLeonardo)

All text above must be included in any redistribution

## Gallery
<img src="images/solstice-a-1.JPG" width="480">
<img src="images/solstice-a-2.JPG" width="480">
<img src="images/solstice-a-3.JPG" width="480">
<img src="images/solstice-a-4.JPG" width="480">
