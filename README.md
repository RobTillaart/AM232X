# AM232X

Arduino library for AM2320 AM2321 and AM2322 I2C temperature and humidity sensor

## Description

AM232X is a sensor similar to the DHT12 with an I2C interface. 
Although in theory this could enable multiple sensors on one bus
the AM232X has a fixed address 0x5C.

## Operation

In setip() you have to call the **AM232X.begin()** to initialize 
the Wire library and do an initial **read()** to fill the variables
**AM232X.temperature** and **AM232X.humidity**. 


## Planned changes
The two variables will be replaced by two functions in an upcoming
breaking version of the lib. This to prevent writing to the two
variables.

Fix several TODO's in the code.

## Warning
The library has several open ends so it is not suitable yet for
any serious application. 

See also LICENCE
