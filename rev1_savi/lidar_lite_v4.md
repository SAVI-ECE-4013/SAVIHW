# LiDAR-Lite v4 Sensor

Source: Garmin LiDAR-Lite v4 LED datasheet
https://static.garmin.com/pumac/LIDAR-Lite%20LED%20v4%20Instructions_EN-US.pdf 

## Interface
- Power:
  - VIN (Pin 1) – 5 V
  - GND (Pin 2)
- I2C:
  - SDA (Pin 3) – Bidirectional
  - SCL (Pin 4) – Input
- Optional GPIO:
  - GPIOA (Pin 5)
  - GPIOB (Pin 6)
- Debug pins:
  - VRETURN (Pin 7)
  - nRESET (Pin 8)
  - SWCLK (Pin 9)
  - SWDIO (Pin 10)

## Notes
- Default I2C address: 0x62
- Max logic level: 3.3 V
- Debug pins not required for normal operation
