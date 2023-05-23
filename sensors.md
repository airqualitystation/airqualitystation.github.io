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
* [Elsys ERS CO2](https://www.elsys.se/en/ers-co2/) (CO2)
* [Elsys ERS VOC](https://www.elsys.se/en/ers-voc/) (VOC)

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

### NKE Watteco
Connectivity : LoRaWAN
* [VAQA’O+](https://www.nke-watteco.fr/produit/capteur-vaqao-plus-lorawan/) (CO2, VOC)

### Ethera Labs
Connectivity : LoRaWAN, LTE, ModBus
* [NEMo XT](https://www.ethera-labs.com/produit/nemo-xt-station-de-monitoring-de-la-qualite-de-lair-interieur/) (CO2, COVL, formaldehyd + additional sensors for PM 1-2,5-10, NO2, O3)

### AERASGARD
Connectivity : na
* [ALQ-CO2-W](https://spluss.de/en/products/air-quality-and-flow/room-co2-and-air-quality-sensor-voc/alq-co2/)

### NetAtmo
Connectivity : Wifi

### [Adeunis](https://www.adeunis.com/produits/gamme-lpwan-868/)
Connectivity : LoRaWAN, Sigfox, NB-IoT
* [Adeunis Breath](https://www.adeunis.com/en/produit/breath-indoor-air-quality/)
* [Adeunis Confort C02](https://www.adeunis.com/en/produit/iaq-co2-temperature-humidity/)

### Blueair Aware

### Vittascience education Kits
* [Qualité d'air - version Arduino](https://fr.vittascience.com/shop/170/qualite-d-air---version-arduino)
* [Qualité d'air - version M5Stack](https://fr.vittascience.com/shop/320/qualite-d-air---version-m5stack)
* [Qualité d'air - version micro:bit](https://fr.vittascience.com/shop/171/qualite-d-air---version-micro-bit)


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
| [Grove CO2 SDC41](https://wiki.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41/) |  1 | 2.4V~5V | SCD41 (CO2, TH) | RiotOS: TBD, Stm32duino: TBD | TBD | [Wio](https://github.com/CampusIoT/tutorial/tree/master/wioterminal/examples/GroveCO2TemperatureHumiditySensorSCD41) |
| [Grove - Gas Sensor V2(Multichannel)](https://wiki.seeedstudio.com/Grove-Multichannel-Gas-Sensor-V2/) |  1 | 2.4V~5V | CO, NO2, C2H5CH, VOC  ... with GM-102B, GM-302B, GM-502B et GM-702B. | RiotOS: TBD, Stm32duino: TBD | TBD | [Wio](https://wiki.seeedstudio.com/Grove-Multichannel-Gas-Sensor-V2/) |
| [Dust Sensor](http://wiki.seeedstudio.com/Grove-Dust_Sensor/) |  TBC | 5V | Ultrasonic | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ2)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ2/) Combustible Gas, Smoke |  TBC | 5V | MQ2 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ3)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ3/) Alcohol Vapor |  TBC | 5V | MQ3 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ5)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ5/) LPG, Natural Gas, Town Gas |  TBC | 5V | MQ5 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ9)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ9/) Carbon Monoxide, Coal Gas, Liquefied Gas |  TBC | 5V | MQ9 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Grove - Multichannel Gas Sensor v2](https://www.seeedstudio.com/Grove-Multichannel-Gas-Sensor-v2-p-4569.html) |  Carbon monoxide (CO), Nitrogen dioxide (NO2), Ethyl alcohol(C2H5CH), Volatile Organic Compounds (VOC) ... | 3.3V~5V  | GM-102B; GM-302B; GM-502B; GM-702B | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (VOC and eCO2) with SGP30 air quality sensor](https://wiki.seeedstudio.com/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/) VOC and eCO2 |  TBC | 5V | SGP30 | RiotOS: TBD, Stm32duino: TBD | TBD | [Wio](https://github.com/CampusIoT/tutorial/tree/master/wioterminal/examples/GroveCO2TemperatureHumiditySensorSCD30) |
| [Grove - High Precision Barometric Pressure Sensor DPS310](https://wiki.seeedstudio.com/Grove-High-Precision-Barometric-Pressure-Sensor-DPS310/) |  TBC | 3.3V / 5V | Infineon DPS310 (Barometer) | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |


### Others

| Board         | Samples @ Fablab | Voltage   | Interfaces | Sensors       | OS support | Fritzing     | Demo     |
| ------------- | ---------------- | --------- | --------- | ------------- | ------- | ------------ | -------- |
| [SparkFun Air Quality Breakout - CCS811](https://www.sparkfun.com/products/14193) | 1 | 3.3V | I2C | VOC | [RIOT](https://github.com/RIOT-OS/RIOT/tree/master/drivers/ccs811) | TBC | TBC |
| [SparkFun Particle Sensor Breakout - MAX30105](https://www.sparkfun.com/products/14045) | TBC | 5V | I2C | Particles | TBC | TBC | TBC |
| [Dust Sensor Module Kit - GP2Y1014AU0F with Cable](https://www.adafruit.com/product/4649) | TBC | 5V | I2C | Dust | TBC | TBC | TBC |
| [SparkFun Geiger Counter](https://easyeda.com/SparkFun/SparkFun_Geiger_Counter-djF0K64qo) | 1 | 5V | UART | Radiation | [Python](https://air.imag.fr/index.php/Geiger_counter), [Processing](https://air.imag.fr/index.php/Geiger_counter) | TBC | TBC |

## Components

* [MAX30105](https://cdn.sparkfun.com/assets/learn_tutorials/5/7/7/MAX30105_3.pdf)
* [CCS811](https://cdn.sparkfun.com/assets/learn_tutorials/1/4/3/CCS811_Datasheet-DS000459.pdf) : Drivers: [RIOT](https://github.com/RIOT-OS/RIOT/tree/master/drivers/ccs811)
* [Sensirion Multi-Pixel Gas Sensor SGP: SGPC3, SGP30, SGP40](https://www.sensirion.com/en/environmental-sensors/gas-sensors/)
* [Sensirion PM Sensor SPS30](https://sensirion.com/products/catalog/SPS30/) [Arduino driver](https://github.com/Sensirion/arduino-sps)
* [ST Microelectronics](??)
* [Amphenol Telaire SM-PWM-01C](https://www.amphenol.com/node/4647) SMART Dust Sensor
* [Plantower PMS7003 PM Sensor](http://www.plantower.com/en/content/?110.html) : [@Gotronic](https://www.gotronic.fr/art-capteur-de-qualite-de-l-air-pms7003-30623.htm)
