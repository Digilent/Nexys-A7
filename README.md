# Nexys A7 Root Repository

## Nexys A7-100T Out-of-Box Demo

### Description

This branch contains sources for the Nexys A7-100T Out-of-Box Demo.

This project is a Vivado demo using the Nexys A7-100T's switches, LEDs, pushbuttons, RGB LEDS, seven-segment display, VGA connector, USB HID Host port, PWM audio output, PDM microphone, 3-axis accelerometer and the temperature sensor written in VHDL. When programmed onto the board, all sixteen of the switches are tied to their corresponding LEDs. Every time a switch is toggled, the LED directly above it will toggle with it. The seven-segment display runs a constant snake pattern.

The two RGB LEDs are initially set to smoothly change from red to green, then green to blue, then blue to red. The table below describes how the D-pad buttons affects the RGB LEDs and the microphone. Once the audio recording is started with the BTNU button the data is taken from the omni-directional microphone and stored into the DDR2 memory. While recording audio the LEDs will light up from left to right. After about 5 seconds the recording stops and the audio will be read from DDR2 memory and played through the headphone jack (labeled mono audio out). Afterwhich the LEDs will turn off from right to left.

The VGA displays a  Digilent / Analog Devices logo, the mouse cursor connected by the usb HID Host port, the audio signal from the microphone, the x , y and z data from the Accelerometer, the FPGA temperature and the value of the RGB componnents. The VGA is only displayed in 1280×1024 resolution:


| Button | Function                                                          |
| ------ | ----------------------------------------------------------------- |
| BTNU   | Audio recording is started and data is taken from the              |
|        | omni-directional microphone                                       |
| BTNC   | The RGB LEDs are set to green                                     |                                    
| BTNL   | The RGB LEDs are set to red                                       |
| BTNR   | The RGB LEDs are set to blue                                      |
| BTND   | The RGB LEDs return to their gradual change loop.                 |
|        | If the user keeps pushing BTND, both LEDs will be isolated then   |
|        | both will be turned off                                           |   

For more information on the Nexys A7-100T Out-of-Box Demo, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/demos/oob) on the Digilent Wiki.

For more information on the Nexys A7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Nexys-A7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes         |
| OS        | No         |
| SW        | No         |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Nexys-A7-100T-OOB

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Nexys A7-100T
* Vivado 2021.1 Installation
* Serial Terminal Emulator
* MicroUSB Cable
* Monitor with VGA port
* VGA Cable
* USB Mouse