## Arty-Z7 Series Board Files

This repository provides the board files for the 
[Arty-Z7 boards](https://store.digilentinc.com/arty-z7-apsoc-zynq-7000-development-board-for-makers-and-hobbyists/).

## Quick Start

To use the board file along with the new sdbuild flow, first do:

```shell
git clone https://github.com/yunqu/Arty-Z7.git <LOCAL>
```

Then in your PYNQ repository (image v2.3), go to folder `sdbuild` and do:

```shell
make BOARDDIR=<LOCAL>
```

Since the make flow also accepts valid petalinux BSP, you can also
specify a given BSP in the `.spec` file. Otherwise by default this 
make flow will start from a hardware project to build the petalinux BSP.

