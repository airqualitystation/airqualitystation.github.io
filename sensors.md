# Air Quality Sensors and Products

## Products

### MCF88 LoRaWAN endpoints
Connectivity : LoRaWAN
* [MCF-LW12TER LoRaWAN® indoor environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12ter/)
* [MCF-LW12TERPM LoRaWAN® outdoor PM and environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12terpm/)
* [MCF-LW12CO2 LoRaWAN® indoor environmental sensor with VOC, LUX and CO2](https://www.mcf88.it/prodotto/mcf-lw12co2/)
* [MCF-LW12TERWP LoRaWAN® outdoor environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12terwp/)

Note: MCF88 endpoints transmit air quality measurements by using the LoRaWAN protocol. The payload decoder is available [here](https://github.com/CampusIoT/payload-codec/tree/master/src/main/ttn_loraappserver/mcf88).

### Elsys
Connectivity : LoRaWAN
* Elsys ERS CO2
* Elsys ERS VOC

### [Nexelec](https://en.nexelec.fr/produits)
Connectivity : LoRaWAN, Sigfox, NB-IoT, Zigbee
* Origin (Smoke)
* Carbon (CO2)
* Secure (CO)
* Aero (CO2, VOC)
* PMi (PM1, PM 2.5, PM10, VOC)
* PMo (PM1, PM 2.5, PM10)
* Sense (PM1, PM 2.5, PM10, CO2, VOC)
* Atmo (PM1, PM 2.5, PM10, HCHO, CO2, VOCs)

### AERASGARD
Connectivity : na
* [ALQ-CO2-W](https://spluss.de/en/products/air-quality-and-flow/room-co2-and-air-quality-sensor-voc/alq-co2/)

### NetAtmo
Connectivity : Wifi

### [Adeunis](https://www.adeunis.com/produits/gamme-lpwan-868/)
Connectivity : LoRaWAN, Sigfox, NB-IoT

### Blueair Aware

## Boards

### Breakout Qwiic

| Board         | Samples @ Fablab | Voltage   | Interface | Sensors | OS Support | Fritzing | Demo     |
| ------------- | ---------------- | --------- | ----------| ------- | ---------- | -------- | -------- |
| [SparkFun Environmental Combo Breakout - CCS811/BME280](https://www.sparkfun.com/products/14348) | 0 | TBC | I2C | CCS811, BME280 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |
| [SparkFun Air Quality Sensor - SGP30 (Qwiic)](https://www.sparkfun.com/products/16531) | 0 | TBC | I2C | SGP30 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |
| [Adafruit SGP30 Air Quality Sensor Breakout - VOC and eCO2 - STEMMA QT / Qwiic](https://www.adafruit.com/product/3709) | 0 | TBC | I2C | SGP30 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |
| [Adafruit SGP40 Air Quality Sensor Breakout - VOC Index - STEMMA QT / Qwiic](https://www.adafruit.com/product/4829) | 0 | TBC | I2C | SGP40 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |
| [Adafruit SCD-30 - NDIR CO2 Temperature and Humidity Sensor - STEMMA QT / Qwiic](https://www.adafruit.com/product/4867) | 0 | TBC | I2C | SCD-30 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |

Note: [SparkFun's Qwiic Connect System](https://www.sparkfun.com/qwiic) uses 4-pin JST connectors to quickly interface development boards with sensors, LCDs, relays and more.

### Seeed Studio Grove sensors

[Gas sensors full list](https://wiki.seeedstudio.com/Sensor_gas/)

| Sensors       | Samples @ Fablab | Voltage   | Sensors       | OS support | Fritzing     | Demo     |
| ------------- | ---------------- | --------- | ------------- | ---------- | ------------ | -------- |
| [Dust Sensor](http://wiki.seeedstudio.com/Grove-Dust_Sensor/) |  TBC | 5V | Ultrasonic | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ2)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ2/) Combustible Gas, Smoke |  TBC | 5V | MQ2 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ3)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ3/) Alcohol Vapor |  TBC | 5V | MQ3 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ5)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ5/) LPG, Natural Gas, Town Gas |  TBC | 5V | MQ5 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ9)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ9/) Carbon Monoxide, Coal Gas, Liquefied Gas |  TBC | 5V | MQ9 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (VOC and eCO2) with SGP30 air quality sensor](https://wiki.seeedstudio.com/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/) VOC and eCO2 |  TBC | 5V | SGP30 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |

### Others

| Board         | Samples @ Fablab | Voltage   | Interfaces | Sensors       | OS support | Fritzing     | Demo     |
| ------------- | ---------------- | --------- | --------- | ------------- | ------- | ------------ | -------- |
| [SparkFun Air Quality Breakout - CCS811](https://www.sparkfun.com/products/14193) | 1 | 3.3V | I2C | VOC | TBC | TBC | TBC |
| [SparkFun Particle Sensor Breakout - MAX30105](https://www.sparkfun.com/products/14045) | TBC | 5V | I2C | Particles | TBC | TBC | TBC |
| [Dust Sensor Module Kit - GP2Y1014AU0F with Cable](https://www.adafruit.com/product/4649) | TBC | 5V | I2C | Dust | TBC | TBC | TBC |


## Components

* [MAX30105](https://cdn.sparkfun.com/assets/learn_tutorials/5/7/7/MAX30105_3.pdf)
* [CCS811](https://cdn.sparkfun.com/assets/learn_tutorials/1/4/3/CCS811_Datasheet-DS000459.pdf)
* [Sensirion Multi-Pixel Gas Sensor SGP: SGPC3, SGP30, SGP40](https://www.sensirion.com/en/environmental-sensors/gas-sensors/)
* [ST Microelectronics](??)
