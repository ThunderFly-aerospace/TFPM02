# TFPM02A - Particulate Matter Sensor for ThunderFly TF-ATMON system

[Particulate matter](https://en.wikipedia.org/wiki/Particulates) sensor for [TF-ATMON system](https://github.com/ThunderFly-aerospace/TF-ATMON) is based on [Sensirion SPS30](https://sensirion.com/products/catalog/SPS30/), [TFGPS01](https://github.com/ThunderFly-aerospace/TFGPS01) and PX4 autopilot firmware with suitable driver. The PX4 driver emits uOrb messages which are translated to [MAVLink](https://en.wikipedia.org/wiki/MAVLink) messages ready to log onboard and transmit to [TF-ATMON enabled GCS](https://github.com/ThunderFly-aerospace/TF-GCS01). 

Look to the following video for a demonstration flight of a sensor mounted on [TF-G2 autogyro](https://github.com/ThunderFly-aerospace/TF-G2). 

[![TF-ATMON particulate matter sensing demonstration](https://img.youtube.com/vi/KUhktPDEi8I/hqdefault.jpg)](https://www.youtube.com/watch?v=KUhktPDEi8I)

## The main features

 - Particulate matter mass concentration PM1.0, PM2.5, PM4 and PM10 in range 0 - 1000 μg/m³ (Accuracy ±10 %)
 - Number concentration for PM0.5, PM1, PM2.5, PM4 and PM10 in range 0 to 3000 #/cm3 
 
Humidity Temperature measurement required to correct interpretation of measured data is not provided directly by the TFPM02A sensor itself. Please use the [TFHT01](https://github.com/ThunderFly-aerospace/TFHT01) to get the humidity and temperature data.

## Usage

The modified [SPS30](https://sensirion.com/products/catalog/SPS30/) sensor is directly connected to the PX4 autopilot supported hardware by using ZHR-5 to JST-GH cable. 

![Bottom view on TFPM02A particulate matter sensor](doc/img/TFPM02_bottom.jpg)

![Top view on TFPM02A particulate matter sensor](doc/img/TFPM02_top.jpg)
