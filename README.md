# Nexys A7 Root Repository

## Nexys A7-50T General Purpose I/O Demo

### Description

This branch contains sources for the Nexys A7-50T General Purpose I/O Demo.

This project is a Vivado demo using the Nexys A7-50T's switches, LEDs, RGB LED's, pushbuttons, seven-segment display, PWM audio output, PDM microphone and USB UART bridge, written in VHDL. When programmed onto the board, all sixteen of the switches are tied to their corresponding LEDs. Every time a switch is toggled, the LED directly above it will toggle with it. If the center push button is pressed, all the LEDs will be tied to ground. The two tri-color LEDs are set to gradually change colors at all times.

The seven segment display counts up from 0 to 9 as long as no buttons are pressed. As long as BTNU is pressed, the first digit on the seven segment display is turned off. In the same manner, BTNL turns off the second digit, BTNR turns off the third, and BTND turns off the fourth. BTNC turns off the entire display and resets the counter. The microphone which is next to Pmod connector JC, records audio data and sends it to the mono audio output located at J8. To listen to the mics output, you will need to plug in headphones or a speaker. 
 
To use the USB-UART bridge feature of this demo, the Nexys A7-50T must be connected to a serial terminal on the computer it is connected to over the MicroUSB cable. Whenever the reset button or BTNC is pressed, the Nexys A7-50T sends the line “Nexys A7-50T GPIO/UART DEMO!” to the serial terminal. Whenever one of the D-pad buttons other than BTNC is pressed, the line “Button press detected!” is sent.

| Button | Function                                                          |
| ------ | ----------------------------------------------------------------- |
| BTNC   | Turns off the entire seven-segment display and resets the counter |
|        | Prints "Nexys A7-50T GPIO/UART DEMO!" through theUSB-UART bridge    |
| BTNU   | Turns off the first digit on seven-segment display                |                               
|        | Prints "Button press detected!" through the USB-UART bridge       |
| BTNL   | Turns off the second digit on seven-segment display               |
|        | Prints "Button press detected!" through theUSB-UART bridge        |
| BTNR   | Turns off the third digit on seven-segment display                |
|        | Prints "Button press detected!" through the USB-UART bridge       |
| BTND   | Turns off the fourth digit on seven-segment display               |
|        | Prints "Button press detected!" through the USB-UART bridge       |

For more information on the Nexys A7-50T General Purpose I/O Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/demos/gpio) on the Digilent Wiki.

For more information on the Nexys A7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Nexys-A7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes         |
| SW        | No         |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Nexys-A7-50T-GPIO

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Nexys A7-50T
* Vivado 2020.1 Installation
* Serial Terminal Emulator
* MicroUSB Cable
* Headphones/Speaker