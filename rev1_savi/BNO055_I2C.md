# BNO055 9-DOF IMU (I2C Mode)

Source: Bosch BNO055 Datasheet
https://cdn-shop.adafruit.com/datasheets/BST_BNO055_DS000_12.pdf

The BNO055 is a 9-degree-of-freedom absolute orientation sensor integrating a 3-axis accelerometer, gyroscope, and magnetometer, with on-chip sensor fusion. This component is used as the primary inertial sensing unit for orientation and motion tracking.

## Interface
- Communication protocol: I2C
- Default I2C address: 0x28 (can be changed to 0x29)
- Logic level: 3.3 V

## Power
- VDD (Pin 3): Core supply
- VDDIO (Pin 28): I/O supply
- GND / GNDIO (Pins 2, 10, 15, 16, 25)

## I2C Pins
- I2C_SDA (Pin 20): Bidirectional data
- I2C_SCL (Pin 19): Clock input

## Control and Configuration Pins
- nRESET (Pin 11): Active-low reset
- INT (Pin 14): Interrupt output
- PS0 (Pin 6), PS1 (Pin 5): Protocol select pins (configured for I2C)
- nBOOT_LOAD_PIN (Pin 4): Bootloader mode select

## Notes
- Sensor fusion is performed on-chip, reducing host processing load.
- Only I2C mode is supported in the current system architecture.
- UART, HID-I2C, and external oscillator pins are not used.
- Do-not-connect (DNC) pins are omitted from the schematic symbol.
