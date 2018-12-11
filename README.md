# Handheld Speedometer Project
## Dariusz Kulpinski - CENG 317-0NA
![EnclosureImage](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureAngle.JPG)

Welcome to the handhelp Spedometer Repository. The Build Instructions are below.
 
[You can click here to visit the Timelog and Progress Reports](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/index.md)
 
[You can click here to see the Final PowerPoint Presenation](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/Hardware%20Presentation%20-%20Dariusz.pptx)

# BUILD INSTRUCTIONS / How To Make a Handheld Spedometer

These are the build instructions on how to make the handheld spedometer. Some items may be more complex to complete, as they need special equipement to complete (ex. PCB builders, CO2 Laser Cutter / Etcher, etc.)

To start off, we should determine what this should look like in the end. More suitably for this project, what should our output look like? Well, fist of all it must output values of speed measurement. Such that it measures your speeds in all x-y-z axis'. Basically the end result we are looking for here is simply values that we can play around with. In terms of build time for this project, it's a good idea to prepare everything before hand, such as part ordering and source downloads of items and code, pre-manufacturing items and whatsoever. If you are ready to commence the build, you can find a weekend to assemble the entire thing together. It shouldn't take you longer whatsoever. With that said, lets begin.

## What do we need to start off with?

Several components are required in order to make this project work. Such that these components are required in order to test the systems and make it a final hardware development platforms. Speaking of development platforms, the primary development platform that will be used here is the Raspberry Pi 3 B+ model. As well as the raspberry pi, the second critical component is the ADXL345 3 axis accelerometer. This is the device that is majorly required in order to recieve the actual inputs itself for the speed. Other than the two major components, all required components for this project is listed below:

