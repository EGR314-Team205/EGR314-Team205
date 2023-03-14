# Appendix E - Component Selection


# Component Research
## Motor 

| Option | Solution   | Pros            | Cons          |
|--------|---------------------------------------------------------------------------------|----------------------------------------------|---------------------------|
| 1 | Pololu  HP Micro Metal Gear Motors Manufacturer #4794 $19.95 [Product Link](https://www.digikey.com/en/products/detail/pololu-corporation/4794/10450215) | High torque Small size Low power consumption	 | Low RPM Open gearbox      |
| 2 | Johnson Motor PC280LG-303 $6.99 [Product Link](https://www.digikey.com/en/products/detail/johnson-motor/PC280LG-303/12719605?s=N4IgTCBcDaIAoGEwA4AMAZA4gWgMytxAF0BfIA)                            | Low power consumption Higher RPM             | Low torque                |
| 3  | # Aslong motor ASJGY-370-6-150  $18.00 [Product Link](https://www.digikey.com/en/products/detail/aslong-motor/ASJGY-370-6-150/17141533)                          | High torque Strong build                     | Higher power consumption  |

**Choice**: Pololu HP Micro Metal Gear Motors #4794

**Rationale**: We decided to go with this particular product since we are able to get relatively higher torque in a small form factor with low power consumption. This fits our product idea well. 


## Temperature Sensor & Op Amp 

| Option | Solution   |     Pros          | Cons      |
|--------|-----------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------|
| 1 | Analog Devices Inc. TMP36GT9Z $2.40 [Product Link](https://www.digikey.com/en/products/detail/analog-devices-inc./TMP36GT9Z/820404?utm_adgroup=Sensors%2C%20Transducers&utm_source=google&utm_medium=cpc&utm_campaign=Shopping_Supplier_Analog%20Devices_8100_Co-op&utm_term=&utm_content=Sensors%2C%20Transducers&gclid=CjwKCAiAuOieBhAIEiwAgjCvcsCZyWVeiyDcKQUVVTk8pV4ASd2GmkGpzxy_TOEjEfYKlqq3DK2GTBoC_5sQAvD_BwE)                 | Can measure from -40 degrees to 125 degrees (Celsius)  Requires 2.7-5.5V to power Inexpensive Analog | Requires ADC <br> Would need to configure specific resistances in the temperatures desired because of the large range the sensor can detect |
| 2 |  Vishay Dale 02C5000FF $7.47 [Product Link](https://www.digikey.com/en/products/detail/vishay-dale/02C5000FF/7102168?utm_adgroup=Sensors&utm_source=google&utm_medium=cpc&utm_campaign=Shopping_Supplier_Vishay&utm_term=&utm_content=Sensors&gclid=CjwKCAiAuOieBhAIEiwAgjCvcjanU_nYK6sKSd_tNL7Bc9r0mU-zho8bE9Sww9H88CmrueyUZ3rF7xoCSCEQAvD_BwE)                         | Smaller in size than above Also can measure from -40 degrees to 125 degrees (Celsius)                | More Expensive Operating Voltage not specified                                                                                         |


**Choice**: Option 1: TMP36GT9Z Temperature Sensor
**Rationale**: While both options have the same range of measurable temperatures, option 1 is able to operate at the range of 2.7V to 5.5V which is within our desired voltage of operation. Also, option 1 is significantly less expensive than option 2.

## Wind Sensor

| Option | Solution                                                                                                        | Pros                                                                                   | Cons                                                                                                                                             |
|--------|-----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 |  Adafruit 1733 $44.95 [Product Link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/1733/5356813)                                                                          | All in one solution Simple linear Voltage to Wind Speed conversion in datasheet Analog | Requires 7-24V to power Expensive Sensor Requires ADC Requires OpAmp                                                                             |
| 2 | ams OSRAM AS5600-ASOM $3.46 [Product Link](https://www.digikey.com/en/products/detail/ams-osram/AS5600-ASOM/4914332)          | I2C protocol Smaller physical footprint Wind cups can be 3d modeled or ordered         | Would require additional wind cup and structure Lower resolution Requires timer and equation implementation within code Requires external magnet |
| 3 | Bourns Inc. PEC12R-4025F-N0024 $1.25 [Product Link](https://www.digikey.com/en/products/detail/bourns-inc/PEC12R-4025F-N0024/4499645) | Low cost solution for reading wind speed Wind cups can be 3d modeled as well           | Would require additional wind cup and structure Lower resolution Requires timer and equation implementation within code Requires ADC             |


**Choice**: AS5600-ASOM + External cup assembly (bought or designed)
**Rationale**: This hall effect sensor will simplify the electrically design while only slightly increasing the programming difficulty. Despite needing to calculate linear velocity from rotational position, this sensor will greatly reduce materials cost in both pcb footprint and external construct.


## Power Supply 

| Option | Solution                                                 | Pros                                                                             | Cons                                                                            |
|--------|----------------------------------------------------------|----------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| 1  | Onsemi LM317BT $1.00 [Product Link](https://www.mouser.com/ProductDetail/onsemi/LM317BT?qs=2OtswVQKCOFqwWAJL8KJcQ%3D%3D)                 | Output is within desired range (1.2 - 37V) Familiarity. Used previously in class | Larger in size compared to other options  Not always in stock Not surface mount |
| 2 | ROHM Semiconductor BD900N1G-CTR $1.34 [Product Link](https://www.mouser.com/ProductDetail/ROHM-Semiconductor/BD900N1G-CTR?qs=tlsG%2FOw5FFj5wsaHI6szYQ%3D%3D )       | Surface mount Reasonable output voltage (1.25 - 13.8V)                           | More expensive than above                                                       |
| 3 | Microchip Technology / Atmel LR12K4-G $1.97 [Product Link](https://www.digikey.com/en/products/detail/texas-instruments/LM340T-5-0-NOPB/6237?utm_adgroup=Texas%20Instruments&utm_source=google&utm_medium=cpc&utm_campaign=Dynamic%20Search_EN_Focus%20Suppliers&utm_term=&utm_content=Texas%20Instruments&gclid=Cj0KCQiA4aacBhCUARIsAI55maFnEFSxY9Nrp74SMGPRYId6pp5bPTp1S4CAfAtAoHT3UKIn8THIalcaAgYoEALw_wcB)  | High output voltage (1-88V) In stock                                             | Most expensive of the three Smallest option                                     |

**Choice**: Option 2: ROHM Semiconductor BD900N1G-CTR
**Rationale**:

## Power Control Module : Switching Voltage Regulator - (Amy)

| Option | Solution                                              | Pros                                                  | Cons                                       |
|--------|-------------------------------------------------------|-------------------------------------------------------|--------------------------------------------|
| 1 |  Adam Tech PA-012 $9.71 [Product Link](https://www.digikey.com/en/products/detail/adam-tech/PA-012/14317019)             | Wall mount No load power consumption                  | 5V output may be too low for components    |
| 2 | Adafruit Industries 1528-1835-ND $24.50 [Product Link](https://www.digikey.com/en/products/detail/adafruit-industries-llc/353/5054549)| Not wall bound Can be recharged after use             | Most expensive option  3.7V may be too low |
| 3 | TKDY 9V 1.5A Power Supply Charger  $12.99 [Product Link](https://www.amazon.com/Adapter-Switching-Transformer-Charger-Certificate/dp/B08F78R13B/ref=pd_lpo_1?pd_rd_w=SALEX&content-id=amzn1.sym.116f529c-aa4d-4763-b2b6-4d614ec7dc00&pf_rd_p=116f529c-aa4d-4763-b2b6-4d614ec7dc00&pf_rd_r=K8CAXBE8ZR889PMYWN45&pd_rd_wg=VDzOb&pd_rd_r=45420db3-0978-4b0b-aca4-bb7349181a80&pd_rd_i=B08F78R13B&th=1) | Continuous short circuit protection Multiple adapters | No datasheet                               |

**Choice**: Option 2: Adafruit Battery Pack
**Rationale**: The Adafruit battery is not bound to a wall outlet so it can be taken almost anywhere. It can also be recharged after every use and has a life cycle of at least 500 uses.

