# Icarus Bee (nRF9160)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-15</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/actinius-icarus-bee/board-iso.png "Icarus Bee (nRF9160)"

The **Icarus Bee** includes global LTE-M & NB-IoT connectivity, GPS,
Accelerometer, on-board Button and RGB LED, an on-board 64Mbit Flash as well
as an eSIM for connectivity out of the box, all in just 32.5 x 28.0 mm. You
can even connect your own nano SIM thanks to the dual-SIM selection circuit!

* [Icarus SoM (nRF9160)]: Nordic nRF9160 based SoM for the Icarus family by [Actinius]
* [nRF9160 SiP]: ARM Cortex-M33F (ARMv8-M) CPU, 1 MB Flash, 256 kB RAM, LTE-M/NB-IoT, GNSS (on SoM)
* [LIS2DH12]: 3-axis low-power accelerometer (on SoM)
* [W25Q64JV]: 64 Mbit SPI NOR Flash (on board)
* User button and RGB LED (on board)
* eSIM (on SoM) and external SIM (on board)
* [Zephyr OS Support]

[nRF9160 SiP]: https://www.nordicsemi.com/Products/nRF9160 "ARM® Cortex M33 with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated LTE-M/NB-IoT modem and GNSS"
[LIS2DH12]: https://www.st.com/en/mems-and-sensors/lis2dh12.html "MEMS digital output 3-axis motion sensor"
[Icarus SoM (nRF9160)]: index.php?dir=electronic/boards/actinius-icarus-som "Icarus SoM (nRF9160)"
[W25Q64JV]: https://www.winbond.com/hq/product/code-storage-flash-memory/serial-nor-flash/?__locale=en&partNo=W25Q64JV "64 Mbit SPI NOR Flash"
[Zephyr OS Support]: https://bridle.tiac-systems.net/doc/latest/zephyr/boards/arm/actinius_icarus_bee/doc/index.html "Zephyr OS Support for Actinius Icarus Bee"
[Actinius]: index.php?dir=electronic/companies/actinius

## References

* *HTML(2022-10-15)*: [Product Page] – *€65,45 (excl. VAT)*
* *HTML(2022-10-15)*: [Symbol and Footprint by SnapEDA]
  – *license protected, uploading to another website forbidden*

[Product Page]: https://www.actinius.com/icarus-bee "Icarus Bee (nRF9160)"
[Symbol and Footprint by SnapEDA]: https://www.snapeda.com/parts/Icarus%20Bee/Actinius/view-part "Created by Actinius and added to SnapEDA on Jan 27, 2021"

| Symbol | Footprint TH | Footprint SMD |
|::|::|::|
| <div style="background-color:white;">[![pcb-assembly-symbol]][pcb-assembly-symbol]</div> | <div style="background-color:black;">[![pcb-assembly-footprint-th]][pcb-assembly-footprint-th]</div> | <div style="background-color:black;">[![pcb-assembly-footprint-smd]][pcb-assembly-footprint-smd]</div> |
| | <div style="background-color:white;"><div style="width:60%;display:inline-block;">[![pcb-assembly-top]][pcb-assembly-top]</div></div> | <div style="background-color:white;"><div style="width:60%;display:inline-block;">[![pcb-assembly-bot]][pcb-assembly-bot]</div></div> |

[pcb-assembly-symbol]: electronic/boards/actinius-icarus-bee/pcb-assembly-symbol.png "Icarus Bee (nRF9160) Symbol"
[pcb-assembly-footprint-th]: electronic/boards/actinius-icarus-bee/pcb-assembly-footprint-th.png "Icarus Bee (nRF9160) Footprint TH"
[pcb-assembly-footprint-smd]: electronic/boards/actinius-icarus-bee/pcb-assembly-footprint-smd.png "Icarus Bee (nRF9160) Footprint SMD"
[pcb-assembly-top]: electronic/boards/actinius-icarus-bee/pcb-assembly-top.png "Icarus Bee (nRF9160) PCB Assembly (top)"
[pcb-assembly-bot]: electronic/boards/actinius-icarus-bee/pcb-assembly-bot.png "Icarus Bee (nRF9160) PCB Assembly (bottom)"

## Documentation

* **PDF(2022-10-15)**: [Introduction]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-bee/introduction)*
* **PDF(2022-10-15)**: [Datasheet]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-bee/datasheet)*
* **PDF(2022-10-15)**: [Finding IMEI and CCID]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-bee/imei-ccid)*
* **PDF(2022-10-15)**: [Board files]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-bee/board-files)*
  * nRF Connect SDK 2.1.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.1.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.1.x-v1.1.0.zip)*
  * nRF Connect SDK 2.0.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.0.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.0.x-v1.1.0.zip)*

[Introduction]: electronic/boards/actinius-icarus-bee/introduction.pdf "2022-10-15: Last updated on: April 18, 2022"
[Datasheet]: electronic/boards/actinius-icarus-bee/datasheet.pdf "2022-10-15: Last updated on: August 15, 2022"
[Finding IMEI and CCID]: electronic/boards/actinius-icarus-bee/imei-ccid.pdf "2022-10-15: Last updated on: April 18, 2022"
[Board files]: electronic/boards/actinius-icarus-bee/board-files.pdf "2022-10-15: Last updated on: October 05, 2022"
[BFUP-v1.1.0-nrf-2.1.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.1.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.1.x"
[BFUP-v1.1.0-nrf-2.0.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.0.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.0.x"

| Board Pinout |
|::|
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-pinout]][board-pinout]</div></div> |

[board-pinout]: electronic/boards/actinius-icarus-bee/board-pinout.png "Icarus Bee (nRF9160) Pinout"

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
