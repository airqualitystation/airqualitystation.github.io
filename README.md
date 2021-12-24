# Air Quality Station

![Fire at Grenoble 20-11-2021](images/FEpQweSWUAI8UEH.jpg)

This project proposes the hardware design and the firmware of a low-cost air quality station for citizens.
Air quality measurements are transmitted over a private or public LoRaWAN network ([Helium](https://explorer.helium.com/), [TTN](https://www.thethingsnetwork.org/) or self-hosted Chirpstack) and displayed as open data ([luftdaten](https://luftdaten.info/), [opensensemap](https://opensensemap.org/)) or in private dashboard ([cayenne](https://accounts.mydevices.com), [thingsboard.io](https://thingsboard.io/)).
The firmware is based on [RIOT OS](https://riot-os.org/).
The IAQ sensors are listed [here](./sensors.md)

[Github repositories](https://github.com/airqualitystation)

## Version 2022
Coming soon
* MCU: STM32WL55 ([Nucleo](https://www.st.com/en/evaluation-tools/nucleo-wl55jc.html), [Seeedstudio](https://wiki.seeedstudio.com/LoRa_E5_Dev_Board/))
* Sensors:
  * Temperature, Humidity, Pressure
  * [CCS811](https://github.com/airqualitystation/firmware/blob/master/ccs811.md) air quality sensor.
  * [SGP30](https://wiki.seeedstudio.com/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/) air quality sensor.
  * [Geiger counter with UART](https://www.sparkfun.com/products/retired/10742)
  * Others to defined
* Firmware : C or MicroPython on RIOT OS

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

## Partners
* [Polytech Grenoble, Université Grenoble Alpes](https://www.polytech-grenoble.fr/)
* [Phelma, Grenoble INP](https://phelma.grenoble-inp.fr/)
* [ATMO Auvergne-Rhône-Alpes](https://www.atmo-auvergnerhonealpes.fr/)
