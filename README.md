# ESP8266 Arduino Core for ESP8266 Deauther Project

This repository is a fork of the [ESP8266 Arduino Core](https://github.com/esp8266/Arduino) to include libraries, boards and modifications necessary to compile the [ESP8266 Deauther](https://github.com/spacehuhntech/esp8266_deauther) project.  
The goal of this is to have a simpler installation setup for anyone that likes to test, modify and contribute to the deauther project.  

## License and credits

Arduino IDE is developed and maintained by the Arduino team. The IDE is licensed under GPL.

ESP8266 core includes an xtensa gcc toolchain, which is also under GPL.

Esptool.py was initially created by Fredrik Ahlberg (@themadinventor, @kongo), and is currently maintained by Angus Gratton (@projectgus) under GPL 2.0 license.

Espressif SDK included in this build is under Espressif MIT License.

ESP8266 core files are licensed under LGPL.

[SPI Flash File System (SPIFFS)](https://github.com/pellepl/spiffs) written by Peter Andersson is used in this project. It is distributed under the MIT license.

[umm_malloc](https://github.com/rhempel/umm_malloc) memory management library written by Ralph Hempel is used in this project. It is distributed under the MIT license.

[SoftwareSerial](https://github.com/plerup/espsoftwareserial) library and examples written by Peter Lerup. Distributed under LGPL 2.1.

[axTLS](http://axtls.sourceforge.net/) library written by Cameron Rich, built from https://github.com/igrr/axtls-8266, is used in this project. It is distributed under [BSD license](https://github.com/igrr/axtls-8266/blob/master/LICENSE).

[BearSSL](https://bearssl.org) library written by Thomas Pornin, built from https://github.com/earlephilhower/bearssl-esp8266, is used in this project.  It is distributed under the [MIT License](https://bearssl.org/#legal-details).

[LittleFS](https://github.com/ARMmbed/littlefs) library written by ARM Limited and released under the [BSD 3-clause license](https://github.com/ARMmbed/littlefs/blob/master/LICENSE.md).

[uzlib](https://github.com/pfalcon/uzlib) library written and (c) 2014-2018 Paul Sokolovsky, licensed under the ZLib license (https://www.zlib.net/zlib_license.html). uzlib is based on: tinf library by Joergen Ibsen (Deflate decompression); Deflate Static Huffman tree routines by Simon Tatham; LZ77 compressor by Paul Sokolovsky; with library integrated and maintained by Paul Sokolovsky.

[ArduinoJSON](https://github.com/bblanchon/ArduinoJson) written by Benoit BLANCHON is used in this project. It is distributed under the MIT license.  

[Adafruit Neopixel](https://github.com/adafruit/Adafruit_NeoPixel) maintained by Adafruit is used in this project. It is distributed under the LGPL-3.0 license.  

[esp8266-oled-ssd1306](https://github.com/ThingPulse/esp8266-oled-ssd1306) written by Daniel Eichhorn and Fabrice Weinberg is used in this project. It is distributed under the MIT license.  

[LinkedList](https://github.com/ivanseidel/LinkedList) written by Ivan Seidel is used in this project. It is distributed under the MIT license.  

[SimpleButton](https://github.com/spacehuhn/SimpleButton) written by Stefan Kremser is used in this project. It is distributed under the MIT license.  

[SimpleCLI](https://github.com/spacehuhn/SimpleCLI) written by Stefan Kremser is used in this project. It is distributed under the MIT license.  

[ESPAsyncTCP](https://github.com/me-no-dev/ESPAsyncTCP) written by Hristo Gochkov is used in this project. It is distributed under the GNU Lesser General Public License.  

[ESPAsyncWebServer](https://github.com/me-no-dev/ESPAsyncWebServer) written by Hristo Gochkov is used in this project. It is distributed under the GNU Lesser General Public License.  

## Modifications

* Added [SimpleCLI library](https://github.com/spacehuhn/SimpleCLI)
* Added [ESPAsyncTCP library](https://github.com/me-no-dev/ESPAsyncTCP)
* Added [ESPAsyncWebServer library](https://github.com/me-no-dev/ESPAsyncWebServer)
* Modified boards.txt.py and boards.txt and platform.txt to add deauther boards and change default values
* Patched libnet802.11a to allow for packet injection
* Modified platform.txt to change package name and add project specific compiler flags