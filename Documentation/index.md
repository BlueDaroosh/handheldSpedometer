---
tagline: Website and GitHub Pages
description: The Sechedule for Dariusz's Sensor Project.
layout: page
title: index schedule
---

Dariusz Kulpinski's Blog - Handheld Spedometer
----------------------------------------------

### September 11th, 2018

The GitHub Repository has been made for the project. The proposal of the project has also been made for the project
and the handheld spedometer idea is born. [Click here to see the Proposal](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/ProposalContentStudentNameRev02.xlsx)

### September 18th, 2018

The Project Schedule (Gantt Chart) was created. [Click here to see the Schedule](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/Accelerometer%20Project.mpp)

### September 25th, 2018

The Budget Sheet has been prepared and all components needed are ready to order.
[Click here to see the Budget Sheet](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PartCostSheetForSpeedometer.xlsx)

### October 2nd, 2018

All parts have been ordered and the proofs of purchase are available to view
[Invoice 1](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice1.png)  
[Invoice 2](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice2.png)  
[Invoice 3](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice3.png)

### October 9th, 2018
Study day... yay!

### October 16th, 2018
All parts are in and the aquisition can be presented. Also got the chance to solder the pins on once of my accelerometers together so that breadboarding the pi and the sensor together can be done easier. Soldered on with no problem.

### October 23rd, 2018
Additional parts were ordered for the project, being the male / female connectors that connect the GPIO pins to the breadboard. Now that all parts are fully in, the breadboarding can be completed. A rough design has been made in fritzing for the board design. Reffering to that rough design, a subdirectory in fritzing holds the fritzing files for the breadboard. The PCB board and wiring diagram will be designed before the start of next class. [Click here to access the fritzing file. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo.fzz)
Below is the breadboard schematic for the connected sensor designed via Fritzing:
![Image of breadboard schematic](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_bb.jpg)
References to the wiring was added to the fritzing directory for referencing purposes. [Click here to see references.txt. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/wiringreferences.txt)
The Pi was also activated to detect the I2C address of the accelerometer. Below is the proof that the Pi detected the address of 0x53 for the ADXL345 accelerometer.
![Image Of I2C Address Proof on Pi](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/image1.JPG)

### October 30th, 2018
The PCB was fully designed and is ready to be manufactured. The Gerber files were created and sent to the prototype lab to be made for soldering for next week. The gerber files have been uploaded to github for future reference. Also the PCB schematic was uploaded to github as well. [Click here to see the Gerber Files](https://github.com/BlueDaroosh/handheldSpedometer/tree/master/GerberFiles)
Below is the image of the PCB design of the circuit board:
![Image of designed PCB](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_pcb.jpg)
The fritzing file has been updated with the new PCB design.
