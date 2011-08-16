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


Thanks
------

Thanks go out to my fellow Boston dorkbotter, Tim, for reverse engineering
the surplus LCD module. 
