# Table of Contents
1. [Mission Statement](#mission-statement)<br>
2. [Innovation Showcase Poster](#innovation-showcase-poster)<br>
3. [Team Design](#team-design-weather-umbrella)<br>
   1. [Finalized Design](#final-design-innovation-showcase)<br>
   2. [Design Rationale](#design-rationale)<br>
   3. [Project Idealization](#project-idealization)<br>
      1. [Rendered Idealistic Design](#rendered-idealistic-design)<br>
4. [Block Diagram](#block-diagram)<br>
5. [Component Selection](#component-selection-overview)<br>
   1. [Motor Subsystem](#motor-subsystem)<br>
   2. [Temperature Sensor](#temperature-sensor)<br>
   3. [Wind Speed Subsystem](#hall-effect-sensor-wind-speed-subsystem)<br>
   4. [Microcontroller](#microcontroller)<br>
6. [Hardware Implementation](#hardware-implementation)<br>
   1. [PCB Renders](#pcb-renders)<br>
      1. [Team PCB](#team-pcb)<br>
      2. [Daughter Board](#daughter-board)<br>
   2. [Future Hardware Design Changes](#future-hardware-design-changes)<br>
7. [Software Implementation](#software-implementation)<br>
   1. [MPLABX Peripheral Overview](#mplabx-peripheral-overview)<br>
   2. [Topic Table](#topic-table)<br>
   3. [Feedback Controller Diagram](#feedback-controller-diagram)<br>
   4. [Future Software Design Changes](#future-software-design-changes)<br>
8. [Lessons Learned](#lessons-learned)<br>
9.  [Recommendations For Future Students](#recommendations-for-future-students)<br>
10. [Initial Design Brief](#initial-design-brief-checkpoint-1)<br>
11. [Appendix](#appendices)

## Mission Statement  

_“Our mission is to design and develop an embedded system that incorporates environmental sensors, providing users with real-time data on temperature and wind speed. By leveraging affordability and small form-factor technologies, we strive to deliver a product that will benifit the user and exceed their expectations.”_


## Innovation Showcase Poster 

![Innovation Schowcasse Poster](/media/webpage/InnovationShowCasePoster.png "Innovation Schowcasse Poster")

## Team Design: Weather Umbrella

This is a product that will assist people in wheelchair to block the wet rain or the very hot sunlight. This device will be activated when either the temperature detects very hot weather or the user feels rain coming down. When it rains, the wind speed sensor will use the data collected of the wind speed and calculate the direction of the wind to direct the umbrella to go against the rain the protect the user from getting wet. The umbrella that is mounted in this device is a umbrella that is able to open and close with a push of a button which will be pressed by the solenoid motor. Also, there is a clamp at the bottom of the device that will be able to clamp onto the side poles of the back supports of wheelchairs.

#### Final Design (Innovation Showcase)
![PCB Holder ](/media/webpage/pcb_holder.jpg "PCB Holder ")



### Design Rationale

During the decision-making process for our selected design, we realized that the initial three ideas did not fully meet the requirements of the course project, nor did they demonstrate the functionality of our project as we had hoped. To address this, we brainstormed new ideas and agreed to use the temperature sensor and hall effect sensor, given their compatibility and our prior experience with testing them. Ultimately, we settled on the innovative concept of a weather umbrella assistant for wheelchairs.

![Concept 2](/media/webpage//EGR314Concept.png "Chosen Design Concept")

### Project Idealization

#### Rendered Idealistic Design

![Project Render](/media/webpage/project_render.jpg "Project Render")

#### Render of PCB Holder

![PCB Holder Render](/media/webpage/pcb_holder_render.jpg "PCB Holder Render")

#### Render of Team PCB

![PCB Render](/media/webpage/PCB_Render.png "PCB Render")

#### Render of Umbrella Holder

![Umbrella Holder Render](/media/webpage/stnad_render.png "Umbrella Holder Render")

## Block Diagram

The following illustration demonstrates the team's projected hardware system and how it interconnects with the centered microcontroller and ESP32 Module. Additionally, the team utilizes I2C as the core communication between our sensors and PIC module.

![Block Diagram](/media/webpage/Block_Diagram.png "Block Diagram")

## Component Selection Overview

### Motor Subsystem

| Solution | Image |
|:----|:----|
|Motor Driver (DRV8830DGQR)| <img src="/media/webpage//drv8830dgqr.png" alt="drv8830DGQRdgqr" width="25%" height="25%"/>| 
|Adafruit 5V Solenoid   | <img src="/media/webpage//solenoid.png" alt="solenoid" width="25%" height="25%"/> |
|Pololu 84 RPM 6V Micro Gearmotor   | <img src="/media/webpage//motor.png" alt="motor" width="25%" height="25%"/>|

### Temperature Sensor

| Solution | Image |
|:----|:----|
|TC74A4 | <img src="/media/webpage//TC74A4.png" alt="TC74A4" width="25%" height="25%"/>|

### Hall Effect Sensor (Wind Speed Subsystem)

| Solution | Image |
|:----|:----|
|AS5600 | <img src="/media/webpage//AS5600.png" alt="AS5600" width="25%" height="25%"/>|

### Microcontroller

| Solution | Image |
|:----|:----|
|PIC18LF26K40 | <img src="/media/webpage//PIC18LF26K40.png" alt="PIC18LF26K40" width="25%" height="25%"/>|

Refer to [Appendix E](Appendix_E.md) for more information

## Hardware Implementation

The following is the schematic for our team PCB

![Hardware Proposal 1](/media/webpage/hardware_proposal_1.png "Hardware Proposal 1")

![Hardware Proposal 2](/media/webpage/hardware_proposal_2.png "Hardware Proposal 2")

Check [Appendix H - Hardware Proposal](Appendix_H.md) for more information

### PCB Renders

#### Team PCB

![PCB Render Front](/media/webpage/pcb_front_render.png "PCB Render Front")

![PCB Render Back](/media/webpage/pcb_back_render.png "PCB Render Back")

#### Daughter Board

![PCB Render Front](/media/webpage/render_daughter_board_front.png "PCB Render Front")

![PCB Render Back](/media/webpage/render_daughter_board_back.png "PCB Render Back")

### Future Hardware Design Changes

In the development of our embedded systems project, it is crucial to carefully consider the power budgeting of the system. Our design currently relies on a wall power system but will need to rely on a standalone battery supply in our proposed application. With this said, It is imperative to evaluate ways in which power budgeting can be made more efficient. One approach that our team can consider, although slightly over the top,  is the utilization of enable pins that can be controlled by unused pins from the microcontroller. Such power-saving techniques can extend the battery life of the system. Furthermore, more advanced methods, such as reducing power consumption during idle periods or implementing sleep modes, can also be explored.

Optimizing the hardware design is another important aspect to improve the performance and reliability of the system by utilizing more efficient hardware configurations. For instance, passive components packages (0805) can be standardized internally and avoid smaller IC packages as our motor controller was non-functional due to potential hardware issues with installation.

Leaving room for expansion and adaptability is an important quality to have when manufacturing. Additional sensors or hardware components can be easily added through connection pins and designing the software architecture to allow for easy modification. The potential for modularized sensor systems, such as atmospheric and humidity sensors, was discussed during the innovation showcase and should be considered for future development.

By taking into account these areas of improvement, our team can create a more efficient and reliable mobile weather station and the above changes can be implemented to ensure the system is adaptable for future versions.

## Software Implementation

Our software proposal outlines the steps for the program to effectively operate. It begins by initializing all sensors and drivers and establishing a secure connection with each of them. The program then monitors sensor values and compares them with predefined thresholds to determine the appropriate actions, including controlling the motors. By following these steps, our software will enable smooth and reliable operation of the system.

Check [Appendix G - Software Proposal](Appendix_G.md) for more information 

![Software Proposal](/media/webpage/software_proposal.png "Software Proposal")

### MPLABX Peripheral Overview
See the following figures for the peripherals and pin GPIO structure utilized in the MPLAB Code Configurator

![MPLABX_Peripherals_and_Pin_Setup_1-1](/media/webpage/MPLABX_Peripherals_and_Pin_Setup_1-1.png "MPLABX_Peripherals_and_Pin_Setup_1-1")

![MPLABX_Peripherals_and_Pin_Setup_1-2](/media/webpage/MPLABX_Peripherals_and_Pin_Setup_1-2.png "MPLABX_Peripherals_and_Pin_Setup_1-2")

![MPLABX_Peripherals_and_Pin_Setup_1-3](/media/webpage/MPLABX_Peripherals_and_Pin_Setup_1-3.png "MPLABX_Peripherals_and_Pin_Setup_1-3")

### Topic Table

Below is our table summarizing all the published and subscribed messages for our topic:

![Topic Table](/media/webpage/topic_table.png "Topic Table")

### Feedback Controller Diagram

Below is our feedback controller diagram which outlines the simplistic software loop to actuate our motors based on measured sensor data

![Feedback Controller Diagram](/media/webpage/feedback_controller.png " Feedback Controller Diagram")

### Future Software Design Changes

The current system uses an OLED screen for displaying data via bar charts. Adding additional user interface elements on top of our button, such as more complex read-only ESP32 commands, would allow the user for more interactivity and control.

The code performance can be optimized for smaller-scale embedded systems such as these which have minimal processing energy and memory. Utilizing simpler functions, algorithms, and smaller data types will reduce memory usage and optimize the overall hardware platform. Small changes such as declaring constant variables and reducing utilization of global variables will also create a better performance impact.

Given that our microcontroller only has 10kb of programmable memory, we could consider writing data to an onboard SD card if more peripherals and sensors were added to the system. With our current design, we were exceeding 90% capacity so external memory could be a valid option.
The PIC Microcontrollers have slower processing speeds so utilizing interrupt service protocols (ISP) in our code algorithms will significantly improve performance and reduce the apparent lag of our single-threaded code capacity.

## Lessons Learned

- Label components with their values on the schematic to help with organization and board populating.
- Be specific about sensor values in software proposals.
- When selecting a microcontroller, carefully read the specifications to ensure it has the necessary capabilities for the project.
- Update project files as changes are made to facilitate understanding by peers.
- Communication is critical in group projects to stay on track and ensure tasks are completed.
- Organize the software diagram logically for clarity.
- Use indicator LEDs on subsystems to test their functionality during PCB board population.
- Order multiples of components in case of breakage or loss.
- Keep track of deadlines and create a schedule for the team.
- Complete assignments beforehand for time to review and fix errors before submission.

## Recommendations for Future Students

- Pay close attention to details and be precise in your work, especially when it comes to labeling components and specifying values.
- Communication is key to success in group projects, so make sure to keep in touch with your team regularly.
- Keep your project files organized and updated to make it easier for peers to understand your work.
- When selecting components, be sure to order multiples in case of loss or breakage.
- Follow a schedule and keep track of deadlines to avoid rushing work.
- Review and double-check your work before submission to catch any errors or mistakes.
- Breaking larger assignments into smaller tasks and setting deadlines for each one.
- Identifying potential obstacles or conflicts ahead of time and coming up with strategies to address them.
- Implementing feedback from the teaching team in a timely fashion.

## Initial Design Brief (Checkpoint 1)

[![Checkpoint1](http://img.youtube.com/vi/tuxcnhY91rg/0.jpg)](http://www.youtube.com/watch?v=tuxcnhY91rg "Checkpoint1")

## Appendices

### Appendix A - Team Organization

[Appendix A -Team Organization](Appendix_A.md)

### Appendix B - User Needs, Benchmarking, and Requirements

[Appendix B - User Needs, Benchmarking, and Requirements](Appendix_B.md)

### Appendix C - Design Ideation

[Appendix C - Design Ideation](Appendix_C.md)

### Appendix D - Verification Table

[Appendix D - Verification Table](Appendix_D.md)

### Appendix E - Component Selection

[Appendix E - Component Selection](Appendix_E.md)

### Appendix F - Microcontroller Selection

[Appendix F - Microcontroller Selection](Appendix_F.md)

### Appendix G - Software Proposal

[Appendix G - Software Proposal](Appendix_G.md)

### Appendix H - Power Budget & Bill of Materials

[Appendix H - Power Budget & Bill of Materials](Appendix_H.md)
