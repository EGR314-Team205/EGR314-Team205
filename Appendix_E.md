# Appendix E - Component Selection

## Component Research

### Motor

| Option | Solution   | Pros            | Cons          |
|--------|---------------------------------------------------------------------------------|----------------------------------------------|---------------------------|
| 1 | Pololu  HP Micro Metal Gear Motors Manufacturer #4794 <br> $19.95 <br> [Product Link](https://www.digikey.com/en/products/detail/pololu-corporation/4794/10450215) | High torque <br>  Small size <br> Low power consumption	 | Low RPM  <br> Open gearbox      |
| 2 | Johnson Motor PC280LG-303 <br> $6.99 <br>[Product Link](https://www.digikey.com/en/products/detail/johnson-motor/PC280LG-303/12719605)                            | Low power consumption Higher RPM             | Low torque                |
| 3  | # Aslong motor ASJGY-370-6-150  <br> $18.00 <br> [Product Link](https://www.digikey.com/en/products/detail/aslong-motor/ASJGY-370-6-150/17141533)                          | High torque <br> Strong build                     | Higher power consumption  |

**Choice**: Pololu HP Micro Metal Gear Motors #4794

<img src="/media/webpage//motor.png" alt="motor" width="25%" height="25%"/>

**Rationale**: We decided to go with this particular product since we are able to get relatively higher torque in a small form factor with low power consumption. This fits our product idea well. 

### Temperature Sensor

| Option | Solution   |     Pros          | Cons      |
|--------|-----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| 1 | Analog Devices Inc. TMP36GT9Z <br> $2.40 <br> [Product Link](https://www.digikey.com/en/products/detail/analog-devices-inc./TMP36GT9Z/820404)                 | Can measure from -40 degrees to 125 degrees (Celsius) <br> Requires 2.7-5.5V to power Inexpensive Analog | Requires ADC <br> Would need to configure specific resistances in the temperatures desired because of the large range the sensor can detect |
| 2 |  Vishay Dale 02C5000FF <br> $7.47 <br> [Product Link](https://www.digikey.com/en/products/detail/vishay-dale/02C5000FF/7102168)                         | Smaller in size than above <br> Can measure from -40 degrees to 125 degrees (Celsius)                | More Expensive <br> Operating Voltage not specified                                                                                         |

**Choice**: Option 1: TMP36GT9Z Temperature Sensor

<img src="/media/webpage//TC74A0.png" alt="TC74A0" width="25%" height="25%"/>

**Rationale**: While both options have the same range of measurable temperatures, option 1 is able to operate at the range of 2.7V to 5.5V which is within our desired voltage of operation. Also, option 1 is significantly less expensive than option 2.

### Hall Effect Sensor (Wind Speed Subsystem)

| Option | Solution                                                                                                        | Pros                                                                                   | Cons                                                                                                                                             |
|--------|-----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 |  Adafruit 1733 <br> $44.95 <br> [Product Link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/1733/5356813)                                                                          | All in one solution <br> Simple linear Voltage to Wind Speed conversion in datasheet  | Requires 7-24V to power Expensive Sensor Requires ADC Requires OpAmp                                                                             |
| 2 | ams OSRAM AS5600-ASOM <br> $3.46 <br> [Product Link](https://www.digikey.com/en/products/detail/ams-osram/AS5600-ASOM/4914332)          | I2C protocol <br> Smaller physical footprint Wind cups can be 3d modeled or ordered         | Would require additional wind cup and structure Lower resolution Requires timer and equation implementation within code Requires external magnet |
| 3 | Bourns Inc. PEC12R-4025F-N0024 <br> $1.25 <br> [Product Link](https://www.digikey.com/en/products/detail/bourns-inc/PEC12R-4025F-N0024/4499645) | Low cost solution for reading wind speed Wind cups can be 3d modeled as well           | Would require additional wind cup and structure Lower resolution Requires timer and equation implementation within code Requires ADC             |

**Choice**: AS5600-ASOM + External cup assembly (bought or designed)

<img src="/media/webpage//AS5600.png" alt="AS5600" width="25%" height="25%"/>

**Rationale**: This hall effect sensor will simplify the electrically design while only slightly increasing the programming difficulty. Despite needing to calculate linear velocity from rotational position, this sensor will greatly reduce materials cost in both pcb footprint and external construct.


### Power Supply

| Option | Solution                                                 | Pros                                                                             | Cons                                                                            |
|--------|----------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| 1  | MicroChip  MIC4575WU <br> $4.58 <br> [Product Link](https://www.digikey.com/en/products/detail/microchip-technology/MIC4575WU/771686)                 | Output is within desired range (1.2 - 37V) <br> Familiarity Used previously in class | Larger in size compared to other options  Not always in stock Not surface mount |
| 2 | ROHM Semiconductor BD900N1G-CTR <br> $1.34 <br> [Product Link](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/BD900N1G-CTR?qs=tlsG%2FOw5FFj5wsaHI6szYQ%3D%3D )       | Surface mount Reasonable output voltage (1.25 - 13.8V)                           | More expensive than above                                                       |
| 3 | Microchip Technology / Atmel LR12K4-G  <br> $1.97 <br> [Product Link](https://www.digikey.com/en/products/detail/texas-instruments/LM340T-5-0-NOPB/6237)  | High output voltage (1-88V) In stock                                             | Most expensive of the three Smallest option                                     |


**Choice**: MIC4575WU

<img src="/media/webpage/MIC4575WU.png" alt="MIC4575WU" width="25%" height="25%"/>

**Rationale**: We chose the MIC4575WU switching voltage regulator because the team had familiarity with a variation of the chip from a previous semester's project. Additionally, it it allows our team to tune the output to 3.3V at fairly cheap cost. Furthermore, the adjustable circuit is outlined in the datasheet with exact part numbers to generate the desired voltage output.


## Power Control Module : Switching Voltage Regulator

| Option | Solution                                              | Pros                                                  | Cons                                       |
|--------|-------------------------------------------------------|-------------------------------------------------------|--------------------------------------------|
| 1 |  Adam Tech PA-012 <br> $9.71 <br> [Product Link](https://www.digikey.com/en/products/detail/adam-tech/PA-012/14317019)             | Wall mount <br>  No load power consumption                  | 5V output may be too low for components    |
| 2 | Adafruit Industries 1528-1835-ND <br> $24.50 <br> [Product Link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/353/5054549)| Not wall bound  <br> Can be recharged after use             | Most expensive option  <br>  3.7V may be too low |
| 3 | TKDY 9V 1.5A Power Supply Charger <br> $12.99 <br> [Product Link](https://www.amazon.com/Adapter-Switching-Transformer-Charger-Certificate/dp/B08F78R13B/ref=pd_lpo_1) | Continuous short circuit protection Multiple adapters | No datasheet                               |

**Choice**:  Adafruit Battery Pack

<img src="/media/webpage/power_supply.png" alt="power_supply" width="25%" height="25%"/>

**Rationale**: The Adafruit battery is not bound to a wall outlet so it can be taken almost anywhere. It can also be recharged after every use and has a life cycle of at least 500 uses.

