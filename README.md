# Nexys A7 Root Repository

## Nexys A7-50T XADC Analog to Digital Converter Demo

### Description

This branch contains sources for the Nexys A7-50T XADC Analog to Digital Converter Demo.

This project is a Vivado demo using the Nexys A7-50T's analog-to-digital converter ciruitry, switches, LEDs, and seven-segment display, written in Verilog. When programmed onto the board, voltage levels between 0 and 1 Volt are read off of the JXADC header. The 16 User LEDs increment from right to left as the voltage difference between the selected channel's pins gets larger. The seven-segment display shows the voltage difference between the selected channel's pins in volts. SW0 and SW1 select which XADC channel is displayed, as shown in the table below. See the Nexys A7-50T's [Reference Manual](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/reference-manual) for more information about how the Artix 7 FPGA's XADC is connected to header JXADC.

| XADC Channel | JXADC Pins             | SW0 Position | SW1 Position |
| ------------ | ---------------------- | ------------ | ------------ |
| AD3          | JXADC1(P) / JXADC7(N)  | Up           | Down         |
| AD10         | JXADC2(P) / JXADC8(N)  | Down         | Up           |
| AD2          | JXADC3(P) / JXADC9(N)  | Down         | Down         |
| AD11         | JXADC4(P) / JXADC10(N) | Up           | Up           |

For more information on the Nexys A7-50T XADC Analog to Digital Converter, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/demos/xadc) on the Digilent Wiki.

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
* https://github.com/Digilent/Nexys-A7-50T-XADC

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Nexys A7-50T
* Vivado 2020.1 Installation
* MicroUSB Cable
* Wires and a circuit to measure