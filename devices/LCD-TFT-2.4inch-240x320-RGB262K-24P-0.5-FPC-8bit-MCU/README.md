# 2.4" TFT-LCD with 240x3(RGB) x 320, 262K colors, 8-bit MCU

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-28</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![part-iso]][part-iso]</span>

[part-iso]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/RY24049B-00-A/part-iso.png "2.4 TFT-LCD RGB 240x320 8-bit MCU"

These kinds of cheap and simple TFT LCDs are mostly no-name mass-produced goods
from China:

* **Si-TFT-LCD**: amorphous silicon thin film transistor liquid crystal display
* **Panel Size**: 2.4 inch and the resolution is 240x320 dot
* **Color Number**: 262K RGB
* **Color Arrangement**: RGB-stripe
* **Driver IC**: [Sitronix ST7789V] or (not yet listed here) [ILITEK ILI9341(V)]
* **Back Light**: 4/6x white LED
* **Interface**:
  * 8-bit MCU for display data
  * *optional*: I2C for driver IC setup
  * *optional*: XL/R+YU/D resistive touch screen terminal
* **Connector**:
  * 24 pin 0.5mm FPC for 8-bit MCU
  * *optional*: 4 pin FPC for separat touch screen terminal

[Sitronix ST7789V]: index.php?dir=electronic/components/sitronix/ST7789V "240RGBx320 dot 262K Color TFT Controller/Driver"
[ILITEK ILI9341(V)]: index.php?dir=electronic/components/ilitek/ILI9341 "240RGBx320 dot 262K Color TFT Controller/Driver"

| Common Mechanical Drawing as provided by SiPEED |
|::|
| [![part-common-mechdraw]][part-common-mechdraw] |

[part-common-mechdraw]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/sipeed-accessories-2.4-lcd.jpg "2.4 TFT-LCD Common Mechanical Drawing"

