# Icarus IoT Board (nRF9160 Feather)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark>$Format:%h$</mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-15</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/actinius-icarus-iot/board-iso.png "Icarus IoT Board (nRF9160 Feather)"

The **Icarus IoT Board** (Internet of Things) is a cost-effective cellular IoT
board in Adafruit's Feather(Wing) form factor. It is built around Nordic Semi's
nRF9160 (GEN2) modem and combines LTE-M & NB-IoT connectivity, GPS,
Accelerometer, SPI Flash, USB, LiPo charger as well as an eSIM with free data
out of the box and a nano SIM connector. All of this in a 22.8 x 50.8 mm package
with castellated pins.

* [nRF9160 SiP]: ARM Cortex-M33F (ARMv8-M) CPU, 1 MB Flash, 256 kB RAM, LTE-M/NB-IoT, GNSS
* [LIS2DH12]: 3-axis low-power accelerometer
* [W25Q64JV]: 64 Mbit SPI NOR Flash
* Reset and user button and RGB LED
* eSIM with SIM switch to optional SIM
* uFL connectors for LTE and GPS antenna
* LiPo Charger with MPPT
* Battery voltage measurement circuit
* Under- and Over-voltage protection
* FTDI USB to serial converter
* [Zephyr OS Support]

[nRF9160 SiP]: https://www.nordicsemi.com/Products/nRF9160 "ARM® Cortex M33 with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated LTE-M/NB-IoT modem and GNSS"
[LIS2DH12]: https://www.st.com/en/mems-and-sensors/lis2dh12.html "MEMS digital output 3-axis motion sensor"
[W25Q64JV]: https://www.winbond.com/hq/product/code-storage-flash-memory/serial-nor-flash/?__locale=en&partNo=W25Q64JV "64 Mbit SPI NOR Flash"
[Zephyr OS Support]: https://bridle.tiac-systems.net/doc/latest/zephyr/boards/arm/actinius_icarus/doc/index.html "Zephyr OS Support for Actinius Icarus IoT Board"

## References

* *HTML(2022-10-15)*: [Product Page] – *€112,95 (excl. VAT)*
* *HTML(2022-10-15)*: [Symbol and Footprint by SnapEDA]
  – *license protected, uploading to another website forbidden*

[Product Page]: https://www.actinius.com/icarus "Icarus IoT Board v2 (nRF9160 Feather)"
[Symbol and Footprint by SnapEDA]: https://www.snapeda.com/parts/Icarus%20IoT%20Board/Actinius/view-part/?ref=actinius "Created by SnapEDA and added to SnapEDA on Jul 29, 2022"

| Symbol | Footprint TH | Footprint SMD |
|::|::|::|
| <div style="background-color:white;">[![pcb-assembly-symbol]][pcb-assembly-symbol]</div> | <div style="background-color:black;"><div style="width:75%;display:inline-block;">[![pcb-assembly-footprint-th]][pcb-assembly-footprint-th]</div></div> | <div style="background-color:black;"><div style="width:75%;display:inline-block;">[![pcb-assembly-footprint-smd]][pcb-assembly-footprint-smd]</div></div> |
| | <div style="background-color:white;"><div style="width:33%;display:inline-block;">[![pcb-assembly-top]][pcb-assembly-top]</div></div> | <div style="background-color:white;"><div style="width:33%;display:inline-block;">[![pcb-assembly-bot]][pcb-assembly-bot]</div></div> |

[pcb-assembly-symbol]: electronic/boards/actinius-icarus-iot/pcb-assembly-symbol.png "Icarus IoT Board (nRF9160 Feather) Symbol"
[pcb-assembly-footprint-th]: electronic/boards/actinius-icarus-iot/pcb-assembly-footprint-th.png "Icarus IoT Board (nRF9160 Feather) Footprint TH"
[pcb-assembly-footprint-smd]: electronic/boards/actinius-icarus-iot/pcb-assembly-footprint-smd.png "Icarus IoT Board (nRF9160 Feather) Footprint SMD"
[pcb-assembly-top]: electronic/boards/actinius-icarus-iot/pcb-assembly-top.png "Icarus IoT Board (nRF9160 Feather) PCB Assembly (top)"
[pcb-assembly-bot]: electronic/boards/actinius-icarus-iot/pcb-assembly-bot.png "Icarus IoT Board (nRF9160 Feather) PCB Assembly (bottom)"

## Documentation

| Block Diagram |
|::|
| <div style="background-color:white;">[![board-blockdiag]][board-blockdiag]</div> |

[board-blockdiag]: electronic/boards/actinius-icarus-iot/board-blockdiag.png "Icarus IoT Board (nRF9160 Feather) Block Diagram"

