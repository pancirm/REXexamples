Data exchange via UDP 
=====================

This folder contains the source files for the demonstration project on data
exchange via UDP communication between two machines or computers.

Both the sender and receiver stations are implemented in the REX Control System
but any of them can be replaced by another device with UDP communication
capabilities. 

The Sender station transmits 4 signals of various types to the Receiver station. 
See the source **.c* files to understand how the data is processed and 
transmitted.

The received data is recorded in the TRND block which allows displaying of the 
trends (graphs) in the *RexView* diagnostic tool. 

## Timing of the project ##

The algorithm runs each 500 milliseconds (0.5 s). See the EXEC function block,  
tick x ntick0 = 0.05 x 10 = 0.5 

## Prerequisities ##
- RexCore must be installed and running on the target devices.

## Running the examples ##
- The **exec.mdl* file is the project main file.
- Open it with *RexDraw*.
- Specify the IP addresses in the source **.c* files. The IP addresses are 
defined by hexadecimal numbers, e.g. 0xC0A80164 for 192.168.1.100.
- Compile and download it to the target devices.
- Switch to online mode and watch the algorithm.
- Enable online monitoring of the REXLANG block (Target->Monitor selection).
- Change the constants in the Sender station on-the-fly and check if it reaches 
the Receiver station.

## Documentation ##

- **Press F1 for help** on the selected function block in the *RexDraw* program.
- [REXLANG function block documentation](http://www.rexcontrols.com/media/HTML/DOC/ENGLISH/REXLANG.html)
- [Function blocks of the REX Control System](http://www.rexcontrols.com/media/HTML/DOC/ENGLISH/index.html)
- [Complete documentation of the REX Control System](http://www.rexcontrols.com/documentation-and-support)

## Additional information ##

- Visit the [REX Controls company webpage](http://www.rexcontrols.com) 
for more information about the example projects and developing advanced 
automation and control solutions using the REX Control System.