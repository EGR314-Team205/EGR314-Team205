# Team Organization

## Mission Statement  

_“Our mission is to design and develop an embedded system that incorporates environmental sensors, providing users with real-time data on temperature and wind speed. By leveraging affordability and small form-factor technologies, we strive to deliver a product that will benifit the user and exceed their expectations.”_

## Checkpoint 1

[![Checkpoint1](http://img.youtube.com/vi/tuxcnhY91rg/0.jpg)](http://www.youtube.com/watch?v=tuxcnhY91rg "Checkpoint1")

## Team Design: Weather Umbrella

This is a product that will assist people in wheelchair to block the wet rain or the very hot sunlight. This device will be activated when either the temperature detects very hot weather or the user feels rain coming down. When it rains, the wind speed sensor will use the data collected of the wind speed and calculate the direction of the wind to direct the umbrella to go against the rain the protect the user from getting wet. The umbrella that is mounted in this device is a umbrella that is able to open and close with a push of a button which will be pressed by the solenoid motor. Also, there is a clamp at the bottom of the device that will be able to clamp onto the side poles of the back supports of wheelchairs.

### Design Rationale

During the decision-making process for our selected design, we realized that the initial three ideas did not fully meet the requirements of the course project, nor did they demonstrate the functionality of our project as we had hoped. To address this, we brainstormed new ideas and agreed to use the temperature sensor and hall effect sensor, given their compatibility and our prior experience with testing them. Ultimately, we settled on the innovative concept of a weather umbrella assistant for wheelchairs.

![Concept 2](/media/webpage//EGR314Concept.png "Chosen Design Concept")

## Block Diagram

The following illustration demonstrates the team's projected hardware system and how it interconnects with the centered microcontroller and ESP32 Module. Additionally, the team utilizes I2C as the core communication between our sensors and PIC module.

![Block Diagram](/media/webpage/Block_Diagram.png "Block Diagram")

## Component Selection Overview

### Motor Sub System

| Solution | Image |
|:----|:----|
|Motor Driver (DRV8830DGQR)| <img src="/media/webpage//drv8830dgqr.png" alt="drv8830DGQRdgqr" width="25%" height="25%"/>| 
|Adafruit 5V Solenoid   | <img src="/media/webpage//solenoid.png" alt="solenoid" width="25%" height="25%"/> |
|Pololu 84 RPM 6V Micro Gearmotor   | <img src="/media/webpage//motor.png" alt="motor" width="25%" height="25%"/>|

### Temperature Sensor

| Solution | Image |
|:----|:----|
|TC74A0 | <img src="/media/webpage//TC74A0.png" alt="TC74A0" width="25%" height="25%"/>|

### Hall Effect (Wind Sensor Subsystem)

| Solution | Image |
|:----|:----|
|AS5600 | <img src="/media/webpage//AS5600.png" alt="AS5600" width="25%" height="25%"/>|

### Microcontroller

| Solution | Image |
|:----|:----|
|PIC18LF26K40 | <img src="/media/webpage//PIC18LF26K40.png" alt="PIC18LF26K40" width="25%" height="25%"/>|

Refer to [Appendix E](Appendix_E.md) for more information

## Hardware Proposal

![Hardware Proposal 1](/media/webpage/hardware_proposal_1.png "Hardware Proposal 1")

![Hardware Proposal 2](/media/webpage/hardware_proposal_2.png "Hardware Proposal 2")

## Software Proposal

![Software Proposal](/media/webpage/software_proposal.png "Software Proposal")

## Appendices

### Appendix A - Team Organization

[Appendix A -Team Organization](Appendix_A.md)

### Appendix B - User Needs, Benchmarking, and Requirements

[Appendix B - User Needs, Benchmarking, and Requirements](Appendix_B.md)

### Appendix C - Design Ideation 

[Appendix C - Design Ideation](Appendix_C.md)

### Appendix D - Block Diagram

[Appendix D - Block Diagram](Appendix_D.md)

### Appendix E - Component Selection

[Appendix E -Component Selection](Appendix_E.md)

### Appendix F - Microcontroller Selection

[Appendix F - Microcontroller Selection](Appendix_F.md)

### Appendix G - Software Proposal

[Appendix G - Software Proposal](Appendix_G.md)

### Appendix H - Hardware Proposal

[Appendix H - Hardware Proposal](Appendix_H.md)
