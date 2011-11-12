gamby.hardware README
=====================

This repository contains the EAGLE files for the GAMBY LCD/Game shield for
Arduino.

If anyone is interested in porting the design over to a non-proprietary
format (e.g. gEDA), please contact me! 

Design Notes
------------

* Every Arduino pin has a second pad. These pads conform to a uniform .1"
spacing, correcting the .05" offset of the header for digital I/O pins 
8-13 and GND/AREF.

* Although it uses the same pins, this design does not use the ATMega's 
built-in SPI. Since this device does not support bidirectional communication,
using the built-in SPI would have wasted a pin; it would have overly
complicated the traces as well.

* The traces between all of the 'used' Arduino pins and the second pad
have been left uncovered by the bottom soldermask. This is to make it
easier to cut the traces should the user want to rewire things --
to make use of the hardware SPI, for example.


Prototypes
----------

The items in the prototypes directory are the versions that were sent for 
short-run fabrication. The pin-out of the first prototype differs from
the new version. The second prototype has a few minor adjustments made
to make it compatible with the fabrication service (0.1" milling bit,
etc.). 


Datasheets
----------

* LCD: Samsung UG09B63-FLGT4AA using `S6B0755 LCD Controller <http://www.alldatasheet.com/datasheet-pdf/pdf/37866/SAMSUNG/S6B0755.html>`__ or compatible (some features unsupported)
* D-Pad: `ALPS SKQAAA010 4-direction switch <http://www.alldatasheet.com/datasheet-pdf/pdf/329112/ALPS/SKQU.html>`__
* Piezo speaker: `TDK PS1240P02BT <http://www.alldatasheet.com/datasheet-pdf/pdf/349367/TDK/PS1720P02.html>`__
* Backlight LEDs: `Dialight 598-8340-107F <http://www.dialight.com/Assets%5CBrochures_And_Catalogs%5CIndication%5CMDEI5981208RT.pdf>`__


Thanks
------

Thanks go out to my fellow Boston dorkbotter, Tim, for reverse engineering
the surplus LCD module. 
