# Seeed Studio XIAO nRF52840 (Sense)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-22</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso] [![board-iso-sense]][board-iso-sense]</span>

[board-iso]: electronic/boards/seeed-studio-xiao-nrf52840/board-iso.png "Seeed Studio XIAO nRF52840"
[board-iso-sense]: electronic/boards/seeed-studio-xiao-nrf52840/board-iso-sense.png "Seeed Studio XIAO nRF52840 Sense"

The **Seeed Studio XIAO nRF52840** and **Seeed Studio XIAO nRF52840 Sense** is
as small as the [Seeed Studio XIAO SAMD21] but equipped with Bluetooth (LE) 5.3,
IEEE 802.15.4 radio stack (Thread, Zigbee, and ANT), and NFC. It carries the
Nordic [nRF52840] near field radio processor that can flexible clock running
up to 64 MHz which is a low-power (5 μA in deep sleep mode) with 256 kB of
internal SRAM, 1 MB of internal Flash memory, 2 MB of on-board Flash memory,
and provides multiple development interfaces: 11 digital pins, 6 analog pins,
11 PWM Pins, 1 I2C interface, 1 UART interface, 1 SPI interface, 1 NFC
interface, 1 SWD Bonding pad interface. The embedded [BQ25101] chip supports
battery charge management. There are one reset button, you can short connect
them to reset the board. All of this is designed in a tiny size with in a
20 x 17.5 mm package with castellated pins.

The **Seeed Studio XIAO nRF52840 Sense** is equipped with a high-precision
6-Axis Inertial Measurement Unit (IMU) which includes a 3-axis accelerometer
and a 3-axis gyroscope and also with a PDM (Pulse Density Modulation) Microphone
which can receive audio data in real-time and can be used for audio recognition.

* [nRF52840]: ARM Cortex-M4F (ARMv7E-M) CPU, 1 MB Flash, 256 kB RAM, Bluetooth (LE) 5.3, IEEE 802.15.4 (Thread, Zigbee, and ANT), and NFC
* [P25Q16H]: 16 Mbit SPI NOR Flash
* [BQ25101]: LiPo Charger
* [LSM6DS3TR-C]: 6DoF inertial measurement unit (IMU) – *only sense version*
* [MSM261D3526H1CPM]: PDM digital microphone – *only sense version*
* Reset button and power/charger LED and 3-color user LED
* [Zephyr OS Support]

[nRF52840]: https://www.nordicsemi.com/Products/nRF52840 "ARM® Cortex M4F with 1 MB Flash and 256 kB RAM, ARM® Trustzone®, ARM® Cryptocell 310, integrated BT-LE 5.3, IEEE 802.15.4 radio and NFC-A tag"
[P25Q16H]: https://www.puyasemi.com/cpzx/info_131_aid_198_kid_195.html#a002 "16 Mbit SPI NOR Flash"
[BQ25101]: https://www.ti.com/product/BQ25101 "250mA Standalone Linear Li-Ion Battery Charger with Thermal Regulation"
[LSM6DS3TR-C]: https://www.st.com/en/mems-and-sensors/lsm6ds3tr-c.html "iNEMO 3D digital accelerometer and a 3D digital gyroscope"
[MSM261D3526H1CPM]: index.php?dir=electronic/components/memsensing-microsystems/MSM261D3526H1CPM "PDM digital output MEMS microphone with Multi‐modes"
[Zephyr OS Support]: https://bridle.tiac-systems.net/doc/latest/zephyr/boards/arm/xiao_ble/doc/index.html "Zephyr OS Support for Seeed Studio XIAO nRF52840 (Sense)"

[Seeed Studio XIAO SAMD21]: index.php?dir=electronic/boards/seeed-studio-xiao-samd21 "Seeed Studio XIAO SAMD21 – Seeeduino XIAO"

## References

**EAN**: #############<br/>
**UPC**:  ############<br/>
**SKU**: 102010448 / 102010469 *(sense version)*

**HSCODE**:   [8543.70.90.99]<br/>
**EUHSCODE**: [8543.70.90.99]<br/>
**USHSCODE**: [8471.49.00.00]<br/>
**COO**: CHINA

