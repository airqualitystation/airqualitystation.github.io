# Air Quality Sensors and Products

## Products

### MCF88

* [MCF-LW12TER LoRaWAN® indoor environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12ter/)
* [MCF-LW12TERPM LoRaWAN® outdoor PM and environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12terpm/)
* [MCF-LW12CO2 LoRaWAN® indoor environmental sensor with VOC, LUX and CO2](https://www.mcf88.it/prodotto/mcf-lw12co2/)
* [MCF-LW12TERWP LoRaWAN® outdoor environmental sensor](https://www.mcf88.it/prodotto/mcf-lw12terwp/)

Note: MCF88 endpoints transmit air quality measurements by using the LoRaWAN protocol. The payload decoder is available [here](https://github.com/CampusIoT/payload-codec/tree/master/src/main/ttn_loraappserver/mcf88).

### NetAtmo

## Boards

### Breakout Qwiic

| Board         | Samples @ Fablab | Voltage   | Interface | Sensors | OS Support | Fritzing | Demo     |
| ------------- | ---------------- | --------- | ----------| ------- | ---------- | -------- | -------- |
| [SparkFun Environmental Combo Breakout - CCS811/BME280](https://www.sparkfun.com/products/14348) | 0 | TBC | I2C | CCS811, BME280 | Riot OS: TBC, MBed: TBC, Stm32duino: TBC | TBC | TBC |

Note: [SparkFun's Qwiic Connect System](https://www.sparkfun.com/qwiic) uses 4-pin JST connectors to quickly interface development boards with sensors, LCDs, relays and more.

### Seeed Studio Grove sensors

[Manufacturer full list](https://www.seeedstudio.com/category/Sensor-for-Grove-c-24.html)

| Sensors       | Samples @ Fablab | Voltage   | Sensors       | OS support | Fritzing     | Demo     |
| ------------- | ---------------- | --------- | ------------- | ---------- | ------------ | -------- |
| [Dust Sensor](http://wiki.seeedstudio.com/Grove-Dust_Sensor/) |  TBC | 5V | Ultrasonic | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ2)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ2/) Combustible Gas, Smoke |  TBC | 5V | MQ2 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ3)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ3/) Alcohol Vapor |  TBC | 5V | MQ3 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ5)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ5/) LPG, Natural Gas, Town Gas |  TBC | 5V | MQ5 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |
| [Gas Sensor (MQ9)](http://wiki.seeedstudio.com/Grove-Gas_Sensor-MQ9/) Carbon Monoxide, Coal Gas, Liquefied Gas |  TBC | 5V | MQ9 | RiotOS: TBD, Stm32duino: TBD | TBD | TBD |

### Others

| Board         | Samples @ Fablab | Voltage   | Interfaces | Sensors       | OS support | Fritzing     | Demo     |
| ------------- | ---------------- | --------- | --------- | ------------- | ------- | ------------ | -------- |
| [SparkFun Air Quality Breakout - CCS811](https://www.sparkfun.com/products/14193) | 1 | 3.3V | I2C | VOC | TBC | TBC | TBC |
| [SparkFun Particle Sensor Breakout - MAX30105](https://www.sparkfun.com/products/14045) | TBC | 5V | I2C | Particles | TBC | TBC | TBC |

## Components

* [MAX30105](https://cdn.sparkfun.com/assets/learn_tutorials/5/7/7/MAX30105_3.pdf)
* [CCS811](https://cdn.sparkfun.com/assets/learn_tutorials/1/4/3/CCS811_Datasheet-DS000459.pdf)
