# GC0328 – 1/6.5＂VGA CMOS Image Sensor (CIS)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-28</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/galaxygore/GC0328/chip-top-bot.svg "GalaxyCore GC0328 Block Diagram"

The GC0328 features 640V x 480H resolution with 1/6.5-inch optical format, and
4-transistorpixel structure for high image quality and low noise variations. It
delivers superior image quality by powerful on-chip design of a 10-bit ADC, and
embedded image signal processor. The full scale integration of high-performance
and low-power functions makes the GC0328 fit the design, reduce implementation
process, and extend the battery life of cell phones, PDAs, and a wide variety
of mobile applications. The product is capable of operating at up to 30 fps at
24 MHz clock in VGA mode, which can be completely controlled by user over image
quality and data format.

* Standard optical format of 1/6.5 inch
* Various output formats: YCbCr4:2:2, RGB565, Raw Bayer
* Support adjusting Voltage of IO
* Windowing support
* Horizontal / Vertical mirror
* Image processing module
* Interface: I2C and 8-bit DVP (D7:0 with CLK and H/VSYNC)
* Package: CSP/wafer

## References

* *HTML(2022-10-28)*: [Camera Image Sensor Catalog], under 1M pixel
  – *GalaxyCore CIS for Mobile Phone*
* **PDF(2022-10-28)**: [GC0328C Datasheet v1.0]
  – *[original(2022-10-28)](https://mangopi.org/_media/gc0328c_datasheet_released_v1.0_20140930.pdf)*
  – *[original(2022-10-28)](https://mangopi.org/doku.php?id=accessories&rev=1657178166)*

[Camera Image Sensor Catalog]: https://www.gcoreinc.com/products/index?cid=2&subcid=6 "GalaxyCore CIS (DVP/SPI) Catalog"
[GC0328C Datasheet v1.0]: electronic/components/galaxygore/GC0328/datasheet-en-v1.0-20140930.pdf "2022-10-28: GC0328C Datasheet (EN), V1.0, Sep. 30, 2014"