[8543.70.90.99]: https://www.tariffnumber.com/2022/85437090 "HS Code 85437090 – Electrical, machines, apparatus – Other"
[8471.49.00.00]: https://www.tariffnumber.com/2022/84714900 "HS Code 84714900 - Data, processing, machines – Other, presented in the form of systems"

*Brand*: Seeed<br/>
*Part number*: 102010448 / 102010469 *(sense version)*

* *HTML(2022-10-22)*: [Product Page] – *$9,90 (excl. VAT)*
* *HTML(2022-10-22)*: [Product Page (Sense)] – *$15,99 (excl. VAT)*
* *HTML(2022-10-22)*: [Seeed Studio XIAO Series]
  – *Compact and powerful microcontroller*
* *HTML(2022-10-22)*: [Overview of the Seeed Studio XIAO]
  – *Overview of the based Seeed Studio XIAO*

[Product Page]: https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html "Seeed Studio XIAO nRF52840"
[Product Page (Sense)]: https://www.seeedstudio.com/Seeed-XIAO-BLE-Sense-nRF52840-p-5253.html "Seeed Studio XIAO nRF52840 Sense"
[Seeed Studio XIAO Series]: https://www.seeedstudio.com/xiao-series-page "XIAO: thumb-sized tiny, but powerful"
[Overview of the Seeed Studio XIAO]: https://sigmdel.ca/michel/ha/xiao/seeeduino_xiao_01_en.html "Based Seeed Studio XIAO Overview"

| PCB Layer | PCB 3D or Footprint | PCB Populated (top & bottom) |
|::|::|::|
| <div style="background-color:white;"><div style="width:65%;display:inline-block"><mark><strong>Eagle or Altium <em>PCB Layer</em> output is missing!</strong></mark></div></div> |<div style="background-color:white;"><div style="width:65%;display:inline-block"><mark><strong>Eagle or Altium <em>PCB 3D / Footprint</em> output is missing!</strong></mark></div></div> | <div style="background-color:white;"><div style="width:33%;display:inline-block">[![pcb-assembly-top]][pcb-assembly-top]</div></div> |
| | | <div style="background-color:white;"><div style="width:33%;display:inline-block">[![pcb-assembly-bot]][pcb-assembly-bot]</div></div> |
| | | <div style="background-color:white;"><div style="width:33%;display:inline-block">[![pcb-assembly-top-sense]][pcb-assembly-top-sense]</div></div> |
| | | <div style="background-color:white;"><div style="width:33%;display:inline-block">[![pcb-assembly-bot-sense]][pcb-assembly-bot-sense]</div></div> |

[pcb-assembly-top]: electronic/boards/seeed-studio-xiao-nrf52840/pcb-assembly-top.png "Seeed Studio XIAO nRF52840 PCB Assembly (top)"
[pcb-assembly-bot]: electronic/boards/seeed-studio-xiao-nrf52840/pcb-assembly-bot.png "Seeed Studio XIAO nRF52840 PCB Assembly (bottom)"
[pcb-assembly-top-sense]: electronic/boards/seeed-studio-xiao-nrf52840/pcb-assembly-top-sense.png "Seeed Studio XIAO nRF52840 (Sense) PCB Assembly (top)"
[pcb-assembly-bot-sense]: electronic/boards/seeed-studio-xiao-nrf52840/pcb-assembly-bot-sense.png "Seeed Studio XIAO nRF52840 (Sense) PCB Assembly (bottom)"

## Documentation

