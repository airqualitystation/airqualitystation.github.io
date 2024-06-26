# Air Quality Station

![Fire at Grenoble 20-11-2021](images/FEpQweSWUAI8UEH.jpg)
Credit: [@villeofficiel](https://twitter.com/villeofficiel/status/1462069831444967427)

This project proposes the hardware design and the firmware of various low-cost and repairable airquality stations for citizens.
Air quality measurements are transmitted over a private or public LoRaWAN network ([Helium](https://explorer.helium.com/), [TTN](https://www.thethingsnetwork.org/) or self-hosted Chirpstack) and displayed as open data ([luftdaten](https://luftdaten.info/), [opensensemap](https://opensensemap.org/)) or in private dashboard ([cayenne](https://accounts.mydevices.com), [thingsboard.io](https://thingsboard.io/)).
The firmware is based on [RIOT OS](https://riot-os.org/).
The IAQ sensors are listed [here](./sensors.md)

[Github repositories](https://github.com/airqualitystation)

## Version 2024 (WIP)

### Flipper Zero with BME680 and PMS7003
* Board: [Flipper Zero](https://github.com/CampusIoT/tutorial/blob/master/flipper_zero/README.md)
* Sensors:
  * BME280: Temperature, Humidity, Pressure
  * PMS7003: PM 1, 2.5, 10
* FAP: https://lab.flipper.net/apps/airmon

[Project (HW+SW)](https://github.com/airqualitystation/flipper_zero/blob/main/README.md)

### ESP32 DevKit with BME280 and Sensirion SPS30
* Board: ESP32 DevKit on [TinyGS_2G4](https://github.com/thingsat/tinygs_2g4station)
* Sensors:
  * [MIKROE-1978 (BME280)](https://www.mikroe.com/weather-click) on Mikrobus Slot 1: Temperature, Humidity, Pressure
  * [Sensirion SPS30 PM Sensor](https://sensirion.com/products/catalog/SPS30/) on Grove I2C connector: PM 1, 2.5, 10
* Connectivity: Wifi, BLE, LoRaWAN (Mikrobus RN2483 on Mikrobus Slot 0)
* Firmware : [RIOT OS](https://doc.riot-os.org/group__boards__esp32__wroom-32.html)

![ESP32 DevKit + RN2483](https://raw.githubusercontent.com/thingsat/tinygs_2g4station/main/images/tinygs2G4_mikrobus_rn2483.jpg)

### RAK3172 with BME680 and PMS7003
* Board: [RAK3172](https://store.rakwireless.com/products/wisduo-lpwan-module-rak3172) : MCU [STM32WLE5](https://www.st.com/en/microcontrollers-microprocessors/stm32wlex.html)
* Sensors:
  * [BME680](https://www.bosch-sensortec.com/products/environmental-sensors/gas-sensors/bme680/) : Temperature, Humidity, Pressure
  * [PMS7003](https://www.plantower.com/en/products_33/76.html): PM 1, 2.5, 10 (2x10 2mm header)
  * [LIS2DH12](https://www.st.com/en/mems-and-sensors/lis2dh12.html) : MEMS digital output motion sensor: ultra-low-power high-performance 3-axis "femto" accelerometer
  * Grove connectors for UART (x2), I2C (x1), Analog GPIO (x2) and Digital GPIO (x1)  
* Power: MPPT for LiPo battery and solar panel (coming soon)
* Connectivity: LoRaWAN, [LoRa Mesh](https://meshtastic.org/) (coming soon)
* Firmware : [RIOT OS](https://github.com/RIOT-OS/RIOT/tree/master/boards/nucleo-wl55jc), [STM32CubeIDE](https://docs.rakwireless.com/Product-Categories/WisDuo/RAK3172-Module/Low-Level-Development/#rak3172-on-stm32cubeide-with-stm32wl-sdk-v1-2-0)

![PCB](images/ih2m-rak-top.png)

## Version 2022

### LoRa E5 Mini with BME280 and PMS7003
* Board: LoRa E5 Mini (STM32WL55J1)
* Sensors:
  * BME280: Temperature, Humidity, Pressure
  * PMS7003: PM 1, 2.5, 10
* [Firmware : RIOT OS](https://github.com/airqualitystation/firmware_for_bmx280_pms7003)
* [Decoder](https://github.com/airqualitystation/firmware_for_bmx280_pms7003/blob/main/codec/decoder.js)
* [Poster](presentations/poster_uspn_mlaix.pdf) [Paper](https://www.sciencedirect.com/science/article/pii/S0048969723026840?dgcid=author) [PhD Thesis (in french)](https://theses.fr/s245973)

![LoRa E5 Mini with BME280 and PMS7003](https://raw.githubusercontent.com/airqualitystation/firmware_for_bmx280_pms7003/main/images/aq_endpoint-02.jpg)
![Dashboard](images/aq_station_lora_e5_dashboard.png)

### Wio Terminal
* MCU: [Seeedstudio](https://wiki.seeedstudio.com/LoRa_E5_Dev_Board/)), [Wio Terminal](https://github.com/CampusIoT/tutorial/tree/master/wioterminal)
* Sensors:
  * Temperature, Humidity, Pressure
  * [CCS811](https://github.com/airqualitystation/firmware/blob/master/ccs811.md) air quality sensor.
  * [Grove CO2 SGP30](https://wiki.seeedstudio.com/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/) .
  * [Grove CO2 SDC41](https://wiki.seeedstudio.com/Grove-CO2-Temperature-Humidity-Sensor-SCD41/) 
  * [Grove - Gas Sensor V2(Multichannel)](https://wiki.seeedstudio.com/Grove-Multichannel-Gas-Sensor-V2/) for detecting CO, NO2, C2H5CH, VOC  with [GM-102B, GM-302B, GM-502B and GM-702B sensors](https://www.cnwinsen.com/products/MEMS-sensor)
  * [Geiger counter with UART](https://www.sparkfun.com/products/retired/10742)
  * Others to defined
* Firmware : Arduino or RIOT OS

![Wio Terminal SCD41](https://raw.githubusercontent.com/CampusIoT/tutorial/master/wioterminal/examples/GroveCO2TemperatureHumiditySensorSCD41/GroveCO2TemperatureHumiditySensorSCD41.jpg)

## Version 2021
* MCU: STM32WL55 ([Nucleo](https://www.st.com/en/evaluation-tools/nucleo-wl55jc.html), [Seeedstudio](https://wiki.seeedstudio.com/LoRa_E5_Dev_Board/))
* Sensor: [CCS811](https://github.com/airqualitystation/firmware/blob/master/ccs811.md) air quality sensor.
* Firmware : C on RIOT OS

## Version 2020

* MCU: [STM32 Nucleo B-L072Z-LRWAN1](https://www.st.com/en/evaluation-tools/b-l072z-lrwan1.html).
* Firmware : C on RIOT OS

![Air Quality Polytech Project Station](images/Station_meteo)

![Air Quality Polytech Project Grafana](images/Projet_Qualite_Air_Grafana_Dashboard.JPG)

Youtube: https://www.youtube.com/playlist?list=PLF3XltIz6OpR8-TI78mwKeDekHcQkxyBV

## Version 2019

* MCU: [P-NUCLEO-LRWAN1](https://www.st.com/en/evaluation-tools/p-nucleo-lrwan1.html).
* Firmware : MBed

![Air Quality Station v1](images/atmo-station-d.jpg)
![Air Quality Dashboard](images/atmo-nodered-3.png)

## Partners & Supporters
* [Labex Persyval Labs, Université Grenoble Alpes](https://persyval-lab.org/)
* [Polytech Grenoble, Université Grenoble Alpes](https://www.polytech-grenoble.fr/)
* [Fablab MaSTIC, Université Grenoble Alpes](https://fabmstic.imag.fr/)
* [Phelma, Grenoble INP](https://phelma.grenoble-inp.fr/)
* [ATMO Auvergne-Rhône-Alpes](https://www.atmo-auvergnerhonealpes.fr/)

## Misc
* [AQ Poster (in french)](https://www.ecologie.gouv.fr/sites/default/files/15104-2_expo-QA_10-panneaux_A4_HD.pdf)

