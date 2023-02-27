

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
|TMP36GT9Z <img src="/media/webpage//TMP36GT9Z.png" alt="TMP36GT9Z" width="25%" height="25%"/>| $2.40|

## Wind Sensor

| Solution | Price |
|:----|:----|
|AS5600 <img src="/media/webpage//AS5600.png" alt="AS5600" width="25%" height="25%"/>| $3.46|


## Microcontroller 

| Solution | Price |
|:----|:----|
|PIC18LF26K40 <img src="/media/webpage//PIC18LF26K40.png" alt="PIC18LF26K40" width="25%" height="25%"/>| $2.04|


# Hardware Proposal 

![Hardware Proposal](/media/webpage/harware_proposal.png "Harware Proposal")

# Software Proposal

![Software Proposal](/media/webpage/software_proposal.png "Software Proposal")

# Appendix A - Team Organization

## Charter 

-Utilize at least two different environmental sensors in our product
-Create a low-cost solution suitable for a targeted consumer base
-Measure and record environmental data
-Broadcast sensor data via MQTT protocol addition to our portfolio of engineering project
-Continue to build experience creating embedded systems and working in a team 
-Continue to improve time management skills throughout the project/semester 
-Express our passion for the environment and engineering

## Communication Channels 

Table 1: Team Member Communication Modes

|Name               |1st Choice Communication |2nd Choice Communication|3rd Choice Communication|
|-------------------|:-----------------------:|-----------------------:|------------------------|
|Michael Gross      |Discord                  |Email                   |Text/SMS                |
|Deepit Arora       |Discord                  |Email                   |Text/SMS                |
|Amy Joyce Valencia |Discord                  |Text/SMS                |Email                   |
|Enoch Choi Discord |Discord                  |Text/SMS                |Email                   |


## Communication Procedures
Short updates will be communicated by Discord. Longer information or files will be communicated via ASU email. Instructor correspondence will pass through the team leader who will distribute any necessary information to the team in a timely manner.

## Meeting Schedule 

The ideal times for our group to meet are Tuesday/Thursday at 12pm (see Table 1 below). Additional contact information has also been provided in this section. Any member with help and coordination from the rest of the team can elect meetings. All times are subject to change in the case of emergency circumstances, sickness, absences, or any event that alters normal meeting times.

Table 2: Meeting times acceptable for each group member, green blocks display days & times that work for all group members.

| Time   | Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday |
|--------|--------|--------|---------|-----------|----------|--------|----------|
|8:00 AM |AM      |EM      |M        |EM         |M         |M       |M         |
|9:00 AM |AM      |EM      |M        |EM         |M         |M       |M         |
|10:00 AM|AM      |EAMD    |M        |EM         |M         |M       |M         |
|11:00 AM|AM      |EAMD    |EAMD     |EM         |EAMD      |M       |M         |
|12:00 PM|AMD     |        |EAMD     |           |EAMD      |M       |M         | 
|1:00 PM |AMD     |M       |AMD      |EM         |AMD       |M       |M         |
|2:00 PM |AMD     |M       |AMD      |EM         |EAMD      |M       |MD        |
|3:00 PM |AMD     |        |EAMD     |EA         |EAMD      |M       |MD        |
|4:00 PM |AMD     |E       |EAD      |EA         |EAMD      |M       |MD        |
|5:00 PM |AMD     |EM      |EAD      |AM         |EAD       |M       |M         |
|6:00 PM |AMD     |EM      |E        |AM         |E         |AM      |AM        |
|7:00 PM |EAM     |EM      |E        |AM         |E         |EAM     |EAM       |
|8:00 PM |EAM     |EAM     |EAM      |AM         |EAM       |EAM     |EAM       |
|9:00 PM |EAM     |EAM     |EAM      |AM         |EAM       |EAM     |EAM       |


Table 3: List of names, abbreviations used in Table 1 above, email, and phone. 

|People |Abbreviation| Email          | Phone       |
|-------|------------|----------------|-------------| 
|Michael|M           |mhgross2@asu.edu|520-419-9061 |
|Deepit |D           |darora12@asu.edu|480-791-8445 |
|Enoch  |E           |echoi22@asu.edu |714-393-9231 |
|Amy    |A           |acvalen9@asu.edu|808-542-8065 |

## Meeting Coordiation
What method will you use to remind yourselves of meetings (a shared calendar?) 
    A reminder text for each other about the times of the meeting.
