# Appendix D -  Microcontroller Selection

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