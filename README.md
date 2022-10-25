## Adafruit QSPI DIP Breakout Board PCB

<a href="http://www.adafruit.com/products/5632"><img src="assets/5632.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

<a href="http://www.adafruit.com/products/5633"><img src="assets/5633.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

<a href="http://www.adafruit.com/products/5634"><img src="assets/5634.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit QSPI DIP Breakout Board. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5632
* https://www.adafruit.com/product/5633
* https://www.adafruit.com/product/5634

### Description

For many modern and powerful chips like the RP2040, ESP32, RT10xx and STM32 series microcontrollers, designers can save money and reduce the number of chip options by not including building in the Flash memory used to store code and resources. Instead, an external QSPI Flash memory chip is wired up that can provide 16-128 Megabytes of memory (5632 - 16MB, 5633 - 64MB, 5634 - 128MB. It's not as fast as if it were on the microcontroller internal bus but with Quad SPI I/O and some clever caching by the chip designer, it's pretty effective!

To make prototyping and designing with QSPI flash a little easier, we designed these breakouts that convert the wide 8-SOIC packages to a cute 0.3" wide DIP. We find these handy when testing out different flash sizes, or if we just want to add more storage memory to a project.

This is the W25QXXJVSSIQ, a 3.3V power and logic chip. Note that the Q at the end means that the Quad Enable bit is permanently set in the status register. If you're using this in QSPI mode, then it'll work right out of the box. If you're using this in SPI mode, the 'hold' and 'write protect' pins don't do anything, so just connect them to 3.3V.

In Arduino, we have the Adafruit_SPIFlash library that can be used to interface with this chip - but don't forget it's only good for 3.3V logic and power! In CircuitPython, this chip has a TOML definition file so you could use it in a board definition.

Comes with a bit of header that can be used to solder in and plug into a breadboard or  to replace an existing socketted SPI flash DIP chip.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