How will your team go about changing or adding meeting times? 
    We can let each other know either during class or through discord.
What's the preferred format for meetings (face-to-face or virtually)?
    Virtually 
Are there any other procedures that your team feels are necessary? Describe them. 
    If a team member is not able to attend a team meeting, they should communicate that 


## Team Coordination 
Discord and emails will be used to communicate. The team will meet virtually over discord call and in the PRLTA 103/107 as required. Calling only be resorted to when a team member is not responding. The team has a shared folder where all the documents and files will be stored.

## Conflict Recognition and Resolution
The team will ensure all members are equally contributing to the assignments. Any minor conflicts should be communicated via a communication channel. Any major conflict should be brought to the instructor's attention and, if necessary, a mediated discussion will be held.
The team will ensure all members are equally contributing to the assignments. Any minor conflicts should be communicated via a communication channel. Any major conflict should be brought to the instructor's attention and, if necessary, a mediated discussion will be held.



# Appendix B - User Needs, Benchmarking, and Requirements

## Design Aspects 

1. Product Design 
    The product design will be based on the use of environmental sensors for the product based on the following requirements:
    1.   Product should use at least one motor controlled by a motor controller
    2.   Product should be unique and not yet sold in the market
    3.   Product should provide a solution to an environmental/weather issue
    4.  Product should have a robust design
    5.  Product should be intuitive to use 
    6.  Product should be energy efficient

2. Functionality
    1.   Product should use at least 2 environmental serial sensors
    2.   Product must work as intended even after multiple uses
    3.   Product should communicate key data over WiFi
    4.   Product should function in a variety of environments
    5.   Product should function straight from box 

3. Interactivity/User Experience
    3.  Product should be interactive in at least one way - creates a dynamic experience for the user
    2. Product should be user friendly 
    3.  Product should be able to be checked remotely
    4.  Product’s feedback response method should be easy to interpret
    5.  Product should have intuitive functionality
    6.  Product should engage the user via visual mediums
    7.  Product should engage the user to continue using the device
    8.  Product should only enhance and not impair the user experience
    9.  Product shall require very minimal reading or audio to understand, less than 150 words of instruction.
    10. Product shall be engaging enough to have bystanders to learn.

4. Customization 
    1. Product should be able to be built with common tools
    2.  Product should allow for easy intractability through the use of external WiFi communication
    3.  Product should display necessary information via a custom display unit 
    4.  Product should tailored around customer needs
    5.  Product should be easily adaptable to user needs

5. Manufacturing
    1.  Product shall have a set of extra parts in case of damage or destruction.
    2.  Parts must be easy to replace through having spare parts or parts able to be made quickly.
    3.  Product manufactured will be tested and approved by each team member before completion
    4.  Products manufactured should be of higher quality
    5.  Product should avoid expensive parts
    6.  Product should include design files and resources for easier repairs by the user

6. Safety
    1.  Product will keep a low voltage
    2.  Product shall not require tools that require training or are dangerous to use.
    3.  Product will not contain sharp edges and will use soft springs, low energy components, and keep air pressure low, if applicable.
    4.  Electrical circuits will be grounded
    5.  Product will give a notice when malfunctioning
    6.  Does not put user in any direct danger
    7. Product will not have any exposed electrical components
    8. Products should include adequate safeguards that are event-triggered.
    9. Product should be made of non-toxic materials


## Jam Board
![User Needs jamboard](/media/webpage/User%20Needs%20jamboard.png "User Needs jamboard")



## Existing Commercial Solutions

### Govee WiFi Thermometer Hygrometer H5179

Link: 
Price: $40
Vendor:Amazon
Description: This product is wifi based temperature and humidity sensor. Temperature is accurate to ±0.54℉/±0.3℃, and humidity is ±3%RH. By refreshing every 2s, you'll stay regularly updated. Now supports widget function.


<img src="/media/webpage/Govee%20WiFi%20Thermometer%20Hygrometer.png" alt="Govee WiFi Thermometer Hygrometer" width="50%" height="50%"/>


|Consumer Voice (Negative)                  | Related Customer Needs                  |
|-------------------------------------------|-----------------------------------------|
|“In less than a year. I have 5 units and   |1. The product needs to be waterproof       |
 4 no longer work. I was using reptile      |2. The product needs to be reliable         |
 cages that had misters. I believe they 
 got wet or there was just too much 
 humidity. I found rust inside the 
 batteries so I’m assuming the water 
 and high humidity did them in”

