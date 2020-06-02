#Marlin_2.0.X_Beta_Alfawise_Ux0 

This is a port of Marlin for Longer Lk4 printers based on work done at https://github.com/3d-printing-canada/Longer-LK1-LK2-BL-Touch-Firmware . All courtesy goes to developers of Marlin and the team responsible for porting Marlin to Longer printers.

Instructions at bottom of readme.

This port is suited for use with my E3D V6 Volcano hotend mount. It natively supports BLTouch autolevelling, E3D V6 Volcano hotend with a 100K thermistor. The port has been configured to work with a 5V BLtouch, and t he print head of my own design (Print head files available at link):

USE THIS AT YOUR SOLE RESPONSIBLITY. THIS PORT HAS NOT BEEN TESTED FOR STABILITY. I AM NOT RESPONSIBLE FOR ANY POSSIBLE DAMAGE DONE TO YOUR PRINTER DUE TO IMPROPER, OR PROPER USE OF MARLIN OR THIS PORT OF MARLIN SPECIFICALLY. I DO NOT CARRY OUT ANY CUSTOMER SERVICE.



Instructions:
1) Flashing ready project.bin
This is the easiest way to get Marlin onto your printer. Just go to releases page of this repository, and download freshest project.bin release. Copy this file onto a MicroSD card. Turn off your Longer LK4 printer. Put in the SD card. Turn the printer on. A loading bar should show up. This means firmware is flashing. After flashing, you can use Marlin. Take out the SD card, and remove the project.bin file from it to prevent re-flashing firmware every time you use. 
2) Building from scratch (This allows to reconfigure settings of Marlin, e.g. number of probe points that BLTouch will use, print speeds, etc)
Use Visual Studio Code and PlatformIO IDE extension.
Load the whole sources project into Platform IO.
Modify configuration.h file as you wish
In Platform IO IDE menu, hit Build to compile. In the source folder you'll find project.bin file. Proceed same as in section 1)




