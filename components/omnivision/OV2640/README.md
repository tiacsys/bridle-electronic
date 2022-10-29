# OV2640 – 1/4＂UXGA CMOS Image Sensor (CIS)

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-28</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/omnivision/OV2640/chip-top-bot.svg "OmniVision OV2640 Block Diagram"

The OV2640 image sensor is a low voltage CMOS sensor that provides the full
functionality of a single-chip UXGA (1632 x 1232) camera and image processor
in a small footprint package. The OV2640 provides full-frame, sub-sampled,
scaled or windowed 8-bit/10-bit images in a wide range of formats, controlled
through the Serial Camera Control Bus (SCCB) interface.

This product has an image array capable of operating at up to 15 frames per
second (fps) in UXGA resolution with complete user control over image quality,
formatting and output data transfer. All required image processing functions,
including exposure control, gamma, white balance, color saturation, hue control,
white pixel canceling, noise canceling, and more, are also programmable through
the SCCB interface. The OV2640 also includes a compression engine for increased
processing power. In addition, OmniVision CameraChip™ products use proprietary
sensor technology to improve image quality by reducing or eliminating common
lighting/electrical sources of image contamination, such as fixed pattern noise,
smearing, etc., to produce a clean, fully stable color image.

* Standard optical format of 1/4 inch
* Various output formats: YUV422/420, YCbCr4:2:2, GRB422, RGB565/555,
  8-/10-bit Raw Bayer Data
* Supports image sizes: UXGA, SXGA, SVGA, and any size scaling down
  from SXGA to 40 x 30
* Variable frame rate control
* Automatic image control functions, 3A+
  * automatic exposure control (AEC)
  * automatic gain control (AGC)
  * automatic white balance (AWB)
  * automatic band filter (ABF)
  * automatic black-level calibration (ABLC)
* Supports LED and flash strobe mode
* Package: CSP2/wafer

## References

* *HTML(2022-10-28)*: [2MP CameraChip Product Page]
  – *WEBARCHIVE: OmniVision's archived web site from Nov. 10, 2011*
* *HTML(2022-10-28)*: [OV2640 Product Page]
  – *WEBARCHIVE: OmniVision's archived web site from Nov. 10, 2011*

[2MP CameraChip Product Page]: http://web.archive.org/web/20111101114839/http://www.ovt.com:80/products/category.php?id=10 "OmniVision's 2MP CameraChip Product Page from Nov. 10, 2011"
[OV2640 Product Page]: http://web.archive.org/web/20111014200352/http://ovt.com/products/sensor.php?id=3 "OmniVision's OV2640 Product Page from Nov. 10, 2011"

### Product Overview

