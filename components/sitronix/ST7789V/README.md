# ST7789V – 240RGBx320 dot 262K Color TFT Controller/Driver

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-27</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/sitronix/ST7789V/chip-top-bot.svg "Sitronix ST7789V"

The ST7789V is a single-chip controller/driver for 262K-color, graphic type
TFT-LCD. It consists of 720 source line and 320 gate line driving circuits.
This chip is capable of connecting directly to an external microprocessor, and
accepts, 8-bits/9-bits/16-bits/18-bits parallel interface. Display data can be
stored in the on-chip display data RAM of 240x320x18 bits. It can perform
display data RAM read/write operation with no external operation clock to
minimize power consumption. In addition, because of the integrated power
supply circuit necessary to drive liquid crystal; it is possible to make
a display system with the fewest components. Multiple communication interfaces
will by provided:

* Parallel 8080-series MCU Interface (8-bit, 9-bit, 16-bit & 18-bit)
* 6/16/18 RGB Interface (VSYNC, HSYNC, DOTCLK, ENABLE, DB[17:0])
* Serial Peripheral Interface (SPI Interface)
* VSYNC Interface

## References

* *HTML(2022-10-27)*: [AIoT DDI Catalog]
  – *Sitronix Digital Display Interface Product Catalog for AIoT devices*
* **PDF(2022-10-27)**: [ST7789V Datasheet (EN) V1.6, 2017/09]
  – *[original(2022-10-27)](https://www.crystalfontz.com/controllers/Sitronix/ST7789V/470)*
* **PDF(2022-10-27)**: [ST7789VW Datasheet (EN) V1.0, 2017/09]
  – *[original(2022-10-27)](https://www.waveshare.com/w/upload/a/ae/ST7789_Datasheet.pdf)*
* **PDF(2022-10-27)**: [ST7789V2 Datasheet (EN) V1.0, 2016/11]
  – *[original(2022-10-27)](https://m5stack.oss-cn-shenzhen.aliyuncs.com/resource/docs/datasheet/unit/lcd/ST7789V2_SPEC_V1.0.pdf)*
* **PDF(2022-10-27)**: [ST7789V Datasheet (EN) V1.4, 2014/10]
  – *[original(2022-10-27)](https://www.crystalfontz.com/controllers/Sitronix/ST7789V/446)*
* **PDF(2022-10-27)**: [ST7789VI Datasheet (EN) V1.4, 2014/04]
  – *[original(2022-10-27)](https://cdn.datasheetspdf.com/pdf-down/S/T/7/ST7789VI-Sitronix.pdf)*
* **PDF(2022-10-27)**: [ST7789V Datasheet (EN) V1.3, 2014/03]
  – *[original(2022-10-27)](https://newhavendisplay.com/content/datasheets/ST7789V.pdf)*
* **PDF(2022-10-27)**: [ST7789V Datasheet (EN) V1.0, 2013/10]
  – *[original(2022-10-27)](https://cdn.datasheetspdf.com/pdf-down/S/T/7/ST7789V-SitronixTechnology.pdf)*
* **PDF(2022-10-27)**: [ST7789V Datasheet (EN) V0.1, 2013/07] – Preliminary Version
  – *[original(2022-10-27)](https://www.crystalfontz.com/controllers/Sitronix/ST7789V/382)*

[AIoT DDI Catalog]: https://www.sitronix.com.tw/en/products/aiot-device-ddi "Sitronix AIoT device DDI Catalog"
[ST7789V Datasheet (EN) V1.6, 2017/09]: electronic/components/sitronix/ST7789V/ST7789V-datasheet-en-v1.6.pdf "2022-10-27: ST7789V Datasheet (EN), V1.6, 2017/09"
[ST7789VW Datasheet (EN) V1.0, 2017/09]: electronic/components/sitronix/ST7789V/ST7789VW-datasheet-en-v1.0.pdf "2022-10-27: ST7789VW Datasheet (EN), V1.0, 2017/09"
[ST7789V2 Datasheet (EN) V1.0, 2016/11]: electronic/components/sitronix/ST7789V/ST7789V2-datasheet-en-v1.0.pdf "2022-10-27: ST7789V2 Datasheet (EN), V1.0, 2016/11"
[ST7789V Datasheet (EN) V1.4, 2014/10]: electronic/components/sitronix/ST7789V/ST7789V-datasheet-en-v1.4.pdf "2022-10-27: ST7789V Datasheet (EN), V1.4, 2014/10"
[ST7789VI Datasheet (EN) V1.4, 2014/04]: electronic/components/sitronix/ST7789V/ST7789VI-datasheet-en-v1.4.pdf "2022-10-27: ST7789VI Datasheet (EN), V1.4, 2014/04"
[ST7789V Datasheet (EN) V1.3, 2014/03]: electronic/components/sitronix/ST7789V/ST7789V-datasheet-en-v1.3.pdf "2022-10-27: ST7789V Datasheet (EN), V1.3, 2014/03"
[ST7789V Datasheet (EN) V1.0, 2013/10]: electronic/components/sitronix/ST7789V/ST7789V-datasheet-en-v1.0.pdf "2022-10-27: ST7789V Datasheet (EN), V1.0, 2013/10"
[ST7789V Datasheet (EN) V0.1, 2013/07]: electronic/components/sitronix/ST7789V/ST7789V-datasheet-en-v0.1.pdf "2022-10-27: ST7789V Datasheet (EN), V0.1, 2013/07"
