Using the MCP23S17 I/O expander 
===============================

This folder contains the source files for working with the GPIO pins of the
MCP23S17 16-bit I/O expander via SPI bus, which is available e.g. on the 
Raspberry Pi minicomputer. The example is based on the REXLANG user-programmable 
function block of the REX Control System. 

The GPIO port A is used as digital outputs, the GPIO port B is used as digital
inputs with the internal pull-up resistors enabled. 

## Prerequisities ##

- SPI bus must be enabled and available (e.g. /dev/spidev0.0 on the Raspberry Pi)

## Documentation ##

- [Getting started with REX on the Raspberry Pi minicomputer](http://www.rexcontrols.com/media/DOC/ENGLISH/REX_Getting_Started_RasPi_ENG.pdf)
- [Function blocks of the REX Control System](http://www.rexcontrols.com/media/HTML/DOC/ENGLISH/index.html)

## Additional information ##

Visit the [REX Controls company webpage](http://www.rexcontrols.com/rex-control-system-raspberry-pi) 
for more information about the example projects and developing advanced 
automation and control solutions using the REX Control System and the Raspberry
Pi.

Raspberry Pi is a trademark of the [Raspberry Pi Foundation](http://www.raspberrypi.org)
