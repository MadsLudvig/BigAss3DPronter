# Industrial 3D Printer
*__Big 3D printer made with industrial parts from an injection molding machine__*

### Introduction

This is a 3D printer made with an extruder from an injection moulding machine and Motors and axis from several old ATM CNC robots. It will be using an material dryer and a mini vacuum conveyor for supplying the extruder with material. It will be build such that the extruder only moves on one axis because of its weight (approximately 50kg). The extruder will be moved on the x-axis and the bottom plate will be moved on the z- and y-axis. The software will be Marlin which is going to run on a Teensy 4.0. Then octoprint will be used as an Marlin host to control. Here octoprint will run on a Raspberry Pi 4.0 with an 15" industrial grade touch screen.

*__More information on the individual modules can be seen in the "Modules" folder__*



### Mechanical composition

Here as said before the extruder is going to be moved in the X-axis and the bottom plate is going to be moved in the Y- and Z-axis. This is seen in Figure 5 below:

![3D-Printer-Axis](md_attachments/3D-Printer-Axis.png)

*Figure 5: Here is seen an example of how the axis will look*

Here it should be noted that although the axis placements are correct on the image. The way the axisses are moved are not. This image is just to show axis placement. The Z-axis is not moving the extruder it should here be moving the bottom plate instead. The reason why the extruder is placed on the x-axis is because of its sheer size and weight. Here it will be advantagous only to move it from side to side to minimize movement of mass. To make the x-axis move the weight of the extruder, the long axis of the ATM CNC robot is going to be used. This is because this has lots of already built-in support and can therefore support the extruder with ease. It also has place for motor mounting, gear and gearrack for moving the axis, and a cable carrier. This i going to be very advantageus for running the material supply line for the extruder, motor cables for x and w axisses, and heating element wires for extruder. Everything will then be mounted on a steel frame made out of welded steel beams. The material of the bottom plate is being researched, so the best material can be found. For now the material is aluminium, but that could also be replaced with borosilicate glass because of its hardness and temperature resistance



### Global Bill of Materials

| Name                                         | Quantity |                             Link                             | Price (DKK) |
| :------------------------------------------- | :------: | :----------------------------------------------------------: | :---------: |
| Conradt mini vacuum conveyer                 |    1     |                                                              |    4000     |
| ILCE-QX1 Power adapter                       |    1     | [Link](https://www.subtel.dk/index.php?cl=details&offerId=3978956963&lang=6&anid=915664&cnid=192d2e4a1f71bd07ce1a5f9bbb185e09&campaign=dk-pla/Netzteil/915664&gclid=Cj0KCQiAs5eCBhCBARIsAEhk4r6M4nEBqRl9llAmq8cqiiVEmtkUiZZ6ZFrAzY_FEcEVpPGQpeQw50saAnzREALw_wcB) |     259     |
| 15" Touch screen                             |    1     | [Link](https://www.beetronics.dk/15-tommer-touchskaerm-metal-4-3) |    2699     |
| Cable                                        |    1     |   [Link](https://dk.rs-online.com/web/p/yy-kabel/1811780/)   |     589     |
| Connector                                    |    16    |  [Link](https://dk.rs-online.com/web/p/d-sub-stik/5443749/)  |    6.376    |
| Connector house                              |    16    | [Link](https://dk.rs-online.com/web/p/d-sub-bagkapper/5444039/) |    27.22    |
| Material dryer                               |    1     |                                                              |     NaN     |
| SN74LS640N                                   |    6     | [Link](https://www.ti.com/store/ti/en/p/product/?p=SN74LS640N) |    9.54     |
| SN74ABT245BN                                 |    6     | [Link](https://www.ti.com/store/ti/en/p/product/?p=SN74ABT245BN) |    4.52     |
| Aluminium bottom plate                       |    1     |                                                              |     NaN     |
| Heating elements bottom plate                |    1     |                                                              |     NaN     |
| Steel frame                                  |    1     |                                                              |     NaN     |
| Mounting adapter for servo motor to extruder |    1     |                                                              |     NaN     |

So here the price comes up to: 8169kr. DKK for now. Here it should be noted that this is not close to the final cost, since the mounting brackets, the steel frame, and the aluminium bottom plate will cost a lot. 

