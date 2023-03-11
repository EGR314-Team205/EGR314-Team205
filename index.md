# Team Organization

## Mission Statement 
_“To produce and showcase a cost-effective product that provides at least 2 different environmental sensory data types that will benefit the consumer.”_


# Checkpoint 1
[![Checkpoint1](http://img.youtube.com/vi/tuxcnhY91rg/0.jpg)](http://www.youtube.com/watch?v=tuxcnhY91rg "Checkpoint1")




# Team Design: Weather Umbrella
This is a product that will assist people in wheelchair to block the wet rain or the very hot sunlight. This device will be activated when either the temperature detects very hot weather or the user feels rain coming down. When it rains, the wind speed sensor will use the data collected of the wind speed and calculate the direction of the wind to direct the umbrella to go against the rain the protect the user from getting wet. The umbrella that is mounted in this device is a umbrella that is able to open and close with a push of a button which will be pressed by the solenoid motor. Also, there is a clamp at the bottom of the device that will be able to clamp onto the side poles of the back supports of wheelchairs.

![Concept 2](/media/webpage//EGR314Concept.png "Chosen Design Concept")


# Block Diagram 
The following illustration demonstrates the team's projected hardware system and how it interconnects with the centered microcontroller and ESP32 Module. Additionally, the team utilizes I2C as the core communication between our sensors and PIC module.

![Block Diagram](/media/webpage/Block_Diagram.png "Block Diagram")


# Verification Table 

| |5V Power Supply|PIC|Voltage Divider|Windspeed Sensor|Temp Sensor|Motor Controller|Solenoid Motor (Extension)|Auxilary Motor (Pivot)|ESP32 MQTT Module|Push Button (Manual Override)|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|5V Power Supply|u|u|u|nc|nc|nc|nc|nc|nc|nc|
|PIC| |u|u|u|u|u|nc|nc|u|u|
|Voltage Divider| | |u|nc|nc|nc|nc|nc|nc|nc|
|Windspeed Sensor| | | |u|nc|nc|nc|nc|nc|nc|
|Temp Sensor| | | | |u|nc|nc|nc|nc|nc|
|Motor Controller| | | | | |u|u|u|nc|nc|
|Solenoid Motor (Extension)| | | | | | |u|nc|nc|nc|
|Auxilary Motor (Pivot)| | | | | | | |u|nc|nc|
|ESP32 MQTT Module| | | | | | | | |u|nc|
|Push Button (Manual Override)| | | | | | | | | |u|

## keys

| sign | meaning|
| :----| :----|
| u | unverified connection/subsystem |
| x | connection verified by you |
| v (XYZ, 1/23/45)| connection verified by instructors (INITIALS, date) |
| (xyz) | serial protocol |
| nc | No Connection |

# Component Selection 


## Motor Sub System

| Solution | Price |
|:----|:----|
|drv8830dgqr <img src="/media/webpage//drv8830dgqr.png" alt="drv8830dgqr" width="25%" height="25%"/>| $2.41|
|solenoid <img src="/media/webpage//solenoid.png" alt="solenoid" width="25%" height="25%"/> | $7.50|
|motor <img src="/media/webpage//motor.png" alt="motor" width="25%" height="25%"/>| $19.95|

## Temperature Sensor & Op Amp

| Solution | Price |
|:----|:----|
|TC74A0 <img src="/media/webpage//TC74A0.png" alt="TC74A0" width="25%" height="25%"/>| $1.09|

## Hall Effect (Wind Sensor)

| Solution | Price |
|:----|:----|
|AS5600 <img src="/media/webpage//AS5600.png" alt="AS5600" width="25%" height="25%"/>| $3.46|


## Microcontroller 

| Solution | Price |
|:----|:----|
|PIC18LF26K40 <img src="/media/webpage//PIC18LF26K40.png" alt="PIC18LF26K40" width="25%" height="25%"/>| $2.04|


# Hardware Proposal 

![Hardware Proposal](/media/webpage/hardware_proposal.png "Hardware Proposal")

# Software Proposal

![Software Proposal](/media/webpage/software_proposal.png "Software Proposal")

# Appendix A - Team Organization
[ Appendix A - Team Organization](Appendix_A.md)

# Appendix B - User Needs, Benchmarking, and Requirements
[ Appendix B - User Needs, Benchmarking, and Requirements](Appendix_B.md)



# Appendix D - Component Selection
[ Appendix D -Component Selection](Appendix_D.md)


# Appendix E - Bill of Materials
[ Appendix E - Bill of Materials](Appendix_E.md)
