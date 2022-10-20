# Icarus SoM DK (nRF9160)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark>$Format:%h$</mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-15</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/actinius-icarus-som-dk/board-iso.png "Icarus SoM DK (nRF9160)"

The **Icarus SoM DK** (System on Module Development Kit) is a single board
development kit for evaluation and development on the [Icarus SoM (nRF9160)]
that includes global LTE-M & NB-IoT connectivity, GPS, Accelerometer and an
eSIM. The development kit provides interfacing to the SoM through USB-C, a set
of user LEDs, a reset and user button, a battery charging port, and a external
nano SIM connector. The board is also Arduino Uno Rev3 compatible which makes
using external shields possible.

* [Icarus SoM (nRF9160)]: Nordic nRF9160 based SoM for the Icarus family by [Actinius]
* [nRF9160 SiP]: ARM Cortex-M33F (ARMv8-M) CPU, 1 MB Flash, 256 kB RAM, LTE-M/NB-IoT, GNSS
* [LIS2DH12]: 3-axis low-power accelerometer
* [W25Q64JV]: 64 Mbit SPI NOR Flash (on board)
* [WS2812]: NeoPixel addressable RGB LED
* Reset and user button and blue LED (on board)
* eSIM (on SoM) and external SIM (on board)
* FTDI USB to serial converter

[nRF9160 SiP]: https://www.nordicsemi.com/Products/nRF9160 "ARM® Cortex M33 with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated LTE-M/NB-IoT modem and GNSS"
[LIS2DH12]: https://www.st.com/en/mems-and-sensors/lis2dh12.html "MEMS digital output 3-axis motion sensor"
[Icarus SoM (nRF9160)]: index.php?dir=electronic/boards/actinius-icarus-som "Icarus SoM (nRF9160)"
[W25Q64JV]: https://www.winbond.com/hq/product/code-storage-flash-memory/serial-nor-flash/?__locale=en&partNo=W25Q64JV "64 Mbit SPI NOR Flash"
[WS2812]: http://www.world-semi.com/Certifications/WS2812B.html "4-pin digital RGB LED"
[Actinius]: index.php?dir=electronic/companies/actinius

## References

* *HTML(2022-10-15)*: [Product Page] – *€119,49 (excl. VAT)*

[Product Page]: https://www.actinius.com/icarus-som-dk "Icarus SoM DK (nRF9160)"

## Documentation

| Block Diagram |
|::|
| <div style="background-color:white;">[![board-blockdiag]][board-blockdiag]</div> |

[board-blockdiag]: electronic/boards/actinius-icarus-som-dk/board-blockdiag.png "Icarus SoM DK (nRF9160) Block Diagram"

* **PDF(2022-10-15)**: [Introduction]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som-dk/introduction)*
* **PDF(2022-10-15)**: [Datasheet]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som-dk/datasheet)*
* **PDF(2022-10-15)**: [Board files]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som-dk/board-files)*

[Introduction]: electronic/boards/actinius-icarus-som-dk/introduction.pdf "2022-10-15: Last updated on: April 18, 2022"
[Datasheet]: electronic/boards/actinius-icarus-som-dk/datasheet.pdf "2022-10-15: Last updated on: August 15, 2022"
[Board files]: electronic/boards/actinius-icarus-som-dk/board-files.pdf "2022-10-15: Last updated on: April 21, 2022"

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
