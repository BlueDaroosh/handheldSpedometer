---
tagline: Website and GitHub Pages
description: The Sechedule for Dariusz's Sensor Project.
layout: page
title: index schedule
---

Dariusz Kulpinski's Blog - Handheld Spedometer
----------------------------------------------

# September 11th, 2018

The GitHub Repository has been made for the project. The proposal of the project has also been made for the project
and the handheld spedometer idea is born. [Click here to see the Proposal](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/ProposalContentStudentNameRev02.xlsx)

# September 18th, 2018

The Project Schedule (Gantt Chart) was created. [Click here to see the Schedule](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/Accelerometer%20Project.mpp)

# September 25th, 2018

The Budget Sheet has been prepared and all components needed are ready to order.
[Click here to see the Budget Sheet](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PartCostSheetForSpeedometer.xlsx)

# October 2nd, 2018

All parts have been ordered and the proofs of purchase are available to view
[Invoice 1](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice1.png)  
[Invoice 2](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice2.png)  
[Invoice 3](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/invoice3.png)

# October 9th, 2018
Study day... yay!

# October 16th, 2018
All parts are in and the aquisition can be presented. Also got the chance to solder the pins on once of my accelerometers together so that breadboarding the pi and the sensor together can be done easier. Soldered on with no problem.

# October 23rd, 2018
Additional parts were ordered for the project, being the male / female connectors that connect the GPIO pins to the breadboard. Now that all parts are fully in, the breadboarding can be completed. A rough design has been made in fritzing for the board design. Reffering to that rough design, a subdirectory in fritzing holds the fritzing files for the breadboard. The PCB board and wiring diagram will be designed before the start of next class. [Click here to access the fritzing file. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo.fzz)
Below is the breadboard schematic for the connected sensor designed via Fritzing:
![Image of breadboard schematic](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_bb.jpg)
References to the wiring was added to the fritzing directory for referencing purposes. [Click here to see references.txt. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/wiringreferences.txt)
The Pi was also activated to detect the I2C address of the accelerometer. Below is the proof that the Pi detected the address of 0x53 for the ADXL345 accelerometer.
![Image Of I2C Address Proof on Pi](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/image1.JPG)

