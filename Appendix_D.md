# Appendix D - Block Diagram 


## Verification Table 

|        | 5V Power Supply | PIC | Voltage Regulator | Windspeed Sensor | Temp Sensor | Motor Controller | Solenoid Motor (Extension) | Auxilary Motor (Pivot) | ESP32 MQTT Module | Push Button (Manual Override) |
|-------------------------------|-----------------|:---:|:-----------------:|:----------------:|:-----------:|:----------------:|:--------------------------:|:----------------------:|:-----------------:|:-----------------------------:|
|        5V Power Supply        |        u        |  u  |         u         |        nc        |      nc     |         u        |             nc             |           nc           |         nc        |               nc              |
|              PIC              |                 |  u  |         u         |         u        |      u      |         u        |             nc             |            u           |         u         |               u               |
|       Voltage Regulator       |                 |     |         u         |         u        |      u      |         u        |             nc             |           nc           |         u         |               u               |
|        Windspeed Sensor       |                 |     |                   |         u        |      nc     |        nc        |             nc             |           nc           |         nc        |               nc              |
|          Temp Sensor          |                 |     |                   |                  |      u      |        nc        |             nc             |           nc           |         nc        |               nc              |
|        Motor Controller       |                 |     |                   |                  |             |         u        |              u             |            u           |         nc        |               nc              |
|   Solenoid Motor (Extension)  |                 |     |                   |                  |             |                  |              u             |           nc           |         nc        |               nc              |
|     Auxilary Motor (Pivot)    |                 |     |                   |                  |             |                  |                            |            u           |         nc        |               nc              |
| ESP32 MQTT Module             |                 |     |                   |                  |             |                  |                            |                        |         u         |               nc              |
| Push Button (Manual Override) |                 |     |                   |                  |             |                  |                            |                        |                   |               u               |

## keys

| sign | meaning|
| :----| :----|
| u | unverified connection/subsystem |
| x | connection verified by you |
| v (XYZ, 1/23/45)| connection verified by instructors (INITIALS, date) |
| (xyz) | serial protocol |
| nc | No Connection |