|Consumer Voice (Negative)                  | Related Customer Needs                  |
|-------------------------------------------|-----------------------------------------|
|“I wanted a more accurate and user-friendly| Should be easy to use | 
hygrometer for my humidor. With the app     |The product needs to be reliable|
I am able to see the temp, and humidity 
of my cigar cooler from anywhere. You can 
set the ranges to alert your phone if the 
temp or RH gets too high or low. Very 
useful!”



## Use Cases

### User Story #1: Sierra

Sierra is a 19-year-old college student trying to come up with her final project topic. She decides to visit a museum because she’s always had a love for learning and exploring new things. She finds out that there is an exhibit showcasing new technologies, so she checks it out. Majoring in environmental science, she wonders if she can incorporate this into her project. Upon looking at the exhibit, she sees that there are robots designed to help with environmental issues.
Sierra has become fascinated with robot technology and how they can be incorporated into fixing environmental issues. She decides that for her project, she would like to work on designing solar panels that rotate with the sun placement.

### User Story #2: Timothy

Timothy is five years old and has just recently started kindergarten. His class is going on a field trip to the science center. Tim has never seen or played with a robot before, but since there will be an exhibit, he will get to interact with them. At the exhibit, Tim is able to turn the knobs on the robot. He realizes that if he turns it to the, the robot dispenses water to water the plants, if he turns it to the left, the water stops.
Tim learns that a robot does not just have to be a piece of metal with arms and legs - as long as it was a machine that helped people with a task. He also learns that he can “program” a robot by turning different knobs and buttons, making them change their task.


# Appendix C - Design Ideation 

The following document outlines the team’s brainstorming process in preparation of developing an environmental product. By generating ~100 raw ideas, the team was able to assemble more complete product designs due to the sheer quality of possible ideas. Using the integrated collaborative application, Google Jamboard, the team generated a plethora of ideas and sorted those into categories. After this process, the team was able to conceptualize three designs and proceed to design vectorized drawings. This process can be seen below.

## Concept Sketches 


## Initial Brainstroming Session
![Initial Brainstroming Session](/media/webpage//Initial%20Brainstorming%20Session.png "Initial Brainstroming Session")

## Grouping Phase 1
The team sorted the ideas into either 1) a base idea which could be expanded upon or 2) a potential modifying attribute of a pre-existing idea.