- Safety Glasses (Eye protection and other protection you prefer)
- Raspberry Pi 3 B+ Model (Must be I2C ready.)
- SD Card with Raspbian OS (Available Online or install image on own SD card.)
- ADXL345 3 Axis Accelerometer (This is the primary component for measuring speeds. Must be I2C ready.)
- Breadboarding Platform (Any Size Works
- USB mouse, USB Keyboard, HDMI cable and HDMI monitor to use the Pi With.
- GPIo Cables (male to female connections between board and sensor)
- GPIo Pin Headers (Something that allows you to connect a PCB itself to the Pi)
- Jumper Wires (Used for the PCB component or the breadboarding if preffered)
- Wire stripping / Cutting tools
- Soldering Equipment (Soldering Iron, Lead Free Solder, Proper Ventilation, Wet Sponge, Solder Sucker, etc)
- Printed Circuit Board (PCB. This will be discussed later.)
- PCB design software (Example. Fritzing. This will be discussed later.)
- Device Enclosure (This will be discussed later.)
- Enclosure Design Software (Example. CorelDraw6. This will be discussed later.)
- Some means of way to produce the PCB and the enclosure (This will be discussed later.)
- And of course, some money.

But why money? It is because all these components must be purchased beforehand. It is very possible that you may already own some of these items, such as safety goggles, soldering equipement, jumpers, breadboard, tools, etc. But if you do not, it is highly reccomended to get all these items within the list above so that the project can be completed.
To get all these equipement, you must establish a budget. Without a budget, you will not know what you will be paying for, and infact lose track of what you need to order. To create a budget is simple. Simply record down everything you require, find out where you can purchase these items, note down purchase links, their cost + taxes or other shipping costs, and a simple description of what it is. Below you can find an example of the Budget Sheet that was used in order to create the project.

[You Can Click Here to View the Example Budget for the Project.](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PartCostSheetForSpeedometer.xlsx)
<br />Note: You require Microsoft Office Excel or other Spreadsheet software to view this file.

In this case, my budget example landed around $210 Canadian for this project. Depending on what you already own, the budget varies.
<br /> Once you order, and recieve all the parts needed, then the building of the actual system can begin.

## Phase 1: Testing The Design.

To start off, we need to make sure that we know how to connect our device and how its going to work in the end. With that being said, we should breadboard our design first so that we know how to design our PCB in the end.

Four connections are required to connect our accelerometer to the raspberry pi. First we need to supply 3.3V, connect the ground, and connect our I2C data bus and clock bus. We also need to ensure that the connecting pins of the accelerometer are soldered onto the device so that there is a solid connection between the breadboard pins and the sensor. Once that is done, we can wire our breadboard. Below is how the breadboarding should look like:
![Breadboard image](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_bb.jpg)
<br />[You can see more information about wiring the breadboard here.](https://www.anstack.com/blog/2016/07/05/accelerometer-intro.html
)
#### Pin locations may vary depending on the manufacturer of the sensor itself.
Basically in the end, your wiring must match the schematic as follows:
![Wiring Schematic](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_schem.jpg)
Once this breadboarding is complete, You have the option to jump towards the Third Phase of the build, which powers on the system, or continue on to the Second Phase to design the circuit board for actual system itself.

## Phase 2: Building a Circuit Board

With our breadboard schematic done, we can now design a circuit board that will eliminate all our wiring in the device. A highly reccomended software for this part is Fritzing. Fritzing is a software that allows you to design a breadboard, wiring diagram, and the circuit board itself with ease.
<br />[Click here to visit Fritzing.org](http://fritzing.org/home/)
<br />Once fritzing is installed, build a breadboard design very similar to the design above. Once designed, a schematic of your board and a PCB template will automatically be generated. All you have to do is simply complete the connections.
<br />For the PCB, make sure that each of the connections are designed to fit the devices, and ensure that they can be soldered on depending on which side the contacts are.
<br />Below is a sample of how the PCB should look like in the end:
![PCB Design](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo_pcb.jpg)
<br />[Click here to learn more on how to design a PCB in Fritzing](http://fritzing.org/learning/tutorials/designing-pcb/)
<br />Ensure that the connection to the Pi Header can be soldered on the TOP of the board, and make sure that soldering on the sensor can be done on the BOTTOM of the board. Remember, Yellow lines indicate the TOP, while orange lines indicate the BOTTOM. To connect the bottom and the top together, use VIA'S to link them together. You also have access to the original fritzing file if you want to modify that for yourself. [You can click here to download the fritzing file.](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/fritzing/handheldspedo.fzz)
<br />If you are satisfied with the board design, export the PCB as an Extended Gerber File for manufacturing. If you have access to a PCB builder, you can use that. Otherwise, you need to send these Gerber files to a service that Prints out circuit boards, which may add to your budget.

Once you obtain your circuit board, you can proceed to soldering on the pins. Please ensure that you have proper ventilation for this part, and safety glasses are absolutely mandatory for this part.
[If you need help on soldering, a tutorial can be found here.](https://www.build-electronic-circuits.com/how-to-solder/)
<br />To solder the board, ensure that the sensors pins are soldered on the BOTTOM of the board. Ensure that the PI connectors are soldered on the TOP of the board. To Solder the Vias, take some jumper wire, strip it of its protection and stick it throuhg the via. Solder the jumper on both ends, and cut off the excess. That solders on the via and you linked top to bottom.
<br /> This is an example of how the soldering should be completed:
![Soldering Example](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/PCBSoldering.png)
Once the board is fully soldered, it's time to move to Phase 3.

## Phase 3: Powering the Accelerometer

In this phase, we will test our design to see if it outputs values and reads from the sensor. This part will be majorly focused on the use of the PI, so this is where the monitor, mouse keyboard and HDMI cable come into play.
When you start up your Pi, make sure you complete setup if that has not happened already. The most important part to begin with is to ensure that we can read from our sensor's i2c address. First the Pi must be configured to activate I2C. To do this, go into your Raspberyy Pi Preferences:
![Pi Preferences](https://www.kiwi-electronics.nl/image/data/blog/5/jessie_cli_1.png)

Under your IO, ensure that the I2C interface is switched to on. That completes this step.
The next step is the i2c tools. To install this, open the terminal and type in:
#### sudo apt-get install -y i2c-tools
<br /> Input your credentials and allow the installation to complete. Once that's done, we check if our sensors i2c address is found on the GPIo. Run the following command in the terminal:
#### sudo i2cdetect -y 1
<br /> Running this, you should get the following result:
![GPIo I2C pickup](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Documentation/IMG_9533.JPG)
<br />If you see the address of 0x53, you are all set. Otherwise you need to go back and see what mistakes you have done.

Let's understand how the code is supposed to work in the end. First of all, when working with I2C, we need to program the system to ensure that it will register and read I2C devices that are connected to the I2C bus. Next thing is how this data should be processed. It depends on how you want to display and store the information. Let's say for example we want to take data from a sensor, store it in a database, and have a mobile device read from that database to display the current values for the accelerometer. Below is some PSEUDO CODE that would demonstrate what we would like to do:
![Write From Server](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/PseudoCodeAssignment/WriteFromServer.txt)
![Read From Client](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/PseudoCodeAssignment/ReadToClient.txt)

The next part is programming the device itself to take inputs from the sensor. This is written under python, but should be simple to implement. Run Thonny on the pi. Once thonny runs, save a .py file anywhere. Below is a link to the source code.
<br />[Click here to access the source code.](https://github.com/DcubeTechVentures/ADXL345/blob/master/Python/ADXL345.py)
<br />Once you format everything properly, and make sure the syntax is correct, you can run the script. By running the script, you should get the following results:
![Output Results](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Code/OutputCapture.JPG)
<br /> Feel free to look at the script, and modify it however you please. You may modify it to print out actual speed values, print out estimates, make it loop, give it an interface, etc. From this point whatever you do with the source code is at your discresion.
<br />The last part to the project is building a case that fits your circuit and pi.

## Phase 4: The Enclosure

Do do the enclosure is totally up to you, but it is highly reccomended so that your components are secured and protected. The example case for this project was made using CorelDraw 6. Other design softwares can be used as well to create the enclosure.
[This is a link to the example closure, which can be modified to your circuit design.](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/ADXL345Case.cdr)
NOTE: This is a coreldraw file, therefore you require coreldraw to edit this file.
<br />Once you design your enclosure for the circuit, you can take the file and use a locally available CO2 laser etcher or other tool that corresponds to your design. Otherwise you may also require to use a service which will build the enclosure for you, but at an added cost for the budget. Once you get your enclosure parts, build the entire thing together, and that is your final result. Below are images of an example of the final result:
![Enclosure Top](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureTop.JPG)
![Enclosure Back](https://github.com/BlueDaroosh/handheldSpedometer/blob/master/Enclosure/EnclosureBack.JPG)
This marks the end of the project. Your circuit board and enclosure are now yours to modify and cherish.

## Final Comments

If you were looking through the instructions before hand and ended up here, good for you. Projects like these are not very easy to complete without much experience of hardware manufacturing. In terms of my own experience building this system, i could say that it could be better in terms of the software and the enclosure part. Building this project myself gave me a timeframe, but not a lot of time to complete this ideally. Also my access to some components during this project were limited as the times i was around to build this didn't really accomadate my plans. It may take several attempts to do this project ideally, but otherwise you may have all the time in the world to complete this yourself. From the end of this build, you are free to take this item and modify it however you may like so that it can be better than what it normally is. From that point, i have nothing else to say. If you liked this build, please feel free to share it with others. If you did not like it at all, that means i should learn from my mistakes, but hey, this was also my first attempt at ever building with hardware. Other than that, thats it. Thank you for your support on the Handheld Speedometer.

#### Credits and Works Cited. Without these, the project would have not been possible:
Dcube Tech Ventures. (N.D.) 3-AXIS ACCELEROMETER, ADXL345 WITH RASPBERRY PI USING PYTHON. 
Obtained From: https://www.instructables.com/id/3-Axis-Accelerometer-ADXL345-With-Raspberry-Pi-Usi/
<br />AviV1. (N.D.) HOW TO USE THE ADXL345 ON RASPBERRY PI.
Obtained From: https://www.instructables.com/id/how-to-use-the-ADXL345-on-Raspberry-pi/
<br />GPIo: https://www.raspberrypi.org/documentation/usage/gpio/
<br />I2C Wiring: https://www.anstack.com/blog/2016/07/05/accelerometer-intro.html
<br /> Humber College - CENG 317 Hardware Production Tech Course
