# VGA CMOS Image Sensor with 640 x 480, 10-bit ADC, 8-bit DVP

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-28</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![part-iso]][part-iso]</span>

[part-iso]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-T01-GA4.2/part-iso.png "VGA CIS 10-bit ADC 640x480 8-bit DVP"

These kinds of cheap and simple CIS cameras are mostly no-name mass-produced
goods from China:

* **Array Technology**: 0.3MP CMOS Image Sensor (CIS)
* **Array Size**: 1/6.5 inch and the resolution is 640x480 dot (VGA)
* **Sensor IC**: [GalaxyCore GC0328]
* **Output Format**: YCbCr422, RGB565/555/444, 10-bit Raw RGB Bayer Data
* **Interface**:
  * 8-/10-bit DVP for sensor image data
  * I2C for sensor IC setup
  * *optional*: strobe mode
* **Connector**:
  * 24 pin 0.5mm FPC for 8-bit Digital Video Port (DVP)

[GalaxyCore GC0328]: index.php?dir=electronic/components/galaxygore/GC0328 "640x480 10-bit VGA CMOS Image Sensor"
[OmniVision OV2640]: index.php?dir=electronic/components/omnivision/OV2640 "1600x1200 10-bit UXGA CMOS Image Sensor"

| MANUFACTOR / DISTRIBUTOR / TYP / IC | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Specification&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | PCBA Top / Bottom |
|::|::|::|
| **ZV-T01-GA4.2** <br/> [GC0328][GalaxyCore GC0328] <br/> *also seen on product photos*: <br/> **[ZV-T01-GA4.4]**, or **ZV-SP-B-GA4.4** | [![ZV-T01-GA4.2-draw]][ZV-T01-GA4.2-draw]  [![ZV-T01-GA4.2-con24p]][ZV-T01-GA4.2-con24p] | [![ZV-T01-GA4.2-iso]][ZV-T01-GA4.2-iso] |
| **ZV-Sipeed-GA4A4.3** <br/> [GC0328][GalaxyCore GC0328] <br/> *also seen on product photos*: <br/> **ZV-XS-GA4A4.4**, or **[…-GA4A4.4-V1.0]** eg.: **[Widora-GA4A4.4-V1.0]** | [![ZV-Sipeed-GA4A4.3-draw]][ZV-Sipeed-GA4A4.3-draw]  [![ZV-Sipeed-GA4A4.3-con24p]][ZV-Sipeed-GA4A4.3-con24p] | [![ZV-Sipeed-GA4A4.3-iso]][ZV-Sipeed-GA4A4.3-iso]  [![…-GA4A4.4-pcba]][…-GA4A4.4-pcba] |
| **ZV-Sipeed-GA4A4.4** <br/> [GC0328][GalaxyCore GC0328] | [![ZV-Sipeed-GA4A4.4-draw]][ZV-Sipeed-GA4A4.4-draw]  [![ZV-Sipeed-GA4A4.4-con24p]][ZV-Sipeed-GA4A4.4-con24p] | [![ZV-Sipeed-GA4A4.4-pcba]][ZV-Sipeed-GA4A4.4-pcba]  [![ZV-XS-GA4A4.4-pcba]][ZV-XS-GA4A4.4-pcba] |

[ZV-T01-GA4.2-con24p]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-T01-GA4.2/part-con24p.jpg "ZV-T01-GA4.2 Connector Pin Assignment"
[ZV-T01-GA4.2-draw]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-T01-GA4.2/part-draw.jpg "ZV-T01-GA4.2 Mechanical Drawing"
[ZV-T01-GA4.2-iso]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-T01-GA4.2/part-iso.png "ZV-T01-GA4.2 PCBA Perspective View"
[ZV-T01-GA4.4]: #ZV-T01-GA4.4 "ZV-T01-GA4.4"

[ZV-Sipeed-GA4A4.3-con24p]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.3/part-con24p.jpg "ZV-Sipeed-GA4A4.3 Connector Pin Assignment"
[ZV-Sipeed-GA4A4.3-draw]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.3/part-draw.jpg "ZV-Sipeed-GA4A4.3 Mechanical Drawing"
[ZV-Sipeed-GA4A4.3-iso]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.3/part-iso.png "ZV-Sipeed-GA4A4.3 PCBA Perspective View"
[Widora-GA4A4.4-V1.0]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.3/widora-ga4a4.4-v1.0.pdf "MangoPi's Widora-GA4A4.4-V1.0 Mechanical Drawing by Shenzhen Sunyu Electronic Technology Co."
[…-GA4A4.4-pcba]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.3/part-pcba-alt-1.png "ZV-Sipeed-GA4A4.4 PCBA Alternative Top View"
[…-GA4A4.4-V1.0]: #…-GA4A4.4-V1.0 "…-GA4A4.4-V1.0"

[ZV-Sipeed-GA4A4.4-con24p]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.4/part-con24p.jpg "ZV-Sipeed-GA4A4.4 Connector Pin Assignment"
[ZV-Sipeed-GA4A4.4-draw]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.4/part-draw.jpg "ZV-Sipeed-GA4A4.4 Mechanical Drawing"
[ZV-Sipeed-GA4A4.4-pcba]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.4/part-pcba.png "ZV-Sipeed-GA4A4.4 PCBA Top / Bottom View"
[ZV-XS-GA4A4.4-pcba]: electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP/ZV-Sipeed-GA4A4.4/part-pcba-alt-1.png "ZV-Sipeed-GA4A4.4 PCBA Alternative Top View"

## Origins

* MangoPi: [Accessories](https://mangopi.org/doku.php?id=accessories&rev=1657178166)
* Alibaba: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.alibaba.com/product-detail/Lichee-pi-Camera-OV2640-OV5647-M12_1600290944138.html)
* AliExpress: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.aliexpress.com/item/1005003317184621.html)
* AliExpress: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.aliexpress.com/item/1005002907961007.html)
* AliExpress: [Pi/Widora Camera OV2640 GC0328 Dual Camera](https://de.aliexpress.com/item/1005004575626641.html)

## Notes and References

<span id="ZV-T01-GA4.4">
### ZV-T01-GA4.4

**ATTENTION: my own speculation and interpretation!**

This type can be populated with [OmniVision OV2640] 2MP sensor
**in very rare cases**. See for this:

* Seeed: [Include Camera module changed?](https://forum.seeedstudio.com/t/seeed-studio-sipeed-maixduino-kit-for-risc-v-ai-iot-include-camera-module-changed/251854)
* GitHub: [sipeed/Maixduino/issues/73](https://github.com/sipeed/Maixduino/issues/73#issuecomment-646637974)
* CSDN: [gc0328 dual camera driver](https://blog.csdn.net/weixin_34199764/article/details/112381435)

<span id="…-GA4A4.4-V1.0">
### …-GA4A4.4-V1.0

**ATTENTION: my own speculation and interpretation!**

This type can be populated with [OmniVision OV2640] 2MP sensor
**in very rare cases**. See for this:

* AliExpress: [Pi/Widora Camera OV2640 GC0328 Dual Camera](https://de.aliexpress.com/item/1005004575626641.html)
