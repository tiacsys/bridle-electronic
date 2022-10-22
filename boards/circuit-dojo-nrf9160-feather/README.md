# nRF9160 Feather

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-20</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/circuit-dojo-nrf9160-feather/board-iso.png "nRF9160 Feather"

The **nRF9160 Feather** is a fully featured LTE Cat-M1 and GPS enabled cellular
IoT board in Adafruit's Feather(Wing) form factor. It is built around Nordic
Semi's nRF9160 (GEN2) modem and combines LTE-M & NB-IoT connectivity, GPS,
Accelerometer, SPI Flash, RTC, USB, LiPo charger as well as a nano SIM
connector. All of this in a 22.8 x 50.8 mm package with castellated pins.

* [nRF9160 SiP]: ARM Cortex-M33F (ARMv8-M) CPU, 1 MB Flash, 256 kB RAM, LTE-M/NB-IoT, GNSS
* [LIS2DH12]: 3-axis low-power accelerometer
* [W25Q32JV] or [W25Q16JV]: 32 or 16 Mbit SPI NOR Flash
* [PCF85063ATL]: low-power real-time-clock/calendar with alarm
* Reset and user button and blue LED
* on-board 4FF nano SIM connector
* uFL connectors for LTE and GPS antenna
* [MCP73830T] or [STBC08PMR]: LiPo Charger
* Battery voltage measurement circuit
* SiLabs USB to serial converter
* [Zephyr OS Support]

[nRF9160 SiP]: https://www.nordicsemi.com/Products/nRF9160 "ARM® Cortex M33 with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated LTE-M/NB-IoT modem and GNSS"
[LIS2DH12]: https://www.st.com/en/mems-and-sensors/lis2dh12.html "MEMS digital output 3-axis motion sensor"
[W25Q32JV]: https://www.winbond.com/hq/product/code-storage-flash-memory/serial-nor-flash/?__locale=en&partNo=W25Q32JV "32 Mbit SPI NOR Flash"
[W25Q16JV]: https://www.winbond.com/hq/product/code-storage-flash-memory/serial-nor-flash/?__locale=en&partNo=W25Q16JV "16 Mbit SPI NOR Flash"
[PCF85063ATL]: https://www.nxp.com/part/PCF85063ATL "Tiny Real-Time Clock/calendar with alarm function and I2C-bus"
[MCP73830T]: https://www.microchip.com/en-us/product/MCP73830 "Single Cell Lithium-Ion Charge Management Controller w/ Soft Start"
[STBC08PMR]: https://www.st.com/en/power-management/stbc08.html "800mA Standalone Linear Li-Ion Battery Charger with Thermal Regulation"
[Zephyr OS Support]: https://bridle.tiac-systems.net/doc/latest/zephyr/boards/arm/circuitdojo_feather_nrf9160/doc/index.html "Zephyr OS Support for Circuit Dojo nRF9160 Feather"

## References

* *HTML(2022-10-20)*: [Product Page] – *$99,00 (excl. VAT)*
* *GitHub(2022-10-20)*: [Product Documentation]
  – *Markdown files for the nRF9160 Feather and the Air Quality Wing*
* *GitHub(2022-10-20)*: [Eagle Hardware Design]
  – *Hardware files for the nRF9160 Feather*

[Product Page]: https://www.jaredwolff.com/store/nrf9160-feather "nRF9160 Feather"
[Product Documentation]: https://github.com/circuitdojo/docs "nRF9160 Feather and Air Quality Wing"
[Eagle Hardware Design]: https://github.com/circuitdojo/nrf9160-feather "nRF9160 Feather"

| Symbol | Features (top-down) | Features (bottom-up) |
|::|::|::|
| <div style="background-color:white;">[![pcb-assembly-3d]][pcb-assembly-3d]</div> | <div style="background-color:white;">[![pcb-assembly-features-top]][pcb-assembly-features-top]</div> | <div style="background-color:white;">[![pcb-assembly-features-bot]][pcb-assembly-features-bot]</div> |
| | <div style="background-color:white;"><div style="width:75%;display:inline-block;">[![pcb-assembly-top]][pcb-assembly-top]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block;">[![pcb-assembly-bot]][pcb-assembly-bot]</div></div> |

