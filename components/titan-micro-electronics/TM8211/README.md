# TM8211 – I²S digital output MEMS microphone with Multi‐modes

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-29</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/titan-micro-electronics/TM8211/chip-top-bot.png "Titan Micro Electronics TM8211"

The TM8211 is an Chinese replica of the TDA1311A "Stereo Continuous Calibration
DAC (CC-DAC)" designed by Philips, or the official replica
[PT8211](http://www.princeton.com.tw/en-us/products/multimediaaudioic/digitaltoanalogconverter.aspx)
by [Princeton Tech (PTC)](https://www.princeton.com.tw/).

TM8211 is a two-way 16-bit digital-to-analog conversion integrated circuit. The
chip is designed by CMOS process, the internal circuit structure is designed
based on the R-2R resistor network structure, and the dynamic range of 16-bit
is realized within the full power supply voltage range. TM8211 can support 8X
oversampling audio signal processing by using digital serial bus data input
and fast R-2R network structure. TM8211 supports a wide range of sampling
frequencies and is compatible with PT8211 and TDA1311. The input adopts
LSBJ (Least Significant Bit Justified) format, and the digital encoding
format adopts MSB-first complement format. The TM8211 is available in
an 8-pin SOP package.

## References

* *HTML(2022-10-29)*: [ADC/DAC Catalog]
  – *Titan Micro Analog-to-Digital/Digital-to-Analog Converter Product Lists*
* *HTML(2022-10-29)*: [TM8211 Product Page]
  – *Titan Micro TM8211 Product Page*
* **PDF(2022-10-29)**: [Datasheet (EN) v1.1]
* **PDF(2022-10-29)**: [Datasheet (CN) v1.1]
  – *[original(2022-10-29)](http://www.titanmec.com/index.php/product/download/id/609.html)*

[ADC/DAC Catalog]: http://www.titanmec.com/index.php/product/viewlist/typeid/95.html "Titan Micro Electronics ADC/DAC Catalog"
[TM8211 Product Page]: http://www.titanmec.com/index.php/product/view/id/609.html "Titan Micro Electronics TM8211 Product Page"
[Datasheet (EN) v1.1]: electronic/components/titan-micro-electronics/TM8211/datasheet-en-v1.1-20170703.pdf "2022-10-29: TM8211 Datasheet (EN), V1.1, Jul. 17, 2017"
[Datasheet (CN) v1.1]: electronic/components/titan-micro-electronics/TM8211/datasheet-cn-v1.1-20170703.pdf "2022-10-29: TM8211 Datasheet (CN), V1.1, Jul. 17, 2017"