* **PDF(2022-10-15)**: [Introduction]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus/introduction)*
* **PDF(2022-10-15)**: [Datasheet]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus/datasheet)*
* **PDF(2022-10-15)**: [Finding IMEI and CCID]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus/imei-ccid)*
* **PDF(2022-10-15)**: [Board files]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus/board-files)*
  * nRF Connect SDK 2.1.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.1.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.1.x-v1.1.0.zip)*
  * nRF Connect SDK 2.0.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.0.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.0.x-v1.1.0.zip)*
  * nRF Connect SDK 1.9.x: **ZIP(2022-10-15)**: [BFUP-v1.0.0-nrf-1.9.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v1.9.x-v1.0.0.zip)*
  * nRF Connect SDK 1.8.x: **ZIP(2022-10-15)**: [BFUP-v1.0.0-nrf-1.8.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v1.8.x-v1.0.0.zip)*
  * nRF Connect SDK 1.7.x: **ZIP(2022-10-15)**: [BFUP-v1.0.0-nrf-1.7.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v1.7.x-v1.0.0.zip)*
  * nRF Connect SDK 1.6.x: **ZIP(2022-10-15)**: [BFUP-v1.0.0-nrf-1.6.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v1.6.x-v1.0.0.zip)*
  * nRF Connect SDK 1.5.x: **ZIP(2022-10-15)**: [BFUP-v1.0.0-nrf-1.5.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v1.5.x-v1.0.0.zip)*

[Introduction]: electronic/boards/actinius-icarus-iot/introduction.pdf "2022-10-15: Last updated on: April 18, 2022"
[Datasheet]: electronic/boards/actinius-icarus-iot/datasheet.pdf "2022-10-15: Last updated on: August 15, 2022"
[Finding IMEI and CCID]: electronic/boards/actinius-icarus-iot/imei-ccid.pdf "2022-10-15: Last updated on: March 29, 2022"
[Board files]: electronic/boards/actinius-icarus-iot/board-files.pdf "2022-10-15: Last updated on: October 05, 2022"
[BFUP-v1.1.0-nrf-2.1.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.1.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.1.x"
[BFUP-v1.1.0-nrf-2.0.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.0.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.0.x"
[BFUP-v1.0.0-nrf-1.9.x]: electronic/companies/actinius/BFUP-v1.0.0-nrf-1.9.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.0.0 for nRF Connect SDK (NCS) 1.9.x"
[BFUP-v1.0.0-nrf-1.8.x]: electronic/companies/actinius/BFUP-v1.0.0-nrf-1.8.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.0.0 for nRF Connect SDK (NCS) 1.8.x"
[BFUP-v1.0.0-nrf-1.7.x]: electronic/companies/actinius/BFUP-v1.0.0-nrf-1.7.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.0.0 for nRF Connect SDK (NCS) 1.7.x"
[BFUP-v1.0.0-nrf-1.6.x]: electronic/companies/actinius/BFUP-v1.0.0-nrf-1.6.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.0.0 for nRF Connect SDK (NCS) 1.6.x"
[BFUP-v1.0.0-nrf-1.5.x]: electronic/companies/actinius/BFUP-v1.0.0-nrf-1.5.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.0.0 for nRF Connect SDK (NCS) 1.5.x"

| Board Pinout |
|::|
| <div style="background-color:white;"><div style="width:100%;display:inline-block">[![board-pinout]][board-pinout]</div></div> |

[board-pinout]: electronic/boards/actinius-icarus-iot/board-pinout.png "Icarus IoT Board (nRF9160 Feather) Pinout"

## Getting Started

* **PDF(2022-10-15)**: [Actinius Programmer]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/actinius-programmer)*
* **PDF(2022-10-15)**: [Toolchain installation]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/toolchain-installation)*
* **PDF(2022-10-15)**: [Configuring an application for the Icarus]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/configure-an-application)*
* **PDF(2022-10-15)**: [Building an application for the Icarus]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/building-an-application)*
* **PDF(2022-10-15)**: [Flashing an application onto the Icarus]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/flashing-an-application)*
* **PDF(2022-10-15)**: [Updating the nRF9160 modem firmware]
  – *[HTML(2022-10-15)](https://docs.actinius.com/getting-started/updating-the-modem-firmware)*

[Actinius Programmer]: electronic/companies/actinius/actinius-programmer.pdf "2022-10-15: Last updated on: March 28, 2022"
[Toolchain installation]: electronic/companies/actinius/toolchain-installation.pdf "2022-10-15: Last updated on: March 28, 2022"
[Configuring an application for the Icarus]: electronic/companies/actinius/configure-an-application.pdf "2022-10-15: Last updated on: March 22, 2022"
[Building an application for the Icarus]: electronic/companies/actinius/building-an-application.pdf "2022-10-15: Last updated on: March 22, 2022"
[Flashing an application onto the Icarus]: electronic/companies/actinius/flashing-an-application.pdf "2022-10-15: Last updated on: August 16, 2022"
[Updating the nRF9160 modem firmware]: electronic/companies/actinius/updating-the-modem-firmware.pdf "2022-10-15: Last updated on: September 27, 2022"