[pcb-assembly-3d]: electronic/boards/circuit-dojo-nrf9160-feather/pcb-assembly-3d.png "nRF9160 Feather 3D"
[pcb-assembly-features-top]: electronic/boards/circuit-dojo-nrf9160-feather/pcb-assembly-features-top.png "nRF9160 Feather Features (top)"
[pcb-assembly-features-bot]: electronic/boards/circuit-dojo-nrf9160-feather/pcb-assembly-features-bot.png "nRF9160 Feather Features (bottom)"
[pcb-assembly-top]: electronic/boards/circuit-dojo-nrf9160-feather/pcb-assembly-top.png "nRF9160 Feather PCB Assembly (top)"
[pcb-assembly-bot]: electronic/boards/circuit-dojo-nrf9160-feather/pcb-assembly-bot.png "nRF9160 Feather PCB Assembly (bottom)"

## Documentation

| Block Diagram |
|::|
| <div style="background-color:white;">[![board-blockdiag]][board-blockdiag]</div> |

[board-blockdiag]: electronic/boards/circuit-dojo-nrf9160-feather/board-blockdiag.png "nRF9160 Feather Block Diagram"

* **PDF(2022-10-20)**: [Product Documentation]
  – *[HTML(2022-10-20)](https://docs.jaredwolff.com/)*
* **PDF(2022-10-20)**: [Specification]
  – *[HTML(2022-10-20)](https://docs.jaredwolff.com/nrf9160-specs.html)*
* **PDF(2022-10-20)**: [Compliance]
  – *[HTML(2022-10-20)](https://docs.jaredwolff.com/nrf9160-compliance.html)*
* **PDF(2022-10-20)**: [Changelog]
  – *[HTML(2022-10-20)](https://docs.jaredwolff.com/nrf9160-changelog.html)*
* **PDF(2022-10-20)**: [Downloads]
  – *[HTML(2022-10-20)](https://docs.jaredwolff.com/nrf9160-downloads.html)*
  * nRF Connect SDK 1.3.x: **ZIP(2022-10-20)**: [board-definitions-ncs-v1.3.x]
    – *[original(2022-10-20)](https://docs.jaredwolff.com/files/board-definitions-ncs-v1.3.x.zip)*
  * nRF Connect SDK 1.2.x: **ZIP(2022-10-20)**: [board-definitions-ncs-v1.2.x]
    – *[original(2022-10-20)](https://docs.jaredwolff.com/files/board-definitions-ncs-v1.2.x.zip)*
  * **ZIP(2022-10-20)**: [bootloader-v2]
    – *[original(2022-10-20)](https://docs.jaredwolff.com/files/v2-010421-1502-merged.hex.zip)*
  * **ZIP(2022-10-20)**: [bootloader-v1]
    – *[original(2022-10-20)](https://docs.jaredwolff.com/files/nrf9160_feather_bootloader_v1.zip)*
  * **ZIP(2022-10-20)**: [samples-v1.7.x]
    – *[original(2022-10-20)](https://docs.jaredwolff.com/files/nfed_v1.7.x_e946e5c.zip)*

[Product Documentation]: electronic/boards/circuit-dojo-nrf9160-feather/product-documentation.pdf "2022-10-20: Last updated on: December 08, 2021"
[Specification]: electronic/boards/circuit-dojo-nrf9160-feather/specification.pdf "2022-10-20: Last updated on: December 07, 2020"
[Compliance]: electronic/boards/circuit-dojo-nrf9160-feather/compliance.pdf "2022-10-20: Last updated on: October 13, 2020"
[Changelog]: electronic/boards/circuit-dojo-nrf9160-feather/changelog.pdf "2022-10-20: Last updated on: December 08, 2021"
[Downloads]: electronic/boards/circuit-dojo-nrf9160-feather/downloads.pdf "2022-10-20: Last updated on: December 08, 2021"
[board-definitions-ncs-v1.3.x]: electronic/companies/circuit-dojo-nrf9160-feather/board-definitions-ncs-v1.3.x.zip "2022-10-20: Board Defintions for nRF Connect SDK (NCS) 1.3.x"
[board-definitions-ncs-v1.2.x]: electronic/companies/circuit-dojo-nrf9160-feather/board-definitions-ncs-v1.2.x.zip "2022-10-20: Board Defintions for nRF Connect SDK (NCS) 1.2.x"
[bootloader-v2]: electronic/companies/circuit-dojo-nrf9160-feather/bootloader-v2.zip "2022-10-20: Bootloader v2"
[bootloader-v1]: electronic/companies/circuit-dojo-nrf9160-feather/bootloader-v1.zip "2022-10-20: Bootloader v1"
[samples-v1.7.x]: electronic/companies/circuit-dojo-nrf9160-feather/samples-v1.7.x.zip "2022-10-20: Pre-compiled Samples"

| Revision | Eagle Design Data | PCB Layout | Changelog |
|::|:-|::|:-|
| **v4** – *(October 2021)* | [v4-20220414]:<br/>- [SCH-0015-04]<br/>- [BRD-0015-04]<br/>- [STEP-7-9] | <div style="background-color:black;"><div style="width:100%;display:inline-block">[![board-v4-20220414]][board-v4-20220414]</div></div> | USB-C, LM3281 with PWM/PFM, MCP73830T,<br/>INT1 optional, INT2 on LIS2DH12 |
| **v2** – *(January 2021)* | [v2-20210113]:<br/>- [SCH-0015-02]<br/>- [BRD-0015-02]<br/>- [STEP-5-6] | <div style="background-color:black;"><div style="width:100%;display:inline-block">[![board-v2-20210113]][board-v2-20210113]</div></div> | LIS2DH12 with INT1 and JMP1,<br/>PS_EN now accessible with JMP2,<br/>bottom side labels update |
| **v1** – *(July 2020)* | [v1-20200717]:<br/>- [SCH-0015-01]<br/>- [BRD-0015-01]<br/>- [STEP-3-9] | <div style="background-color:black;"><div style="width:100%;display:inline-block">[![board-v1-20200717]][board-v1-20200717]</div></div> | initial version |

[v4-20220414]: index.php?dir=electronic/boards/circuit-dojo-nrf9160-feather/v4-20220414 "Eagle Design Data"
[SCH-0015-04]: electronic/boards/circuit-dojo-nrf9160-feather/v4-20220414/nrf91-feather.sch "Eagle v9.6.2 Schematic"
[BRD-0015-04]: electronic/boards/circuit-dojo-nrf9160-feather/v4-20220414/nrf91-feather.brd "Eagle v9.6.2 Board"
[STEP-7-9]: electronic/boards/circuit-dojo-nrf9160-feather/v4-20220414/nrf91-feather-v79.step "Autodesk Translation Framework v11.7.0.108 STEP 3D"
[board-v4-20220414]: electronic/boards/circuit-dojo-nrf9160-feather/v4-20220414/nrf91-feather-pcb.svg "nRF9160 Feather v4 (October 2021)"

[v2-20210113]: index.php?dir=electronic/boards/circuit-dojo-nrf9160-feather/v2-20210113 "Eagle Design Data"
[SCH-0015-02]: electronic/boards/circuit-dojo-nrf9160-feather/v2-20210113/nrf91-feather.sch "Eagle v9.5.1 Schematic"
[BRD-0015-02]: electronic/boards/circuit-dojo-nrf9160-feather/v2-20210113/nrf91-feather.brd "Eagle v9.5.1 Board"
[STEP-5-6]: electronic/boards/circuit-dojo-nrf9160-feather/v2-20210113/nrf91-feather-v56.step "Autodesk Translation Framework v9.7.0.1280 STEP 3D"
[board-v2-20210113]: electronic/boards/circuit-dojo-nrf9160-feather/v2-20210113/nrf91-feather-pcb.svg "nRF9160 Feather v2 (January 2021)"

[v1-20200717]: index.php?dir=electronic/boards/circuit-dojo-nrf9160-feather/v1-20200717 "Eagle Design Data"
[SCH-0015-01]: electronic/boards/circuit-dojo-nrf9160-feather/v1-20200717/nrf91-feather.sch "Eagle v9.5.1 Schematic"
[BRD-0015-01]: electronic/boards/circuit-dojo-nrf9160-feather/v1-20200717/nrf91-feather.brd "Eagle v9.5.1 Board"
[STEP-3-9]: electronic/boards/circuit-dojo-nrf9160-feather/v1-20200717/nrf91-feather-v39.step "Autodesk Translation Framework v9.7.0.1280 STEP 3D"
[board-v1-20200717]: electronic/boards/circuit-dojo-nrf9160-feather/v1-20200717/nrf91-feather-pcb.svg "nRF9160 Feather v2 (January 2021)"
