# Better Fridge - Home Assistant Custom Component

An improvement over the standard Generic Thermostat component, designed to provide better control and monitoring of your refrigerator's temperature.

## Hardware Requirements

- A HA temperature sensor placed inside the fridge to monitor the internal temperature.
- A HA switch or relay to power the firdge's compressor on and off.

## Features (in progress)

- [X] Closed loop temperature control to maintain the desired fridge temperature. (based on the standard Generic Thermostat behavior)
- [ ] Protection against temperature sensor errors to prevent the compressor from running indefinitely. 
  - [ ] A timeout mechanism will be implemented to turn off the compressor if the sensor fails to report a valid temperature for a certain period.
  - [ ] Automatic resume of normal operation once the sensor starts reporting valid temperatures again.
  - [ ] HA notifications to alert the user of sensor issues and compressor status.
- [ ] Configurable maximum compressor run time to prevent potential damage from prolonged operation.
- [ ] Optional integration with additional temperature sensor from internal fridge cooling unit for preventing ice buildup and ensuring optimal cooling performance.
- [ ] Optional TIME Mode to allow for operation without a temperature sensor, using fixed on/off durations to control the compressor. This mode will be useful for users who do not have a compatible temperature sensor or prefer a simpler control method.
