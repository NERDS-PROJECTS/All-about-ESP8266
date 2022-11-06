# All-about-ESP8266
[ESP8266.docx](https://github.com/NERDS-PROJECTS/All-about-ESP8266/files/9945195/ESP8266.docx)

The ESP8266 is a low-cost Wi-Fi microchip, with built-in TCP/IP networking software, and
microcontroller capability, produced by Espressif Systems in Shanghai, China.


The chip was popularized in the English-speaking maker community in August 2014 via the ESP01 module, made by a third-party manufacturer Ai-Thinker. This small module allows microcontrollers to connect to a Wi-Fi network and make simple TCP/IP connections using Hayes-style commands. However, at first, there was almost no English-language documentation on the chip and the commands it accepted. The very low price and the fact that there were very few external components on the module, which suggested that it could eventually be very inexpensive in volume, attracted many hackers to explore the module, the chip, and the software on it, as well as to translate the Chinese documentation.

The ESP8285 is a similar chip with a built-in 1 MiB flash memory, allowing the design of singlechip devices capable of connecting via Wi-Fi.

These microcontroller chips have been succeeded by the ESP32 family of devices.


| List 1 | List 2 |
| --- | --- |
| Manufacturer | Espressif Systems |
| Type	| 32-bit microcontroller |
| CPU |	Tensilica Diamond  Standard 106Micro (aka. L106) @ 80 MHz (default) or 160 MHz |
| Memory	| 32 KiB instruction,80 KiB user data |
| Input |	17 GPIO pins |
| Power |	3.3 V DC |
| Successor |	ESP32 |


![image](https://user-images.githubusercontent.com/116709965/200155376-093cb2a3-8f5f-46d6-8de5-3c066668db0f.png)

The pinout is as follows for the common ESP-01 module:
1.	GND, Ground (0 V)
2.	GPIO 2, General-purpose input/output No. 2
3.	GPIO 0, General-purpose input/output No. 0
4.	RX, Receive data in, also GPIO3
5. VCC, Voltage (+3.3 V; can handle up to 3.6 V)
6. RST, Reset
7. CH_PD, Chip power-down
8. TX, Transmit data out, also GPIO1

In October 2014, Espressif Systems released a software development kit (SDK) for programming
the chip directly, which removed the need for a separate microcontroller.Since then, there have
been many official SDK releases from Espressif; Espressif maintains two versions of the SDK —
one that is based on FreeRTOS and the other based on callbacks.

### SDKs

An alternative to Espressif's official SDK is the open-source ESP-Open-SDK that is based on the GNU Compiler Collection (GCC) toolchain, maintained by Max Filippov.Another alternative is the "Unofficial Development Kit" by Mikhail Grigorev.

Other SDKs, mostly open-source, include:

* Arduino — A C++-based firmware. With this core, the ESP8266 CPU and its Wi-Fi components can be programmed like any other Arduino device. The ESP8266 Arduino Core is available through GitHub (https://github.com/esp8266/Arduino).

* ESP8266 BASIC (http://www.esp8266basic.com/) — An open-source BASIC-like interpreter specifically tailored for the Internet of Things (IoT). Self-hosting browser-based development environment.

* ESP Easy — Developed by home automation enthusiasts.

* ESPHome (https://esphome.io/index.html) — ESPHome is a system to control your	ESP8266 Die shot ESP8266/ESP32 by simple yet powerful configuration files and control them remotely through home automation systems.

* Tasmota (https://github.com/arendst/Sonoff-Tasmota) - open-source firmware, for home automation.

* ESP-Open-RTOS (https://github.com/SuperHouse/esp-open-rtos) — Open-source FreeRTOS-based ESP8266 software framework.

* ESP-Open-SDK (https://github.com/pfalcon/esp-open-sdk) — Free and open (as much as possible) integrated SDK for ESP8266/ESP8285 chips.

* Espruino — An actively maintained JavaScript SDK and firmware, closely emulating Node.js. Supports a few MCUs, including the ESP8266.

* ESPurna (https://github.com/xoseperez/espurna/wiki) — Open-source ESP8285/ESP8266 firmware.


* Forthright (https://github.com/niclash/forthright) — Port of Jones Forth to the ESP8266 microcontroller.

* MicroPython (https://micropython.org/) — A port of MicroPython (an implementation of Python for embedded devices) to the ESP8266 platform.

* Moddable SDK (https://github.com/Moddable-OpenSource/moddable#supported-hardware) — includes JavaScript language and library support for the ESP8266
* Mongoose OS — An open-source operating system for connected products. Supports ESP8266 and ESP32. Develop in C or JavaScript.

* NodeMCU — A Lua-based firmware.

* PlatformIO (https://platformio.org/platforms/espressif8266) — A cross-platform IDE and unified debugger, which sits
on top of Arduino code and libraries.

* Punyforth (https://github.com/zeroflag/punyforth) — Forth-inspired programming language for the ESP8266.

* Sming (https://github.com/SmingHub/Sming) — An actively developed asynchronous C/C++ framework with superb performance and multiple network features.

uLisp (http://www.ulisp.com/show?21T5) — A version of the Lisp programming language specifically designed to run on processors with a limited amount of RAM.

ZBasic for ESP8266 (http://www.zbasic.net) — A subset of Microsoft's widely-used Visual Basic 6, which has been adapted as a control language for the ZX microcontroller family and the ESP8266.

Zerynth — IoT framework for programming ESP8266 and other microcontrollers in Python. IOTBAH - is An operating system (OS) for Espressif ESP8266

### References
 
1.	"ESP8266 Overview" (http://espressif.com/en/products/hardware/esp8266ex/overview). Espressif Systems. Retrieved 2017-10-02.
2.	Brian Benchoff (August 26, 2014). "New Chip Alert: The ESP8266 WiFi Module (It's $5)" (http://hackaday.com/2014/08/26/new-chi p-alert-the-esp8266-wifi-module-its-5/). Hackaday. Retrieved 2015-06-24.
3.	Brian Benchoff (September 6, 2014). "The Current State of ESP8266 Development" (http://hackaday.com/2014/09/06/the-current-s tate-of-esp8266-development/). Hackaday. Retrieved 2015-06-24.
4.	"Espressif Announces ESP8285 Wi-Fi Chip for Wearable Devices" (https://espressif.com/en/media_overview/news/espressif-anno unces-esp8285-wi-fi-chip-wearable-devices). Espressif Systems. Mar 9, 2016. Retrieved 2016-07-10.
5.	"ESP8266 Non-OS SDK API Reference, Chapter 2.4. System Performance" (https://www.espressif.com/sites/default/files/docume ntation/2c-esp8266_non_os_sdk_api_reference_en.pdf#page=19) (PDF). espressif.com. Espressif Systems. 
The flash mode and frequency directly influence the code execution speed. Setting the flash to a higher frequency and QIO mode may produce the best results in terms of performance, though it costs in terms of power consumption. "ESP8266 Non-OS SDK API Reference" (https://www.espressif.com/sites/default/files/documentation/2c-esp8266_non_os_sdk_api_reference_en.pdf) (PDF). espressif.com. Espressif Systems.  Success varies chip to chip.
6.	"ESP8266 Non-OS SDK API Reference, Chapter 2.5. System Memory" (https://www.espressif.com/sites/default/files/documentatio n/2c-esp8266_non_os_sdk_api_reference_en.pdf#page=20) (PDF). espressif.com. Espressif Systems.
7.	"ESP8266 Technical Reference, Version 1.7" (https://www.espressif.com/sites/default/files/documentation/esp8266-technical_refer ence_en.pdf) (PDF). Espressif Systems. Retrieved 2021-04-22.
8.	"Espressif ESP8266 Developer Zone Discussion Forum: Does ESP8266 actually have hardware I2C?" (http://bbs.espressif.com/vi ewtopic.php?t=1032#p5449). Espressif Systems. 2014-10-27. Retrieved 2017-10-02.
9.	Brian Benchoff (October 25, 2014). "An SDK for the ESP8266 WiFi Chip" (http://hackaday.com/2014/10/25/an-sdk-for-the-esp8266 -wifi-chip/). Hackaday. Retrieved 2015-06-24.
10.	"Official SDK release from Espressif for ESP8266" (http://bbs.espressif.com/viewforum.php?f=46/). Espressif Systems. July 29, 2015. Retrieved 2015-08-08.
11.	Paul Sokolovsky. "esp-open-sdk: Free and open (as much as possible) integrated SDK for ESP8266/ESP8285 chips" (https://githu b.com/pfalcon/esp-open-sdk).
12.	Max Filippov (February 15, 2015). "ESP8266 GCC Toolchain" (https://github.com/esp8266/esp8266-wiki/wiki/Toolchain). Retrieved 2015-08-08.
13.	Mikhail Grigorev. "Unofficial Development Kit for Espressif ESP8266 (GitHub Repository)" (https://github.com/CHERTS/esp8266-d evkit).
14.	Mikhail Grigorev. "Project Unofficial Development Kit for Espressif ESP8266" (http://programs74.ru/udkew-en.html).
15.	"Mongoose OS Documentation" (https://mongoose-os.com/docs/quickstart/setup.html). Cesanta.
