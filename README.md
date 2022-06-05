# STM32duino  BoardManagerFiles for arm64

This is an Arduino Boardmanagerfile. 
This allows you to develop Arduino sketches for STM32 arm boards (Blue Pill) on Raspberry Pi 64-bit.

By itself, the [Arduino IDE](https://www.arduino.cc/en/Main/Software) does not support STM32 arm processors. This software for arm linux adds support for STM32 arm processors to the Arduino IDE.

To use, start  the Arduino IDE on your raspberry. In *File --> Preferences --> Additional Board Manager URLs:* paste the following url:

``https://raw.githubusercontent.com/koendv/BoardManagerFiles/master/package_stmicroelectronics_index.json``

Press OK.

Open *Tools -> Board: -> Boards Manager*
In the search field, type "STM32". Install the "STM32 Cores" board package. Instalation takes some time.

In the Tools menu select the STM32 cores as compilation target. As an example, if using a STM32F103 Blue Pill choose *Tools->Board: -> Generic STM32F1 series* .

## credit

Raspberry version adapted from the [original for intel linux](https://github.com/stm32duino/BoardManagerFiles)