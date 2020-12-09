
[![Arduino CI](https://github.com/RobTillaart/AM232X/workflows/Arduino%20CI/badge.svg)](https://github.com/marketplace/actions/arduino_ci)
[![License: MIT](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/RobTillaart/AM232X/blob/master/LICENSE)
[![GitHub release](https://img.shields.io/github/release/RobTillaart/AM232X.svg?maxAge=3600)](https://github.com/RobTillaart/AM232X/releases)

# AM232X

Arduino library for AM2320 AM2321 and AM2322 I2C temperature and humidity sensor

## Description

AM232X is a sensor similar to the DHT12 with an I2C interface. 
Although in theory this could enable multiple sensors on one bus
the AM232X has a fixed address **0x5C** so 

Typical parameters

|        |  range | accuracy | repeatability
|:-------|:------:|:------:|:------:|
| Temperature | -40 - 80   | 0.5°C  | ±0.1 |
| Humidity    | 0.0 - 99.9 | 3%     | ±0.1 |
| Sample time | 2 seconds  |        |      |



## Interface

### Constructor

- **AM232X()** constructor
- **begin(uint8_t sda, uint8_t scl)** for ESP32
- **begin()** for AVR


### Base calls

- **read()**
- **getHumidity()**
- **getTemperature()**


### Misc

- **getModel()** 
- **getVersion()**
- **getDeviceID()**
- **getStatus()**
- **getUserRegisterA()**
- **getUserRegisterB()**
- **setStatus(uint8_t value)**
- **setUserRegisterA(int value)**
- **setUserRegisterB(int value)**


## Operation

See examples


## Planned changes

Fix several TODO's in the code.


## Warning

The library has several open ends so use at own risk.

See also LICENCE