| MANUFACTOR / DISTRIBUTOR / TYP / IC | &nbsp;&nbsp;&nbsp;TOP&nbsp;&nbsp;&nbsp; | BOTTOM |
|::|::|::|
| [Seeed Studio](https://www.seeedstudio.com/2-4-TFT-LCD-p-4049.html) <br/> **DS:**[RY24049B0-00-A] <br/> [ST7789V][Sitronix ST7789V] | <div style="background-color:white;">[![RY24049B0-top]][RY24049B0-top]</div> | <div style="background-color:white;">[![RY24049B0-bot]][RY24049B0-bot]</div> |
| [Seeed Studio](https://www.seeedstudio.com/Sipeed-MAix-BiT-for-RISC-V-AI-IoT-1-p-2873.html) <br/> **SPEC:**[JLT24100B] **DS:**[JLT24100B-V1] <br/> [ST7789V][Sitronix ST7789V] <br/> *also seen on product photos*: **1LT24100B-V1** | <div style="background-color:white;">[![JLT24100B-top]][JLT24100B-top]</div> | <div style="background-color:white;">[![JLT24100B-bot]][JLT24100B-bot]</div> |
| [SiPEED](https://dl.sipeed.com/shareURL/Accessories/LCD) <br/> [ZSX024-B2441 V1] <br/> [ST7789V][Sitronix ST7789V] <br/> *also seen on product photos*: **ZSX024-H2441** | <div style="background-color:white;">[![ZSX024-B2441-top]][ZSX024-B2441-top]</div> | <div style="background-color:white;">[![ZSX024-B2441-bot]][ZSX024-B2441-bot]</div> |
|  | <div style="background-color:white;">[![ZSX024-B2441-top-alt-1]][ZSX024-B2441-top-alt-1]</div> | <div style="background-color:white;">[![ZSX024-B2441-bot-alt-1]][ZSX024-B2441-bot-alt-1]</div> |

[RY24049B0-00-A]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/RY24049B-00-A/datasheet-reva-20171107.pdf "RY24049B0-00-A Datasheet Rev. A (2017-11-07)"
[RY24049B0-top]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/RY24049B-00-A/part-top.png "RY24049B0-00-A Top View"
[RY24049B0-bot]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/RY24049B-00-A/part-bot.png "RY24049B0-00-A Bottom View"

[JLT24100B]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/JLT24100B/specification-v0.0-20161123.pdf "JLT24100B Specification V0.0 (2016-11-23)"
[JLT24100B-V1]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/JLT24100B/datasheet-v1.0-20180329.pdf "JLT24100B Datasheet V1.0 (2018-03-29)"
[JLT24100B-top]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/JLT24100B/part-top.jpg "JLT24100B-V1 Top View"
[JLT24100B-bot]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/JLT24100B/part-bot.jpg "JLT24100B-V1 Bottom View"

[ZSX024-B2441 V1]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/ZSX024-B2441/part-params-table.jpg "ZSX024-B2441 V1 Table with parameters"
[ZSX024-B2441-top]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/ZSX024-B2441/part-top.png "ZSX024-B2441 V1 Top View"
[ZSX024-B2441-bot]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/ZSX024-B2441/part-bot.png "ZSX024-B2441 V1 Bottom View"
[ZSX024-B2441-top-alt-1]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/ZSX024-B2441/part-top-alt-1.jpg "ZSX024-B2441 V1 Top View"
[ZSX024-B2441-bot-alt-1]: electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU/ZSX024-B2441/part-bot-alt-1.jpg "ZSX024-B2441 V1 Bottom View"

## Notes and References

* [JLT24100B 8-bit Full Data Set](http://www.51lcm.com/Lcddata/024/JLT24100B/JLT24100B-8BIT.rar):
  demo program, specifications, reference design data

* [SiPEED MaixDuino ST7789V LCD Library](https://maixduino.sipeed.com/en/libs/sipeed_st7789.html)
* [ZSX024-B2441 on Espressif i80 Controller](https://github.com/espressif/esp-idf/issues/9963)
  ```none
  My LCD display is called ZSX024-B2441, a component in SiPEED Maix Dock. The
  display is not broken because it works on that board. The display uses 8-bit
  MCU parallel interface with ST7789V controller.

  Here is my connection:

     ESP Board                      LCD Screen
  ┌─────────────┐              ┌────────────────┐
  │             │              │                │
  │         3V3 ├─────────────►│ VCC            │
  │             │              │                │
  │         GND ├──────────────┤ GND            │
  │             │              │                │
  │      GPIO12 ├─────────────►│ D0             │
  │             │              │                │
  │      GPIO16 ├─────────────►│ D1             │
  │             │              │                │
  │      GPIO17 ├─────────────►│ D2             │
  │             │              │                │
  │      GPIO18 ├─────────────►│ D3             │
  │             │              │                │
  │      GPIO19 ├─────────────►│ D4             │
  │             │              │                │
  │      GPIO21 ├─────────────►│ D5             │
  │             │              │                │
  │       GPIO5 ├─────────────►│ D6             │
  │             │              │                │
  │      GPIO15 ├─────────────►│ D7             │
  │             │              │                │
  │      GPIO32 ├─────────────►│ PCLK           │
  │             │              │                │
  │      GPIO27 ├─────────────►│ CS             │
  │             │              │                │
  │      GPIO33 ├─────────────►│ D/C            │
  │             │              │                │
  │       GPIO0 ├─────────────►│ RST            │
  │             │              │                │
  │         3V3 ├─────5R1─────►│ LEDA           │
  │             │              │                │
  │         GND ├──────────────┤ LEDK           │
  │             │              │                │
  └─────────────┘              └────────────────┘

  This is rather urgent for me, could someone please give me some suggestions or
  a guide to solve the problem? Please note that I'm using one single PCB board
  with an FPC connector to the lcd instead of devkit and wire connections, thus
  it is hard for me to change the pin connections as well as to test signals
  with oscilloscope.
  ```
