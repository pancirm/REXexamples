Modbus master for testing UniPi as Modbus TCP slave 
===================================================
 
This folder contains the source files for the demonstration project on using
the REX Control System on the Raspberry Pi minicomputer with the UniPi extension
board. 

This example is a Modbus TCP master for testing the UniPi as Modbus slave. The 
Modbus TCP slave device (UniPi) is supposed to have the IP address 192.168.1.100.

## Modbus registers ##

### UniPi input signals ###
| Register No. | Meaning                         | Data range |
| ------------:|:------------------------------- |:---------- |
|            0 | Digital inputs (LSB=I01)        | 0..4095    |
|            1 | Analog input 1 (0..10V, 16-bit) | 0..65535   |
|            2 | Analog input 2 (0..10V, 16-bit) | 0..65535   |

### UniPi output signals ###
| Register No. | Meaning                       | Data range |
| ------------:|:----------------------------- |:---------- |
|         2048 | UniPi relays (LSB=relay 1)    | 0..255     |
|         2049 | Analog output (PWM on pin 18) | 0..1023    |

### Adding signals, changing Modbus register mapping, changing IP address of the slave device ###

Go to Modbus TCP Master driver (MTM block) configuration and press "Special 
edit" for Modbus configuration. Make sure to read the Modbus driver 
documentation (see below).

## Documentation ##

- **Press F1 for help** on the selected function block in the *RexDraw* program.
- [Getting started with REX and UniPi board (Raspberry Pi)](http://www.rexcontrols.com/media/DOC/ENGLISH/REX_Getting_Started_UniPi_ENG.pdf)
- [RPiDrv - Raspberry Pi driver (including PiFace Digital, UniPi, Intellisys PIO)](http://www.rexcontrols.com/media/DOC/ENGLISH/RPiDrv_ENG.pdf)
- [MbDrv - Modbus driver](http://www.rexcontrols.com/media/DOC/ENGLISH/MbDrv_ENG.pdf)
- [Function blocks of the REX Control System](http://www.rexcontrols.com/media/HTML/DOC/ENGLISH/index.html)
- [Complete documentation of the REX Control System](http://www.rexcontrols.com/documentation-and-support)

## Additional information ##

- More info about the UniPi board can be found at [unipi.technology](http://www.unipi.technology).
- Raspberry Pi is a trademark of the [Raspberry Pi Foundation](http://www.raspberrypi.org).
- Visit the [REX Controls company webpage](http://www.rexcontrols.com) 
for more information about the example projects and developing advanced 
automation and control solutions using the REX Control System.