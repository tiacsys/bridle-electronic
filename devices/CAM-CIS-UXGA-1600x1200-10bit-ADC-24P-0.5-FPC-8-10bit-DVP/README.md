# UXGA CMOS Image Sensor with 1600 x 1200, 10-bit ADC, 8/10-bit DVP

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-28</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![part-iso]][part-iso]</span>

[part-iso]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/RYS-2640-M7/part-iso.png "UXGA CIS 10-bit ADC 1600x1200 8/10-bit DVP"

These kinds of cheap and simple CIS cameras are mostly no-name mass-produced
goods from China:

* **Array Technology**: 2MP CMOS Image Sensor (CIS)
* **Array Size**: 1/4 inch and the resolution is 1600x1200 dot (UXGA)
* **Sensor IC**: [OmniVision OV2640]
* **Output Format**: YUV422/420, YCbCr422, GRB422, RGB565/555, 8-/10-bit Raw RGB Bayer Data
* **Interface**:
  * 8-/10-bit DVP for sensor image data
  * I2C for sensor IC setup (OmniVision's SCCB)
  * *optional*: strobe mode
* **Connector**:
  * 24 pin 0.5mm FPC for 8/10-bit Digital Video Port (DVP)

[OmniVision OV2640]: index.php?dir=electronic/components/omnivision/OV2640 "1600x1200 10-bit UXGA CMOS Image Sensor"

| Common Mechanical Drawing (OV2640: 8-bit, NO strobe) | Common Mechanical Drawing (OV2640: 10-bit, strobe) |
|::|::|
| [![part-common-mechdraw-ov2640-8bit]][part-common-mechdraw-ov2640-8bit] | [![part-common-mechdraw-ov2640-10bit-strobe]][part-common-mechdraw-ov2640-10bit-strobe] |

[part-common-mechdraw-ov2640-8bit]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/ali-drawing-ov2640-8bit-cam.png "UXGA CIS 8-bit Common Mechanical Drawing"
[part-common-mechdraw-ov2640-10bit-strobe]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/ali-drawing-ov2640-10bit-strobe-cam.png "UXGA CIS 10-bit strobe Common Mechanical Drawing"

| MANUFACTOR / DISTRIBUTOR / TYP / IC | Specification | PCBA Top / Bottom |
|::|::|::|
| **RYS-2640-M7** <br/> [OV2640][OmniVision OV2640] <br/> (10bit/strobe) | [![RYS-2640-M7-draw]][RYS-2640-M7-draw] | [![RYS-2640-M7-iso]][RYS-2640-M7-iso] |
| **DCX-OV2640-V2** <br/> [OV2640][OmniVision OV2640] <br/> (10bit/strobe) | [![DCX-OV2640-V2-draw]][DCX-OV2640-V2-draw] | [![DCX-OV2640-V2-pcba]][DCX-OV2640-V2-pcba] |
| **HDF3M-811XR** <br/> [OV2640][OmniVision OV2640] <br/> (10bit/strobe) | [![HDF3M-811XR-draw]][HDF3M-811XR-draw]  [![HDF3M-811XR-con24p]][HDF3M-811XR-con24p] | [![HDF3M-811XR-pcba]][HDF3M-811XR-pcba]  [![HDF3M-811XR-sch]][HDF3M-811XR-sch] |
| **HDF3M-811XR** <br/> [OV2640][OmniVision OV2640] <br/> (8bit) | [![HDF3M-811XR-draw-alt-1]][HDF3M-811XR-draw-alt-1]  [![HDF3M-811XR-con24p-alt-1]][HDF3M-811XR-con24p-alt-1] | [![HDF3M-811XR-prod-alt-1]][HDF3M-811XR-prod-alt-1] |
| **OV2640-75MM** <br/> [OV2640][OmniVision OV2640] <br/> (8bit) | [![OV2640-75MM-draw]][OV2640-75MM-draw] | [![OV2640-75MM-pcba]][OV2640-75MM-pcba] |

[RYS-2640-M7-draw]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/RYS-2640-M7/part-draw.jpg "RYS-2640-M7 Mechanical Drawing"
[RYS-2640-M7-iso]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/RYS-2640-M7/part-iso.png "RYS-2640-M7 PCBA Perspective View"

[DCX-OV2640-V2-draw]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/DCX-OV2640-V2/part-draw.jpg "DCX-OV2640-V2 Mechanical Drawing"
[DCX-OV2640-V2-pcba]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/DCX-OV2640-V2/part-pcba.png "DCX-OV2640-V2 PCBA Top / Bottom View"

[HDF3M-811XR-con24p]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-con24p.jpg "HDF3M-811XR Connector Pin Assignment"
[HDF3M-811XR-draw]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-draw.jpg "HDF3M-811XR Mechanical Drawing"
[HDF3M-811XR-pcba]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-pcba.png "HDF3M-811XR PCBA Top / Bottom View"
[HDF3M-811XR-sch]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-sch.jpg "HDF3M-811XR Schematic"
[HDF3M-811XR-prod-alt-1]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-prod-alt-1.jpg "HDF3M-811XR Alternative w/o Strobe Mode"
[HDF3M-811XR-con24p-alt-1]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-con24p-alt-1.jpg "HDF3M-811XR Connector Pin Assignment"
[HDF3M-811XR-draw-alt-1]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/HDF3M-811XR/part-draw-alt-1.jpg "HDF3M-811XR Mechanical Drawing"

[OV2640-75MM-draw]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/OV2640-75MM/part-draw.png "OV2640-75MM Mechanical Drawing"
[OV2640-75MM-pcba]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/OV2640-75MM/part-pcba.png "OV2640-75MM PCBA Top / Bottom View"

## Origins

* MangoPi: [Accessories](https://mangopi.org/doku.php?id=accessories&rev=1657178166)
* Alibaba: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.alibaba.com/product-detail/Lichee-pi-Camera-OV2640-OV5647-M12_1600290944138.html)
* AliExpress: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.aliexpress.com/item/1005003317184621.html)
* AliExpress: [Licheepi Sipeed Camera OV2640 OV5647 GC0328](https://www.aliexpress.com/item/1005002907961007.html)
* AliExpress: [New OV2640 Camera Module for ESP32 CAM](https://www.aliexpress.com/item/1005004518669324.html)
* AliExpress: [OV2640 Camera Module for TTGO T-Camera Plus](https://www.aliexpress.com/item/1005001321193803.html)
* AliExpress: [ESP32 module 66/120/160 degree OV2640](https://www.aliexpress.com/item/1005002260523682.html)
* AliExpress: [ESP32 OV2640 Camera Module CMOS Image Sensor Module](https://www.aliexpress.com/item/4000061425990.html)
* AliExpress: [Pi/Widora Camera OV2640 GC0328 Dual Camera](https://de.aliexpress.com/item/1005004575626641.html)

### Reference Schematics

| **(1)** [OV2640][OmniVision OV2640] (8-bit / 24 MHz / 2.8 Volt) [origin](https://blog.csdn.net/weixin_34199764/article/details/112381435) |
|::|
| [![part-common-sch-ov2640-8bit-24mhz-2v8]][part-common-sch-ov2640-8bit-24mhz-2v8] |

[part-common-sch-ov2640-8bit-24mhz-2v8]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/csdn-112381435-sch-ov2640-8bit-24mhz-2v8.jpg "OV2640 Reference Schematic 1"

| **(2)** [OV2640][OmniVision OV2640] (8-bit / 24 MHz / 1.3 Volt) [origin](https://www.aliexpress.com/i/4000181941178.html) |
|::|
| [![part-common-sch-ov2640-8bit-24mhz-1v3]][part-common-sch-ov2640-8bit-24mhz-1v3] |

[part-common-sch-ov2640-8bit-24mhz-1v3]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/csdn-112381435-sch-ov2640-8bit-24mhz-1v3.jpg "OV2640 Reference Schematic 2"

| **(3)** [OV2640][OmniVision OV2640] (8-bit / 12 MHz / 1.3 Volt) [origin](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp) |
|::|
| [![part-common-sch-ov2640-8bit-12mhz-1v3]][part-common-sch-ov2640-8bit-12mhz-1v3] |
| [![part-common-pcb-ov2640-8bit-12mhz-1v3]][part-common-pcb-ov2640-8bit-12mhz-1v3] |

[part-common-sch-ov2640-8bit-12mhz-1v3]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/csdn-112381435-sch-ov2640-8bit-12mhz-1v3.jpg "OV2640 Reference Schematic 3"
[part-common-pcb-ov2640-8bit-12mhz-1v3]: electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP/csdn-112381435-pcb-ov2640-8bit-12mhz-1v3.jpg "OV2640 Reference PCB Layout 3"
