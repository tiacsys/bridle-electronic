# ILI9341 – 240RGBx320 dot 262K Color TFT Controller/Driver

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-27</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/ilitek/ILI9341/chip-top-bot.svg "ILITEK ILI9341(V)"

The ILI9341(V) is a 262,144-color single-chip SOC driver for a-TFT liquid
crystal display with resolution of 240RGBx320 dots, comprising a 720-channel
source driver, a 320-channel gate driver, 172,800 bytes GRAM for graphic
display data of 240RGBx320 dots, and power supply circuit. It supports parallel
8-/9-/16-/18-bit data bus MCU interface, 6-/16-/18-bit data bus RGB interface
and 3-/4-line serial peripheral interface (SPI). The moving picture area can
be specified in internal GRAM by window address function. The specified window
area can be updated selectively, so that moving picture can be displayed
simultaneously independent of still picture area.

## References

* [ILI9341 vs. ILI9341V](https://www.avrfreaks.net/forum/ili9341-vs-ili9341v)
* *HTML(2022-10-27)*: [Small size driver IC Catalog]
  – *ILITEK small size driver IC Product Catalog*
* **PDF(2022-10-27)**: [ILI9341V Datasheet (EN) V1.0, 2013/04]
  – *[original(2022-10-27)](https://cdn.datasheetspdf.com/pdf-down/I/L/I/ILI9341V-ILITEK.pdf)*
  – *[original(2022-10-27)](https://www.crystalfontz.com/controllers/Ilitek/ILI9341V/143)*
* **PDF(2022-10-27)**: [ILI9341 Datasheet (EN) V1.13, 2011/07]
  – *[original(2022-10-27)](https://cdn.datasheetspdf.com/pdf-down/I/L/I/ILI9341_ILITEK.pdf)*
* **PDF(2022-10-27)**: [ILI9341 Datasheet (EN) V1.02, 2010/12] – Preliminary Version
  – *[original(2022-10-27)](https://www.digikey.com/htmldatasheets/production/1640716/0/0/1/ILI9341-Datasheet.pdf)*

[Small size driver IC Catalog]: http://www.ilitek.com/page/about/index.aspx?kind=9 "ILITEK Small size driver IC Catalog"
[ILI9341V Datasheet (EN) V1.0, 2013/04]: electronic/components/ilitek/ILI9341/ILI9341V-datasheet-en-v1.0.pdf "2022-10-27: ILI9341V Datasheet (EN), V1.0, 2013/04"
[ILI9341 Datasheet (EN) V1.13, 2011/07]: electronic/components/ilitek/ILI9341/ILI9341-datasheet-en-v1.13.pdf "2022-10-27: ILI9341 Datasheet (EN), V1.13, 2011/07"
[ILI9341 Datasheet (EN) V1.02, 2010/12]: electronic/components/ilitek/ILI9341/ILI9341-datasheet-en-v1.02.pdf "2022-10-27: ILI9341 Datasheet (EN), V1.02, 2010/12"
