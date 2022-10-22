# Icarus SoM (nRF9160)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-15</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/actinius-icarus-som/board-iso.png "Icarus SoM (nRF9160)"

The **Icarus SoM** (System on Module) is a ready solution that provides cutting
edge low-power cellular IoT connectivity in module form. It is meant to be
integrated into other electronics designs and can be powered using a 3.3 V
regulator or directly through a LiPo battery. The module includes global
LTE-M & NB-IoT connectivity, GPS, Accelerometer, and a SIM switching circuit
that allows the user to choose between the onboard eSIM or an externally
connected SIM. All of this in a 18.5 x 28.0 mm package with castellated pins.

* [nRF9160 SiP]: ARM Cortex-M33F (ARMv8-M) CPU, 1 MB Flash, 256 kB RAM, LTE-M/NB-IoT, GNSS
* [LIS2DH12]: 3-axis low-power accelerometer
* eSIM with SIM switch to external SIM
* uFL connectors for LTE and GPS antenna
* [Zephyr OS Support]

[nRF9160 SiP]: https://www.nordicsemi.com/Products/nRF9160 "ARM® Cortex M33 with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated LTE-M/NB-IoT modem and GNSS"
[LIS2DH12]: https://www.st.com/en/mems-and-sensors/lis2dh12.html "MEMS digital output 3-axis motion sensor"
[Zephyr OS Support]: https://bridle.tiac-systems.net/doc/latest/zephyr/boards/arm/actinius_icarus_som/doc/index.html "Zephyr OS Support for Actinius Icarus SoM"

## References

* *HTML(2022-10-15)*: [Product Page] – *€48,00 (excl. VAT)*
* *HTML(2022-10-15)*: [Symbol and Footprint by SnapEDA]
  – *license protected, uploading to another website forbidden*

[Product Page]: https://www.actinius.com/icarus-som "Icarus SoM (nRF9160)"
[Symbol and Footprint by SnapEDA]: https://www.snapeda.com/parts/Icarus%20SOM/Actinius/view-part "Created by SnapEDA and added to SnapEDA on Nov 16, 2020"

| Symbol | Footprint SOM (top-down) |
|::|::|::|
| <div style="background-color:white;">[![pcb-assembly-symbol]][pcb-assembly-symbol]</div> | <div style="background-color:black;">[![pcb-assembly-footprint-som]][pcb-assembly-footprint-som]</div> |
| | <div style="background-color:white;"><div style="width:75%;display:inline-block;">[![pcb-assembly-top]][pcb-assembly-top]</div></div> |

[pcb-assembly-symbol]: electronic/boards/actinius-icarus-som/pcb-assembly-symbol.png "Icarus SoM (nRF9160) Symbol"
[pcb-assembly-footprint-som]: electronic/boards/actinius-icarus-som/pcb-assembly-footprint-som.png "Icarus SoM (nRF9160) Footprint"
[pcb-assembly-top]: electronic/boards/actinius-icarus-som/pcb-assembly-top.png "Icarus SoM (nRF9160) PCB Assembly (top)"

## Documentation

| Block Diagram |
|::|
| <div style="background-color:white;">[![board-blockdiag]][board-blockdiag]</div> |

[board-blockdiag]: electronic/boards/actinius-icarus-som/board-blockdiag.png "Icarus SoM (nRF9160) Block Diagram"

* **PDF(2022-10-15)**: [Introduction]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som/introduction)*
* **PDF(2022-10-15)**: [Datasheet]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som/datasheet)*
* **PDF(2022-10-15)**: [Board files]
  – *[HTML(2022-10-15)](https://docs.actinius.com/icarus-som/board-files)*
  * nRF Connect SDK 2.1.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.1.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.1.x-v1.1.0.zip)*
  * nRF Connect SDK 2.0.x: **ZIP(2022-10-15)**: [BFUP-v1.1.0-nrf-2.0.x]
    – *[original(2022-10-15)](https://cdn.actini.us/zephyr/nRF%20Connect%20SDK%20v2.0.x-v1.1.0.zip)*

[Introduction]: electronic/boards/actinius-icarus-som/introduction.pdf "2022-10-15: Last updated on: April 18, 2022"
[Datasheet]: electronic/boards/actinius-icarus-som/datasheet.pdf "2022-10-15: Last updated on: August 15, 2022"
[Board files]: electronic/boards/actinius-icarus-som/board-files.pdf "2022-10-15: Last updated on: October 05, 2022"
[BFUP-v1.1.0-nrf-2.1.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.1.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.1.x"
[BFUP-v1.1.0-nrf-2.0.x]: electronic/companies/actinius/BFUP-v1.1.0-nrf-2.0.x.zip "2022-10-15: Board Files Update Pack (BFUP) 1.1.0 for nRF Connect SDK (NCS) 2.0.x"

| SoM Pinout | SoM Reference Design |
|::|::|
| <div style="width:50%;display:inline-block">[![board-pinout]][board-pinout]</div> | [![board-refdesign]][board-refdesign] |

[board-pinout]: electronic/boards/actinius-icarus-som/board-pinout.png "Icarus SoM (nRF9160) Pinout"
[board-refdesign]: electronic/boards/actinius-icarus-som/board-refdesign.png "Icarus SoM (nRF9160) Reference Design"

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