* **PDF(2022-10-22)**: [XIAO BLE Sense Getting Started]
  – *[HTML(2022-10-22)](https://wiki.seeedstudio.com/XIAO-BLE-Sense-Getting-Started)*
* **PDF(2022-10-22)**: [Getting Started with Seeed Studio XIAO nRF52840 (Sense)]
  – *[HTML(2022-10-22)](https://wiki.seeedstudio.com/XIAO_BLE)*
* **PDF(2022-10-22)**: [Seeed Studio XIAO nRF52840 (Sense) with CircuitPython]
  – *[HTML(2022-10-22)](https://wiki.seeedstudio.com/XIAO-BLE_CircutPython)*

[XIAO BLE Sense Getting Started]: electronic/boards/seeed-studio-xiao-nrf52840/getting-started-xiao-ble.pdf "2022-10-22: Last updated on: MONTH DAY, YEAR"
[Getting Started with Seeed Studio XIAO nRF52840 (Sense)]: electronic/boards/seeed-studio-xiao-nrf52840/getting-started.pdf "2022-10-22: Last updated on: MONTH DAY, YEAR"
[Seeed Studio XIAO nRF52840 (Sense) with CircuitPython]: electronic/boards/seeed-studio-xiao-nrf52840/circuitpython.pdf "2022-10-22: Last updated on: MONTH DAY, YEAR"

| Pinout |
|::|
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-pinout]][board-pinout]</div></div> |
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-interfaces-top]][board-interfaces-top]</div></div> |
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-interfaces-bot]][board-interfaces-bot]</div></div> |

[board-pinout]: electronic/boards/seeed-studio-xiao-nrf52840/board-pinout.png "Seeed Studio XIAO nRF52840 (Sense) Pinout"
[board-interfaces-top]: electronic/boards/seeed-studio-xiao-nrf52840/board-interfaces-top.png "Seeed Studio XIAO nRF52840 (Sense) Interfaces (top)"
[board-interfaces-bot]: electronic/boards/seeed-studio-xiao-nrf52840/board-interfaces-bot.png "Seeed Studio XIAO nRF52840 (Sense) Interfaces (bottom)"

* **PDF(2022-10-22)**: [Eagle Schematic v1.0 (211027)]
  – *[ZIP(2022-10-22)](https://files.seeedstudio.com/wiki/XIAO-BLE/Seeed-XIAO-nRF52840-v1.0-SCH.zip)*
* **PDF(2022-10-22)**: [Bottom pad positioning dimensioning v1.0 (211122)]
  – *[ZIP(2022-10-22)](https://files.seeedstudio.com/wiki/XIAO-BLE/Bottom-pad-positioning.zip)*
* **PDF(2022-10-22)**: [Bottom pad positioning silkscreen v1.0 (211122)]
  – *[ZIP(2022-10-22)](https://files.seeedstudio.com/wiki/XIAO-BLE/Bottom-pad-positioning.zip)*

[Eagle Schematic v1.0 (211027)]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-schematic.pdf "2022-10-22: Last updated on: October 27, 2021"
[Bottom pad positioning dimensioning v1.0 (211122)]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-dimensioning.pdf "2022-10-22: Last updated on: November 22, 2021"
[Bottom pad positioning silkscreen v1.0 (211122)]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-silkscreen.pdf "2022-10-22: Last updated on: November 22, 2021"

| Revision | Design Data | PCB Layout | Changelog |
|::|:-|::|:-|
| **v1.0** – *(January 2021)* | <mark><strong>Eagle BRD file is missing!</strong></mark><br/>[eagle-design-v1.0-211027]:<br/>- [SCH-1-0]<br/>- BRD-1-0<br/>- [DXF-1-0]<br/>- [DWG-1-0] | <mark><strong>Eagle BRD file is missing!</strong></mark> <div style="background-color:white;"><div style="width:75%;display:inline-block">[![eagle-board-dimensioning-v1.0-211027]][eagle-board-dimensioning-v1.0-211027]</div></div> <div style="background-color:black;"><div style="width:40%;display:inline-block">[![eagle-board-silkscreen-v1.0-211027]][eagle-board-silkscreen-v1.0-211027]</div></div> | Initail Version |

[eagle-design-v1.0-211027]: index.php?dir=electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027 "Eagle Design Data"
[SCH-1-0]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840.sch "Eagle v6.4 Schematic"
[DXF-1-0]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-dimensioning.dxf "AutoCAD Drawing Exchange Format, version 2004"
[DWG-1-0]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-dimensioning.dwg "DWG AutoDesk AutoCAD Release 13"
[eagle-board-dimensioning-v1.0-211027]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-dimensioning.svg "2022-10-22: Last updated on: November 22, 2021"
[eagle-board-silkscreen-v1.0-211027]: electronic/boards/seeed-studio-xiao-nrf52840/eagle-design-v1.0-211027/xiao-nrf52840-silkscreen.svg "2022-10-22: Last updated on: November 22, 2021"
