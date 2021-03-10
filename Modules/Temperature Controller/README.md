# Temperature Controller


To control the temperature of the 6 heating bands on the extruder and the heating pads on the bottom plate, a PID controller will be made using a Raspberry Pi 3, 8 thermalcouple amplifiers and 8 solid-state relays. The outputs to the solid-state relays will be with PWM, so the temperature control is more precise. Then the Raspberry Pi 3 will run a webserver where temperature data can easily be requested and changes via POST and GET requests. This way the Raspberry Pi 4 running octoprint can request and change temperatures easily. The thermocouple amplifiers in question can be seen in the BoM. These have been chosen for their universitality of thermalcouple types and their i2c capability.



### Bill of Materials

| Name                   | Quantity |                             Link                             | Price(DKK) |
| :--------------------- | :------: | :----------------------------------------------------------: | :--------: |
| Thermocouple Amplifier |    8     | [Link](https://www.digikey.dk/product-detail/da/adafruit-industries-llc/4101/1528-4101-ND/10245127?cur=USD&lang=da) |    97.6    |
| Solid-state relay      |    8     |                             NaN                              |    NaN     |
| Raspberry Pi 3.0       |    1     |                             NaN                              |    NaN     |