* **PDF(2022-10-28)**: [OV2640 Product Brief v1.8.2.4]
  – *[original-WEBARCHIVE-20111110(2022-10-28)](http://web.archive.org/web/20111014201622if_/http://ovt.com/download_document.php?type=sensor&sensorid=3)*
  – *[original(2022-10-28)](https://www.waveshare.com/w/upload/a/af/OV2640.pdf)*
  – *[original(2022-10-28)](https://www.waveshare.com/wiki/OV2640_Camera_Board)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/media/archive/cf/e5/b0/RBS11633-Datenbl-tter.zip)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp)*

[OV2640 Product Brief v1.8.2.4]: electronic/components/omnivision/OV2640/OV2640-productbrief-v1.8.2.4-200605.pdf "2022-10-28: OV2640 Product Brief, V1.8.2.4, May, 2006"

### Product Specification

* **PDF(2022-10-28)**: [OV2640/OV2141 Datasheet v2.21]
  – *[original(2022-10-28)](https://www.plexishop.it/pdf/OV2640.pdf)*
* **PDF(2022-10-28)**: [OV2640/OV2141 Datasheet v2.2]
  – *[original(2022-10-28)](https://www.uctronics.com/download/OV2640_DS.pdf)*
  – *[original(2022-10-28)](https://www.arducam.com/ov2640)*
* **PDF(2022-10-28)**: [OV2640 Datasheet v1.8] – Preliminary
  – *[original(2022-10-28)](https://www.waveshare.com/w/upload/9/92/Ov2640_ds_1.8_.pdf)*
  – *[original(2022-10-28)](https://www.waveshare.com/wiki/OV2640_Camera_Board)*
* **PDF(2022-10-28)**: [OV2640FSL Datasheet v1.3] – Preliminary
  – *[original(2022-10-28)](https://www.mpja.com/download/ov2640data%20sheet.pdf)*
* **PDF(2022-10-28)**: [OV2640 Datasheet v1.6] – Preliminary
  – *[original(2022-10-28)](https://mangopi.org/_media/zh/ov2640ds.pdf)*
  – *[original(2022-10-28)](https://mangopi.org/doku.php?id=accessories&rev=1657178166)*
  – *[original(2022-10-28)](https://www.uctronics.com/download/cam_module/OV2640DS.pdf)*
  – *[original(2022-10-28)](https://dl.sipeed.com/fileList/MAIX/HDK/Chip_DS/OV2640-DATASHEET.pdf)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/media/archive/cf/e5/b0/RBS11633-Datenbl-tter.zip)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp)*

[OV2640/OV2141 Datasheet v2.21]: electronic/components/omnivision/OV2640/OV2640-OV2141-datasheet-v2.21-20070911.pdf "2022-10-28: OV2640/OV2141 Datasheet, V2.21, Sep. 11, 2007"
[OV2640 Datasheet v2.2]: electronic/components/omnivision/OV2640/OV2640-datasheet-v2.2-20070223.pdf "2022-10-28: OV2640/OV2141 Datasheet, V2.2, Feb. 23, 2007"
[OV2640 Datasheet v1.8]: electronic/components/omnivision/OV2640/OV2640-datasheet-v1.8-20060414.pdf "2022-10-28: OV2640 Datasheet, V1.8, Apr. 14, 2006"
[OV2640FSL Datasheet v1.3]: electronic/components/omnivision/OV2640/OV2640FSL-datasheet-v1.3-20060911.pdf "2022-10-28: OV2640FSL Datasheet, V1.3, Sep. 11, 2006"
[OV2640 Datasheet v1.6]: electronic/components/omnivision/OV2640/OV2640-datasheet-v1.6-20060228.pdf "2022-10-28: OV2640 Datasheet, V1.6, Feb. 28, 2006"

### Product Notes

* **PDF(2022-10-28)**: [OV2640 Camera Module Hardware Application Notes v1.04]
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/media/archive/cf/e5/b0/RBS11633-Datenbl-tter.zip)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp)*
* **PDF(2022-10-28)**: [OV2640 Camera Module Software Application Notes v1.03]
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/media/archive/cf/e5/b0/RBS11633-Datenbl-tter.zip)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp)*

[OV2640 Camera Module Hardware Application Notes v1.04]: electronic/components/omnivision/OV2640/OV2640-an-camera-module-hardware-v1.04-20071212.pdf "2022-10-28: OV2640 Datasheet, V1.04, Dec. 12, 2007"
[OV2640 Camera Module Software Application Notes v1.03]: electronic/components/omnivision/OV2640/OV2640-an-camera-module-software-v1.03-20071212.pdf "2022-10-28: OV2640 Datasheet, V1.03, Dec. 12, 2007"

### Supplementary Documentation (should sort in on another place)

#### OmniVision

* **PDF(2022-10-28)**: [OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.2]
  – *[original(2022-10-28)](https://docplayer.net/storage/54/34226126/1667045993/KypoUdVkQmb2dfz1GxQUBg/34226126.pdf)*
  – *[original(2022-10-28)](https://docplayer.net/34226126-Omnivision-serial-camera-control-bus-sccb-functional-specification.html)*
* **PDF(2022-10-28)**: [OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.1]
  – *[original(2022-10-28)](https://www.waveshare.com/w/upload/1/14/OmniVision_Technologies_Seril_Camera_Control_Bus%28SCCB%29_Specification.pdf)*
  – *[original(2022-10-28)](https://www.waveshare.com/wiki/File:OmniVision_Technologies_Seril_Camera_Control_Bus(SCCB)_Specification.pdf)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/media/archive/cf/e5/b0/RBS11633-Datenbl-tter.zip)*
  – *[original(2022-10-28)](https://www.roboter-bausatz.de/p/ov2640-kameramodul-cmos-sensor-2-mp)*
* **PDF(2022-10-28)**: [OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.0]
  – *[original(2022-10-28)](http://www4.cs.umanitoba.ca/~jacky/Teaching/Courses/74.795-LocalVision/ReadingList/ov-sccb.pdf)*

[OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.2]: electronic/components/omnivision/OV2640/sccb-functional-specification-v2.2-200070625.pdf "2022-10-28: SCCB Functional Specification, v2.2, Jun. 25, 2007"
[OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.1]: electronic/components/omnivision/OV2640/sccb-functional-specification-v2.1-20030226.pdf "2022-10-28: SCCB Functional Specification, v2.1, Feb. 26, 2003"
[OmniVision Serial Camera Control Bus (SCCB) Functional Specification v2.0]: electronic/components/omnivision/OV2640/sccb-functional-specification-v2.0-20020308.pdf "2022-10-28: SCCB Functional Specification, v2.0, Mar. 08, 2002"

#### 3rd party

This two documents reflect some parts related to the OmniVision *Digital Video
Port (**DVP**)* as introduced above with the [OV2640FSL Datasheet v1.3] and the
[OV2640 Camera Module Hardware Application Notes v1.04].

* **PDF(2022-10-28)**: [TDnext TDAIP01-EVB Users's Guide Rev 1.0]
  – **page 21**: *6.1 Camera Interfaces*, *Figure 18. FH12-24S-0.5SH Connector*,
  *Table 3. FH12-24S-0.5SH connector pin descriptions*
  – *[original(2022-10-28)](https://s3-eu-west-1.amazonaws.com/assetstdnext/download/camera/tdaip01/TDAIP01-EVB+User's+Guide+rev1.0.pdf)*
  – *[original(2022-10-28)](http://cammodules.td-next.com/tdaip01)*
* **PDF(2022-10-28)**: [FTDI TN-158 What is the Camera Parallel Interface? v1.0]
  – *[original(2022-10-28)](https://www.ftdichip.com/Support/Documents/TechnicalNotes/TN_158_What_Is_The_Camera_Parallel_Interface.pdf)*

[TDnext TDAIP01-EVB Users's Guide Rev 1.0]: electronic/components/omnivision/OV2640/tdnext-tdaip01-evb-user-guide-rev1.0-201702.pdf "2022-10-28: TDnext TDAIP01-EVB Users's Guide, Rev 1.0, February 2017"
[FTDI TN-158 What is the Camera Parallel Interface? v1.0]: electronic/components/omnivision/OV2640/ftdi-tn-158-v1.0-20150323.pdf "2022-10-28: FTDI TN-158, v1.0, Mar. 23, 2005"
