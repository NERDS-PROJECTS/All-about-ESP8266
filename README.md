# All-about-ESP8266
[ESP8266.docx](https://github.com/NERDS-PROJECTS/All-about-ESP8266/files/9945195/ESP8266.docx)

The ESP8266 is a low-cost Wi-Fi microchip, with built-in TCP/IP networking software, and
microcontroller capability, produced by Espressif Systems in Shanghai, China.


The chip was popularized in the English-speaking maker community in August 2014 via the ESP01 module, made by a third-party manufacturer Ai-Thinker. This small module allows microcontrollers to connect to a Wi-Fi network and make simple TCP/IP connections using Hayes-style commands. However, at first, there was almost no English-language documentation on the chip and the commands it accepted. The very low price and the fact that there were very few external components on the module, which suggested that it could eventually be very inexpensive in volume, attracted many hackers to explore the module, the chip, and the software on it, as well as to translate the Chinese documentation.

The ESP8285 is a similar chip with a built-in 1 MiB flash memory, allowing the design of singlechip devices capable of connecting via Wi-Fi.

These microcontroller chips have been succeeded by the ESP32 family of devices.

![image](https://user-images.githubusercontent.com/116709965/200156346-fc167358-d259-45a1-ab5f-8ce0dde63632.png)

ESP8266-IC
| List 1 | List 2 |
| --- | --- |
| Manufacturer | Espressif Systems |
| Type	| 32-bit microcontroller |
| CPU |	Tensilica Diamond  Standard 106Micro (aka. L106) @ 80 MHz (default) or 160 MHz |
| Memory	| 32 KiB instruction,80 KiB user data |
| Input |	17 GPIO pins |
| Power |	3.3 V DC |
| Successor |	ESP32 |

The ESP8266 modules are commonly found in the following IoT devices:
## ESP8266 Applications
* Smart security devices, including surveillance cameras and smart locks
* Smart energy devices, including HVACs and thermostats 
* Smart industrial devices, including Programmable Logic Controllers (PLCs) 
* Smart medical devices, including wearable health monitors

## Chip versus Modules versus Development Boards
As discussed above, the ESP8266 is just the name of the chip. There are essentially three formats you can buy this in:

* ESP8266 Chip: 
This is the basic chip manufactured by Espressif, which comes unshielded and needs to be soldered onto a module. This is unsuitable for most users, apart from perhaps volume device manufacturers that can factor this into the production process under the unit cost of a module.
* ESP8266 Modules: 
These are the surface-mountable modules that contain the chip, which are ready to be mounted onto an MCU, produced by Espressif, Ai-Thinker and certain other manufacturers. They are usually shielded and pre-approved by the FCC for use. This means they’re a good option for device manufacturers looking to scale production.
* ESP8266 Development Boards: 
These are the complete IoT MCU development boards that have the modules preinstalled. They’re used for developers and manufacturers to create prototypes during the design stage, before they start production. Development boards are produced by several different manufacturers and the specifications differ between models. Some core specifications to be aware of when assessing ESP8266 IoT development board options include:

  * GPIO pins
  * ADC pins
  * Wi-Fi antennas
  * LEDs
  * Shielding*
  * Flash Memory 

Many international markets require shielded Wi-Fi devices, as Wi-Fi produces considerable Radio Frequency Interference (RFI), and shielding minimizes this interference. This should, therefore, be a key consideration for all developers and embedded-device manufacturers.

## SDKs

There is now a wide range of software development kits (SDKs) available, enabling developers to program the chip directly without using a separate MCU. 

Espressif provides two official SDKs for use with ESP8266, which are:

* A FreeRTOS based SDK
* A Non-OS SDK
Aside from the Espressif options, there are plenty of commercial and open-source SDKs on the market, including:

* ESP Arduino Core – C++ based firmware
* ESP8266 BASIC – Open-source BASIC-like environment for IoT
* ESP-Open-RTOS – FreeRTOS open-source framework for ESP8266
* ESP-Open-SDK – Open integrated SDK for ESP8266
* Espruino – Javascript SDK and firmware
* Micropython – Python for embedded devices
* Moddable SDK – Javascript SDK
* Mongoose OS – C or Javascript open-source OS
* NodeMCU – Open-source Lua based firmware, similar to Node.js
* Sming – Asynchronous C/C++ framework
* uLisp – Lisp-based framework
* ZBasic – Visual Basic 6 adapted for ESP8266
* Zerynth – Python framework for IoT

## Which is the best ESP8266 Module or Development Board for IoT?

As the above comparisons show, there are many options available with ESP8266 IoT boards and modules. To help you with your decision making, we’ve summarized some of the most popular below.

#### Popular ESP8266 Modules

###### Ai-Thinker ESP-01
![image](https://user-images.githubusercontent.com/116709965/200157195-dfe93292-01e6-43a9-9fca-f1cca79f7e5d.png)

The ESP-01 is one of the biggest selling IoT Wi-Fi modules on the market. It’s widely used in smart home and networking projects.

The default AT firmware enables it to be used in combination with an Arduino. However, you can easily update the firmware with a USB-to-ESP-01 adaptor module.

A common complaint with this board is that the pin posts make it difficult to plug it directly into a breadboard, but this can be easily overcome by building or buying an adaptor module.

There are two versions available, one with 500kb of flash and the other with 1Mbit of flash.


###### Ai-Thinker ESP-05
![image](https://user-images.githubusercontent.com/116709965/200157239-54848747-0949-41d3-a2fe-01b2df6a20a6.png)

This module was developed to provide Wi-Fi connectivity for MCUs such as Raspberry Pi and PIC and other Wi-Fi projects. It, therefore, does not have GPIOS.

It fits into a breadboard without any problems, but there are some complaints about being stuck with the factory set firmware unless you’re prepared to do some serious modifications.


###### Ai-Thinker ESP-12
![image](https://user-images.githubusercontent.com/116709965/200157227-3ae50b77-0b22-492a-a291-b0091654c259.png)

This is a more fully featured module with 11 GPIO pins, an ADC, 4Mbits of flash, and 10-bit resolution. However, the module is not breadboard friendly, meaning you’ll need to use an adaptor. 

There are two versions available, ESP-12F, which has 20 GPIOS and ESP-12S, which has 14.

#### Popular ESP8266 Boards

###### Espressif NodeMCU module V1.0
![image](https://user-images.githubusercontent.com/116709965/200157217-d4e5f11e-5022-490a-9396-ed04838a88be.png)

This board has the ESP-12E module and comes with 4 Mbits of flash and features a row of pins on each side of the breadboard. The board comes with four communication interfaces: SPI, I2C, UART, and I2S, with 16 GPIO and one ADC. The RAM is 160KB, divided into 64KB for instruction and 96KB for data.


###### Adafruit Huzzah ESP8266 Breakout
![image](https://user-images.githubusercontent.com/116709965/200157212-3ca20349-b292-43c3-8398-b61094881157.png)

This microcontroller operates at a logic level of 3.3V and is clocked at 80MHz. It comes programmed with the Lua Interpreter, which makes programming simple, with no boot loading required. Alternatively, you can use the Arduino IDE to program it.

There is an onboard CP2104 USB-to-serial converter, therefore you can simply plug it into your computer and upload your code. The board is also lightweight and small, so it’s useful for projects with space constraints. 


###### WeMos D1 Mini

The WeMos D1 Mini was designed to be one of the smallest possible development boards for the ESP8266 module. It has a micro USB connection and compatibility with several firmware options.

## References
 
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