# October 30th, 2018
The PCB was fully designed and is ready to be manufactured. The Gerber files were created and sent to the prototype lab to be made for soldering for next week. The gerber files have been uploaded to github for future reference. Also the PCB schematic was uploaded to github as well. [Click here to see the Gerber Files](https://github.com/BlueDaroosh/handheldSpedometer/tree/master/GerberFiles)
Below is the image of the PCB design of the circuit board:
![Image of designed PCB](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_pcb.jpg)
The fritzing file has been updated with the new PCB design.

# November 6th, 2018
The PCB has been made by the prototype lab and retrieved for soldering. The soldering was complete, soldering all the pins including vias, sensor and pi board together. Below are the images of the final results of the soldering that was completed, and the PCB board itself below:
![PCB_Front](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PCB_Front.JPG)
![PCB_Back](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PCB_Back.JPG)
The Wiring Schematic was also updated and designed, and is now available on GitHub. Below is the Image of the Wiring Schematic designed in Fritzing:
![Schematic](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_schem.jpg)
The Fritzing file has been updated on GitHub. [Click here to access the fritzing file. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo.fzz)
On Thursday of this week, the programming of the sensor and obtaining these values will be performed and done. Stay tuned for a Blog Entry on Thursday November 8th.

# November 7th, 2018 (Not a Regular Tuesday Class)
Today was taken to focus on being able to implement the code that would get the sensor to output data and values to the pi. The first thing i did was inspect if the newly soldered board registers the address of the accelerometer. Sure enough, the i2c address was registered and i confirmed that the soldering was successful.
![Image Of The Soldered I2C Address](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/IMG_9533.JPG)
After this was verified, i started to work on getting the Remote Desktop Connection working between my laptop and my Pi. After some tedious work and troubleshooting, i was successful and i am able to remote desktop connect to the pi with my laptop.
![Image Of A Successful Connection](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/IMG_9534.JPG)
It was noted down the the pi is connectable through the IP: { 169.254.245.48 } I must use this address to connect to the pi. The programming of the sensor will not take place today, as i am not feeling well at all. I may try to do it tomorrow, otherwise the latest i can do it is on Sunday, if my health gets better or if i feel that i should do it asap.

# November 13th, 2018
This is my first day back recovering from my cold. I was not able to get the code in working order during my absense so i took the time now to do it. I was looking at a link that is witin the Works Cited text file in the code directory that allowed me to get the sensor to read data using the python programming language. Below is the link to the script source code that operated the sensor.
[Click here to see the ADXL345.py file](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Code/ADXL345.py)
Below is the output results that the sensor gave out during runtime of the script:
![OutputSample.jpg](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Code/OutputCapture.JPG)
With this sensor proven to be working, the power up milestone is achieved and confirms that the sensor operates as intended. Below is the link to the Works Cited for the projects source code and pin diagram:
[Click here to see Works Cited](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Code/WorksCited)

### But wait, there's more for November 13th! (It was done in class and out of class.)

The enclosure for the entire set here was in plan to be made as soon as the programming for the sensor was complete. Firstly went to the prototype lab to retrieve a copy of a base case template for the enclosure. Also uploaded this to the professors dropbox so that other students are able to refer to this document itself. Within CorelDraw, the case was modified so that it fits the entire length and width of the pi and the sensor together. All modifications, changes and the CorelDraw file itself is uploaded into the project repository.
[Click here to access the .cdr file](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/ADXL345Case.cdr)
Once the file is complete, it was brought over to the prototype lab to be cut out and manufactured. Once the laser cutting was complete, the entire thing was assembled together, and below is the final result:
![Enclosure Top View](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureTop.JPG)
![Enclosure Angle View](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureAngle.JPG)
![Enclosure Back View](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureBack.JPG)
At this point, this completes the major assembly and build up milestones that are required in the project! Next week will determine the next step for what is required towards the end of the course.

# November 20th, 2018
Today, since the enclosure has been built and completed since last week, i took the oppertunity to self review my enclosure, pointing out design, security, and accessibility. After the self review of the enclosure is submitted, we move onto the next step. The PowerPoint is required for the next milestone of the week, being presentations. I managed to actually complete the PowerPoint today, however trying to save this into the Git repository, the file size was exceeding 25 MB, at which Git only allows smaller or equal for upload. I sent an email to the professor for clarification on what i should do in order to figure out what to do with the PowerPoint. Other than that, my presentation date for my PowerPoint is on Tuesday, December 4th, 2018. The next blogpost will update the PowerPoint situation, and what actions are taken to make it work.

# November 23rd, 2018 (Not a Regular Tuesday Class)
I FIGURED IT OUT! In PowerPoint, clicking on an image, selecting the 'Format' tab and clicking 'Compress Images' allows you to compress the images, get rid of the unnecessary parts of it, and change its resolution so that it fits in the PowerPoint much better and smaller. Resulting in this action, my final PowerPoint presenation was dramatically reduced from 41 MB to only 3 MB. WOW! After the change was made, the PowerPoint has been uploaded to the repository under documentation. [Click Here to see the PowerPoint. ](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/Hardware%20Presentation%20-%20Dariusz.pptx)
The README.md has also been updated to include the PowerPoint Link and a notification that the Build Instructions are coming soon.
### PRESENTATION DATE: December 4th, 2018

# December 4th, 2018
Well i got the chance to present today, and everything went smoothly. So now that the presentation is done, the build instructions are to be completed by next week. Basically the build instructions have to be designed so that someone who wants to build or improve this device can follow instructions provided, which should be finely reviewed for clarity constantly. Other than that, the next log update will be the final blog post on the project, and will contain the results for the build instructions.
