# TEF_ESP
A continuation of Sjef's (PE5PVB) project called TEF6686_ESP32-v1.

This software is designed for tuners based on original PE5PVB board.

More info: https://www.pe5pvb.nl/tef6686/

## What's new?
- RDS TP indicator
- RDS data storing
- signal meter in dBf or dBµV
- XDR-GTK control over Wi-Fi
- new visual themes
- various visual fixes

## TO DO
- battery level indicator (with instructions of connecting)
- add photos of working tuner
- LW/MW/SW bandplan

## Instalation
**Recommended method:** You can download already compiled software and upload it using prepared script from release page. Instructions are included in the archive.

**Alternative method:** You can download source code from release page or using git. Then compile and upload it using for example Arduino IDE. **Important** you need to fill your TEF_eSPI.h file (probably located in Arduino/libraries/TFT_eSPI folder) with these values:
```
#define ILI9341_DRIVER
#define TFT_CS          5
#define TFT_DC          17
#define TFT_RST         16
#define LOAD_GLCD
#define LOAD_FONT2
#define LOAD_FONT4
#define LOAD_FONT6
#define LOAD_FONT7
#define LOAD_FONT8
#define LOAD_GFXFF
#define SMOOTH_FONT
#define SPI_FREQUENCY   10000000
```
**ALL OTHER SETTINGS SHOULD BE REMARKED!**
  

## License
This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 2 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details. 
