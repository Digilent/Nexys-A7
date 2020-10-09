# Nexys A7 Root Repository

## Nexys A7-50T DMA Audio Demo

### Description

This branch contains sources for the Nexys A7-50T DMA Audio Demo.

This project demonstrates how to stream data in and out of the Nexys A7-50T's RAM. Vivado is used to build the demo's hardware platform, and Vitis is used to program the bitstream onto the board and to build and deploy a C application.

For more information on the Nexys A7-50T DMA Audio, including setup instructions, visit its [Demo Page](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/demos/dma-audio) on the Digilent Wiki.

For more information on the Nexys A7, including other demos that may be available, see its [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/nexys-a7/start) on the Digilent Wiki.

### Git Navigation Information

For instructions on how to use this repository with git, and for additional documentation on the submodule and branch structures used, please visit [Digilent FPGA Demo Git Repositories](https://reference.digilentinc.com/reference/programmable-logic/documents/git) on the Digilent Wiki. Note that use of git is not required to use this demo. Digilent recommends the use of project releases, for which instructions can be found in each demo wiki page, linked above.

To see other demos in this repository, see the master branch's [README](https://github.com/Digilent/Nexys-A7).

Some demos do not require some submodules, in these cases, they are still provided to ease switching between demos in git. When unused, the submodule folder is largely empty, except for a readme containing only the heading "Root commit". This demo contains the following submodules:

| Submodule | Used by this demo |
|-----------|-------------------|
| HW        | Yes         |
| SW        | Yes         |

This demo was moved into this repository during 2020.1 updates. Its history prior to these updates can be found in its old repository, linked below:
* https://github.com/Digilent/Nexys-A7-50T-DMA-Audio

### Requirements

The following are required for use of this demo. For more information on how to get any hardware or software you may be missing, see the Demo Page, linked above.

* Nexys A7-50T
* Vivado and Vitis 2020.1 Installations
* MicroUSB Cable
* Serial Terminal Emulator
* Audio cables, headphones, and/or speakers