![Grouping Phase 1](/media/webpage//Grouping%20Phase%201.png "Grouping Phase 1")

## Grouping Phase 2
We looked at the more complete ideas and then decided as a team on the three best ideas we’d like to potentially pursue further. The team then ranked each of the peripheral attributes on a scale of 1-3 with three being the best and assigned related features (yellow) to those almost complete ideas. A handful of the three star ranked attributes were too universal and would be great components of all of the designs so those were left separate and marked accordingly as applicable to all designs. The ideas that weren’t used were grouped together and kept separate.


![Grouping Phase 2](/media/webpage//Grouping%20Phase%202.png "Grouping Phase 2")

### Concept 1: Firefighter’s Hat
This concept utilizes the temperature and air quality sensor to determine whether the fan motor should actuate as an intake or as an outake direction. These sensors will constantly track the environmental data when the firefighter might be in close proximity to heat or a fire. This system, in turn, will attempt to reduce the internal temperatures inside the helmet during these harsh conditions.


![Concept 1](/media/webpage//concept1.png "Concept 1")

### Concept 2: Golf Assist
This is a wind speed sensor which will help golfers and other casual sports to determine directions and speed of wind. There is an LED which will show the user when the wind is at a minimal level. Within the pole under the LED, there is a temperature sensor that provides information to the golfers of the current temperature and the color of the LED will change depending on if it is cold(blue) or hot(red).  The white flags on the top are the wind direction  indicators that show the direction of the wind which is very useful information to golfers when they hit the ball.


![Concept 2](/media/webpage//concept2.png "Concept 2")

### Concept 3: Weather Umbrella
This is a product that will assist people in wheelchair to block the wet rain or the very hot sunlight. This device will be activated when either the temperature detects very hot weather or the user feels rain coming down. When it rains, the wind speed sensor will use the data collected of the wind speed and calculate the direction of the wind to direct the umbrella to go against the rain the protect the user from getting wet. The umbrella that is mounted in this device is a umbrella that is able to open and close with a push of a button which will be pressed by the solenoid motor. Also, there is a clamp at the bottom of the device that will be able to clamp onto the side poles of the back supports of wheelchairs.


![Concept 3](/media/webpage//EGR314Concept.png "Concept 3")


# Appendix D - Component Selection

|1. Determine your project-specific requirements| |3. Look up specifications in the PIC datasheet| | |
|:----|:----|:----|:----|:----|
|Design Considerations|Team Project-Specific Requirementsfrom Problem Definition and Block Diagram|PIC Option 1|PIC Option 2|PIC Option 3|
|How many GPIO Pins?| |25 Pins|44 Pins|80 Pins|
|Built-in Analog to Digital Converter? How many?| |24 Pins|35 Pins|23 Pins|
|Built-in Hardware PWM? How many?| |2x10 bit|4 Pins|12 Pins|
|Built-in I2C? SPI? How many?| |Both, 2|2 SPI Pins,
1 I2C Pin|Both, 1|
|Built-in UART? How many?| |2x EUSART|2 Pins|1|
|Other Required Built-In Features? (optional)| | | | |
|Additional considerations specific to your project specifications (optional)| | | | |
|2. Find 3 microcontrollers that meet your team project-specific requirements and find information on each| |4. Look up part details in the PIC datasheet| | |
|Microcontroller Considerations|Instructions|PIC Option 1|PIC Option 2|PIC Option 3|
|Part Number|Include the entire part number (leave off any letters at the end that specify the package type)|PIC18LF26K40-I/SO|PIC24HJ128GP204|PIC24FJ256DA210|
|Link (URL) to product page|Do not paste links directly into the table. Instead, link them like this.|Link|Link|Link|
|Links (URL) to Data Sheets| |Link|Link|Link|
|Links (URL) to Application Notes|Often provided by manufacturers to give you specific examples of how to use their products. Search for them in the search bar on the Microchip’s website.|Link|Link|Link|
|Links (URL) to Code Examples| |Not Specified|Link|link|
|Links (URL) to External Resources|Search on Google and YouTube for other resources for each specific microcontroller.|Link|Link|Link|
|Production Unit Cost|Find in the Microchip online store, or Digikey|$2.04|$6.90|$10.27|
|Supply Voltage Range|Find in the microcontroller datasheet|1.8V – 3.6V|3.0V to 3.6V|3.0-3.6V|
|Absolute Maximum Current for entire IC|Find in the microcontroller datasheet|Not Specified|Not Specified|Not specified|
|Maximum GPIO Pin Current (Source/Sink)|Find in the microcontroller datasheet|Not Specified|5 mA|15-25
mA|
|8-bit or 16-bit Architecture|Find in the microcontroller datasheet|8-bit|16-bit|16-bit|
|Available IC Packages / Footprints|Find in the microcontroller datasheet. Choose a microcontroller with both surface mount and DIP/through-hole packages available. See Most Common Mistakes below for requirements to improve manufacturing reliability.|SPDIP, SOIC, SSOP, QFN, UQFN, PDIP,
TQFP|SPDIP, SOIC, QFN-S, QFN, TQFP|SSOP, UQFN(28-Lead), UQFN(36-Lead)|
|Supports External Interrupts?|Find in the microcontroller datasheet|YES|YES|YES|
|In-System Programming Capability and Type|Allows for programming the microcontroller without removing it from the PCB. Find in the microcontroller datasheet.|YES, ICSP|YES, ICSP|YES, ICSP|
|Programming Hardware, Cost, and URL|Find on the microcontroller product page|PG164140, $76.99,
Link| | |
|Works with MPLAB® X Integrated Development Environment (IDE)?|Required. See Microchip Development Tools|YES|YES|YES|
|Works with Microchip Code Configurator?|Required. Go to the MCC website, click the “Manual Downloads” tab, scroll to the device library that goes with the PIC you chose (likely “MCC 8-bit PIC”) and read the release notes to make sure your microcontroller is in the list of supported devices.|YES|YES|YES|
| | | | | |
|5. Write overall pros, cons, and rankings for the chosen microcontrollers| | | | |
|Overall Pros|Write at least 2 for each microcontroller|Has all the necessary Pins Low cost
Works with MCC|Has both SPI and I2C pins.
Has all the required hardware and software capabilities.|High pin countSPI and I2C pins
Has all the required hardware and software capabilities.|
|Overall Cons|Write at least 2 for each microcontroller|Has the least amount of GPIO pins
Max GPIO current not specified|Maximum current not specified. Supply Voltage range not specified Most expensive option out of the three.
Maximum GPIO current is lower than others|Does not include code examples.
Small voltage rangehas more features than required|
|Ranking|1 = first, 2 = second, 3 = third|1|2|3|



# Appendix E - Bill of Materials

|Unit Quantity|Unit Cost|Total Cost|Manufacturer|Manufacturer Part #|Vendor Link|Datasheet Link|Supplier|Supplier Part #|
|:----|:----|:----|:----|:----|:----|:----|:----|:----|
|3|$3.46|$10.38|ams OSRAM|AS5600-ASOM|AS5600-ASOM ams OSRAM | Sensors, Transducers | DigiKey|AS5600|Digikey|AS5600-ASOMCT-ND|
|3|$1.09|$3.27|Microchip Technology|TC74A4-3.3VCTTR|https://www.digikey.com/en/products/detail/microchip-technology/TC74A0-3-3VCTTR/443283?utm_adgroup=Sensors%20%26%20Transducers&utm_source=google&utm_medium=cpc&utm_campaign=Dynamic%20Search_EN_Product&utm_term=&utm_content=Sensors%20%26%20Transducers&gclid=Cj0KCQiAorKfBhC0ARIsAHDzsluRC9vkZOzyMioyHe91-SaGQORL9M6hDhOnLADPvnQ51CuxYXtEaZkaAu0OEALw_wcB|TC74A4|Digikey|TC74A4-3.3VCTCT-ND|
|3|$0.34|$1.02|Radial Magnets, Inc.|8995|TC74A4-3.3VCTTR|https://media.digikey.com/pdf/Data%20Sheets/Radial%20Magnet%20Inc%20PDFs/8995_Dwg.pdf|Digikey|469-1024-ND|
|5|$0.85|$4.25|Mechatronics Bearing Group|6000-2RS|6000-2RS Mechatronics Bearing Group | Hardware, Fasteners, Accessories | DigiKey|https://www.mechatronics.com/bearing-group/pdf/6000-2RS.pdf|Digikey|1995-1011-ND|
|50|$0.00540|$0.27|Samsung Electro-Mechanics|CL05A104KA5NNNC|CL05A104KA5NNNC Samsung Electro-Mechanics | Capacitors | DigiKey|https://media.digikey.com/pdf/Data%20Sheets/Samsung%20PDFs/CL05A104KA5NNNC.pdf|Digikey|1276-1043-1-ND8|$0.15|$1.20|Kyocera AVX|12065C503JAT2A|12065C503JAT2A KYOCERA AVX | Capacitors | DigiKey|X7R Dielectric | KYOCERA AVX|Digikey|78-12065C503JAT2ACT-ND|
|3|$1.34|$4.02|ROHM Semiconductor|BD900N1G-CTR|BD900N1G-CTR Rohm Semiconductor | Integrated Circuits (ICs) | DigiKey|BD9xxN1-C Series Datasheet | Components101|Digikey|846-BD900N1G-CTRCT-ND|
|1|$9.71|$9.71|Adam Tech|PA-012|https://www.digikey.com/en/products/detail/adam-tech/PA-012/14317019|https://app.adam-tech.com/products/download/data_sheet/219176/pa-012-data-sheet.pdf|Digikey|2057-PA-012-ND|
|1|$1.60|$1.60|SparkFun Electronics|PRT-12748|https://www.digikey.com/en/products/detail/sparkfun-electronics/PRT-12748/17828123?s=N4IgjCBcoGwJxVAYygMwIYBsDOBTANCAPZQDaIALAAxwUBMVIAuoQA4AuUIAyuwE4BLAHYBzEAF9CYOAFYKiECkgYcBYmXB1qcRixAcuvQaImSQdDQBMkAAlZEA7rj42kRIUNxJ2RPs3FAA|n/a|Digikey|1568-PRT-12748-ND|
|100|$0.00580|$0.58|Yageo|RC0402FR-072KL|RC0402FR-072KL YAGEO | Resistors | DigiKey|Datasheet|Digikey|311-2KLRCT-ND|
|4|$0.00|$0.00| | | | | | |
|10|$0.00|$0.00| | | | | | |
|100|$0.0043|$0.43|Walsin Technology Corporation|WR06X221 JTL|https://www.digikey.com/en/products/detail/walsin-technology-corporation/WR06X221-JTL/13239083|http://www.passivecomponent.com/wp-content/uploads/chipR/ASC_WR.pdf|Digikey|1292-WR06X221JTLCT-ND|
|1|$12.99|$12.99|Cloudia|B0B7HK7QB4|B0B7HK7QB4|N/A|Amazon|N/A|
|2|$7.50|$15.00|Adafruit|3992|3992|datasheet|Digikey|1528-2797-ND|
|3|$2.41|$7.23|TI|DRV8830DGQR|DRV8830DGQR|datasheet|Digikey|296-28165-1-ND|
|6|$2.04|$12.24|Microchip Technology|PIC18LF26K40-I/SO|https://www.digikey.com/en/products/detail/microchip-technology/PIC18LF26K40-I-SO/6623494|datasheet|Digikey|PIC18LF26K40-I/SO-ND|
|10|$0.335|$3.35| | |https://www.digikey.com/en/products/detail/visual-communications-company-vcc/LSM0805543V/10229615| |Digikey| |
|2|$19.95|$39.90|pololu|4794|https://www.digikey.com/en/products/detail/pololu-corporation/4794/10450215|https://www.pololu.com/product-info-merged/4794|Digikey|2183-4794-ND|
|10|$0.15|$1.50|KYOCERA AVX|12065C503JAT2A|https://www.digikey.com/en/products/detail/kyocera-avx/12065C503JAT2A/1604879|https://datasheets.kyocera-avx.com/X7RDielectric.pdf|Digikey|478-12065C503JAT2ACT-ND|
|20|$0.35|$7.00|Visual Communications Company |LSM0805543V|https://www.digikey.com/en/products/detail/visual-communications-company-vcc/LSM0805543V/10229615|http://static.vcclite.com/files/LSM0805543V_White_Datasheet.pdf|Digikey|28-LSM0805543VCT-ND|
|2|$4.95|$9.90|Stackpole Electronics Inc|RNCP1206FTD10K0|https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNCP1206FTD10K0/2240370|https://www.seielect.com/Catalog/SEI-RNCP.pdf|Digikey|RNCP1206FTD10K0CT-ND|
| | | | | | | | | |
|5|$0.13|$0.65|Micro Commercial Co|MMSZ4684-TP|https://www.digikey.com/en/products/detail/micro-commercial-co/MMSZ4684-TP/2345538|https://www.mccsemi.com/pdf/Products/MMSZ4678-MMSZ4716(SOD-123).pdf|Digikey|MMSZ4684-TPMSCT-ND|
|3|$4.34|$13.02|Microchip Technology|MIC4575WU|https://www.digikey.com/en/products/detail/microchip-technology/MIC4575WU/771686|https://www.digikey.com/en/htmldatasheets/production/83394/0/0/1/mic4575.html|Digikey|576-1217-ND|
|5|$0.10|$0.50|Stackpole Electronics|RNCP0805FTD1K50|https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNCP0805FTD1K50/2240233|https://www.digikey.com/en/htmldatasheets/production/1956285/0/0/1/mr3fb30l0.html|Digikey|RNCP0805FTD1K50CT-ND|
|5|$0.10|$0.50|Stackpole Electronics|RNCP0805FTD2K49|https://www.digikey.com/en/products/detail/stackpole-electronics-inc/RNCP0805FTD2K49/2240240|https://www.digikey.com/en/htmldatasheets/production/1956285/0/0/1/mr3fb30l0.html|Digikey|RNCP0805FTD2K49CT-ND|
|3|$1.92|$5.76|Kyocera AVX|TPSE337M006R0100|https://www.digikey.com/en/products/detail/kyocera-avx/TPSE337M006R0100/563907|https://www.digikey.com/en/htmldatasheets/production/55214/0/0/2/tpse107m016r0100.html|Digikey|478-1804-1-ND - Cut Tape|
|3|$0.91|$2.73|TDK Corporation|445-14428-1-ND|https://www.digikey.com/en/products/detail/tdk-corporation/C2012X5R1V226M125AC/3951664|https://www.digikey.com/en/htmldatasheets/production/558740/0/0/1/c1005c0g1h100d050ba.html|Digikey|C2012X5R1V226M125AC|
|3|$0.10|$0.30|Kyocera AVX|06035C332KAT4A|https://www.digikey.com/en/htmldatasheets/production/485249/0/0/1/18125c474kat2a.html|https://www.digikey.com/en/htmldatasheets/production/485249/0/0/1/18125c474kat2a.html|Digikey|478-10681-1-ND|
