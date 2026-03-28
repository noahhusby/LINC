<img src="/graphics/Linc_Logo.png" width="850">

## About

This project came about from the need to control my PM2812 dual-channel power supply manufactured by the Phillips and Fluke consortium in the mid 90s. While later revisions of this device did feature a serial port, the earlier versions (such as mine) were stuck with the GPIB/HP-IP interface. This interface was used on test equipment up until the mid 2010s and yet there is no simple or affordable way to communicate with it. The interface chips for GPIB are no longer manufactured and difficult to source. 

The goal of this project is to create a controller that can translate commands from a networked device (either over LAN or RS485) to the PM2812 power supply. This would allow for a desk-mounted control panel with a modern OLED display and tactile controls to replace the dated "system power supply-type" interface found on the PM2812.

## Features

- Console Control 💾
  - Virtual COM port allows direct control of test equipment over integrated USB-C port
- Modern Hardware 💻
  - Based upon STM32H533 using new level shifters instead of legacy/unavailable SN7515x series chips
- Remote Control Capability 🛜
  - Integrated RS485 port for secondary physical control panel 

## Related

- LeHuman/[PMPi](https://github.com/LeHuman/PMPi)
- mnemocron/[gpibusb-firmware-stm32](https://github.com/mnemocron/gpibusb-firmware-stm32)

## License

This project is licensed under the `MIT License`.
