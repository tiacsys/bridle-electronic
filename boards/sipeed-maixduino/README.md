# SiPEED MaixDuino (Kit) for RISC-V AI + IoT

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-29</strong></em></small>
</div>

[Fm]: electronic/.logos/dir-blk.png "Folder on Mirror"
[iFm]: electronic/.logos/dir-blk-inline.png "Folder on Mirror"
[Fo]: electronic/.logos/dir-red.png "Folder on Origin"
[iFo]: electronic/.logos/dir-red-inline.png "Folder on Origin"
[Dm]: electronic/.logos/doc-blk.png "Download from Mirror"
[iDm]: electronic/.logos/doc-blk-inline.png "Download from Mirror"
[Do]: electronic/.logos/doc-red.png "Download from Origin"
[iDo]: electronic/.logos/doc-red-inline.png "Download from Origin"
[Cm]: electronic/.logos/cab-blk.png "Download from Mirror"
[iCm]: electronic/.logos/cab-blk-inline.png "Download from Mirror"
[Co]: electronic/.logos/cab-red.png "Download from Origin"
[iCo]: electronic/.logos/cab-red-inline.png "Download from Origin"
[Wm]: electronic/.logos/web-blk.png "Document from Mirror"
[iWm]: electronic/.logos/web-blk-inline.png "Document from Mirror"
[Wo]: electronic/.logos/web-red.png "Document from Origin"
[iWo]: electronic/.logos/web-red-inline.png "Document from Origin"
[Gm]: electronic/.logos/git-blk.png "Repository from Mirror"
[iGm]: electronic/.logos/git-blk-inline.png "Repository from Mirror"
[Go]: electronic/.logos/git-red.png "Repository from Origin"
[iGo]: electronic/.logos/git-red-inline.png "Repository from Origin"

## About

<span style="width:256px;float:right;">[![board-iso]][board-iso]</span>

[board-iso]: electronic/boards/sipeed-maixduino/board-iso.png "SiPEED MaixDuino"

The **SiPEED MaixDuino (Kit)** for RISC-V AI + IoT includes the [Maix-I M1]
SoM that is based on the [K210] RISC-V 64 SoC and is ideal for AI + IoT
applications. MaixDuino was designed in an Arduino Uno form factor, different
from other SiPEED Maix-I development boards. The MaixDuino features an
[ESP32-WROOM-32] SoM on board together with the [Maix-I M1] M1 AI module.
The [K210] includes a dual-processor chip with two independent FPU, 64-bits
CPU bit width, 8MB on-chip SRAM, 400 adjustable nominal frequency and
double-precision FPU. The [K210] is equipped with neural network hardware
accelerator KPU, voice processing unit (APU), programmable IO array
(FPIOA/IOMUX), and Fast Fourier Transform (FFT) accelerator. Typical
applications include smart home (robotic vacuum cleaner and smart cleaner),
medical device, industry 4.0, agriculture, and education. The [ESP32-WROOM-32]
module rounds up the development board with basic WiFi/Bluetooth v4.2 and
Bluetooth Low Energy support, **ready for AIoT (AI + IoT) Edge Computing**.

This kit offers additional on-board components and accessories:

* an 8-bit MCU LCD 24P 0.5mm FPC connector for the enclosed
  [2.4inch TFT display][LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU]
* an 24P 0.5mm FPC connector for the DVP camera that comes all with the kit:
  * [CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP] with [GC0328] or
  * [CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP] with [OV2640]
* an on-board omnidirectional I2S digital output MEMS microphone [MSM261S4030H0]
* an 3W DAC+PA audio output (mono over 2-pin 1.25mm connector):
  * [TM8211]: 16 bit dynamic range and low harmonic distortion D/A-Converter (DAC)
  * [NS4150]: 3W output power and up to 90% efficiency Class-D Power Amplifier (PA)
* USB to serial port over [CH552]:
  * Port 0: ISP to [Maix-I M1] module, [K210]
  * Port 1: ISP to [ESP32-WROOM-32] module
* Reset and boot flag button and usr 3-color RGB LED
* uFL connector for WiFi and BT antenna

[K210]: index.php?dir=electronic/components/canaan/K210 "Canaan Kendryte K210"
[Maix-I M1]: index.php?dir=electronic/components/sipeed/Maix-I "SiPEED Maix-I M1"
[ESP32-WROOM-32]: https://www.espressif.com/en/products/modules/esp32 "Xtensa LX3 32-bit dual­core with 4 MB Flash (on module), 448 kB ROM and 520 kB RAM, AES-128/256, Hash, RSA, integrated BT-LE 4.2, IEEE 802.11 b/g/n WiFi radio"
[LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU]: index.php?dir=electronic/devices/LCD-TFT-2.4inch-240x320-RGB262K-24P-0.5-FPC-8bit-MCU "2.4 inch TFT-LCD with 240x3(RGB) x 320, 262K colors, 8-bit MCU"
[CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP]: index.php?dir=electronic/devices/CAM-CIS-VGA-640x480-10bit-ADC-24P-0.5-FPC-8bit-DVP "VGA CIS with 640 x 480, 10-bit ADC, 8-bit DVP"
[CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP]: index.php?dir=electronic/devices/CAM-CIS-UXGA-1600x1200-10bit-ADC-24P-0.5-FPC-8-10bit-DVP "UXGA CIS with 1600 x 1200, 10-bit ADC, 8/10-bit DVP"
[GC0328]: index.php?dir=electronic/components/galaxygore/GC0328 "640x480 10-bit VGA CMOS Image Sensor"
[OV2640]: index.php?dir=electronic/components/omnivision/OV2640 "1600x1200 10-bit UXGA CMOS Image Sensor"
[MSM261S4030H0]: index.php?dir=electronic/components/memsensing-microsystems/MSM261S4030H0 "I²S digital output MEMS microphone with Multi‐modes"
[TM8211]: index.php?dir=electronic/components/titan-micro-electronics/TM8211 "two-way 16-bit DAC for audio application"
[NS4150]: index.php?dir=electronic/components/nsiway/NS4150 "3W mono Class-D audio power amplifier"
[CH552]: http://www.wch-ic.com/products/CH552.html "8-bit USB Device MCU"

### Common Features and Specifications

* Built-in neural network processor (KPU + APU + FFT)
* Connector: compatible with Arduino interface TF card slot, speaker port
* Dimensions: 68mm × 54mm
* Power input: USB Type-C (6V to 12V)
* Temperature rise: <20K
* Operating temperature range: -30°C to 85°C
* Wireless: support 2.4G 802.11/b/g/n and Bluetooth 4.2
* Frequency range: 2400MHz to 2483.5MHz
* Transmit power:
  * 802.11.b: +15dBm
  * 802.11.g: +10dBm (54Mbps)
  * 802.11.n: +10dBm (65Mbps)
* Wireless connector: IPEX 3mm × 3mm
* WiFi mode: Station / SoftAP / SoftAP + Station

| PCB Layer | PCB 3D or Footprint | PCB Populated (top & bottom) |
|::|::|::|
| <div style="background-color:white;"><div style="width:65%;display:inline-block"><mark><strong>Eagle or Altium <em>PCB Layer</em> output is missing!</strong></mark></div></div> |<div style="background-color:white;"><div style="width:65%;display:inline-block"><mark><strong>Eagle or Altium <em>PCB 3D / Footprint</em> output is missing!</strong></mark></div></div> | <div style="background-color:white;"><div style="width:50%;display:inline-block">[![pcb-assembly-top]][pcb-assembly-top]</div></div> |
| | | <div style="background-color:white;"><div style="width:50%;display:inline-block">[![pcb-assembly-bot]][pcb-assembly-bot]</div></div> |

[pcb-assembly-top]: electronic/boards/sipeed-maixduino/pcb-assembly-top.png "SiPEED MaixDuino PCB Assembly (top)"
[pcb-assembly-bot]: electronic/boards/sipeed-maixduino/pcb-assembly-bot.png "SiPEED MaixDuino PCB Assembly (bottom)"

## References

**EAN**: #############<br/>
**UPC**:  ############<br/>
**SKU**: 110110044 / 102991184 (only development board)

**HSCODE**:   [8543.70.90.99]<br/>
**EUHSCODE**: [8543.70.90.99]<br/>
**USHSCODE**: [8471.49.00.00]<br/>
**COO**: CHINA

[8543.70.90.99]: https://www.tariffnumber.com/2022/85437090 "HS Code 85437090 – Electrical, machines, apparatus – Other"
[8471.49.00.00]: https://www.tariffnumber.com/2022/84714900 "HS Code 84714900 - Data, processing, machines – Other, presented in the form of systems"

*Brand*: Seeed<br/>
*Part number*: 113991054

* *HTML(2022-10-29)*: [SiPEED Product Page] – *$41-51 (**incl.** VAT)*
* *HTML(2022-10-29)*: [DFRobot Product Page] – *$36.90 (excl. VAT)*
* *HTML(2022-10-29)*: [Seeed Studio Product Page] – *$28.40 (excl. VAT)*
* *HTML(2022-10-29)*: [Seeed Studio Kit Product Page] – *$34.90 (excl. VAT)*
* **PDF(2022-10-29)**: [SiPEED Specification v1.0]
  – *[original(2022-10-29)](https://www.mouser.de/pdfDocs/SipeedMaixduinoSpecifications_ENV10.pdf)*
* **PDF(2022-10-29)**: [Seeed Studio (Mouser) Product Overview 08-17-2022]
  – *[original(2022-10-29)](https://www.mouser.com/pdfDocs/Product_Overview-SeeedStudioSipeedMaixduinoKit.pdf)*

[SiPEED Product Page]: https://www.aliexpress.com/item/1005002547345797.html "SiPEED MaixDuino Kit in AliExpress On-Line-Shop by SiPEED"
[DFRobot Product Page]: https://www.dfrobot.com/product-1965.html "DFRobot MaixDuino AI Development Kit K210 RISC-V AI + ESP32 IoT"
[Seeed Studio Product Page]: https://www.seeedstudio.com/Sipeed-Maixduino-for-RISC-V-AI-IoT-p-4046.html "Seeed Studio MaixDuino for RISC-V AI + IoT"
[Seeed Studio Kit Product Page]: https://www.seeedstudio.com/Sipeed-Maixduino-Kit-for-RISC-V-AI-IoT-p-4047.html "Seeed Studio MaixDuino Kit for RISC-V AI + IoT"
[SiPEED Specification v1.0]: electronic/boards/sipeed-maixduino/specification-en-v1.0-20190509.pdf "2022-10-29: SiPEED MaixDuino Specification (EN), V1.0, May 09, 2019"
[Seeed Studio (Mouser) Product Overview 08-17-2022]: electronic/boards/sipeed-maixduino/product-overview-en-seeed-mouser-20220817.pdf "2022-10-29: Seeed Studio MaixDuino Specification by Mouser (EN), Aug. 17, 2022"

| Pinout |
|::|
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-pinout]][board-pinout]</div></div> |
| **Appearance and Functions** |
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![board-functions]][board-functions]</div></div> |

[board-pinout]: electronic/boards/sipeed-maixduino/board-pinout.png "SiPEED MaixDuino Pinout"
[board-functions]: electronic/boards/sipeed-maixduino/board-functions.jpg "SiPEED MaixDuino Appearance and Functions"

## Documentation

* **PDF(2022-10-29)**: [MaixDuino]
  – *[HTML(2022-10-29)](https://wiki.sipeed.com/soft/maixpy/zh/develop_kit_board/maix_duino.html)*
* **PDF(2022-10-29)**: [MaixDuino development board]
  – *[HTML(2022-10-29)](https://wiki.sipeed.com/hardware/zh/maix/maixpy_develop_kit_board/maix_duino.html)*
* **HTML(2022-10-29)**: [Maixduino Documentation]
  – *latest on-line documentation for Arduino and PlatformIO*

[MaixDuino]: electronic/boards/sipeed-maixduino/maixduino.pdf "2022-10-29: Last updated on: October 28, 2022"
[MaixDuino development board]: electronic/boards/sipeed-maixduino/maixduino-development-board.pdf "2022-10-29: Last updated on: July 06, 2022"
[Maixduino Documentation]: https://maixduino.sipeed.com/ "English Documentation or 中文文档 (Chinese)"

| Name | Versions | Date | Mirror | Original | Storage |
|:-|::|::|::|::|::|
|  |  |  |  |  |  |
| <h3>HDK</h3> |  |  |  |  |  |
| <span style="width:96px;float:right;">[![outline-dimension]][outline-dimension]</span> **MaixDuino DXF Outline Dimension** *(by Altium)* | **V4.30** | **2020-04-28** | [![Dm]][outline-dimension.dxf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832/MaixDuino-4.30%28size%29.DXF) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| **MaixDuino DWG Outline Dimension** *(by VariCAD Viewer)* | **V4.30** | **2020-04-28** | [![Dm]][outline-dimension.dwg] |  |  |
| <span style="width:96px;float:right;">[![outline-3d-model]][outline-3d-model]</span> **MaixDuino STEP 3D Model** *(by KiCad)* | **2832** | **2020-08-18** | [![Dm]][outline-3d-model.stp] | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| **MaixDuino PDF Schematic** *(by KiCad)* | **2832** | **2020-08-13** | [![Dm]][schematic-2832-20200813-kicad.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832/Maixduino_2832%28Schematic%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| **MaixDuino PDF Assembly Drawing** *(by KiCad)* | **2832** | **2020-05-30** | [![Dm]][assembly-drawing-2832-20200530-kicad.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832/Maixduino-2832%28Assembly%20drawing%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| <h4>Documentations</h4> |  |  |  |  |  |
| **MaixDuino Excel Pin Assignment Table** | **2832** | **2020-05-30** | [![Dm]][pin-assignment-table-2832-20200530.xlsx] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832/MaixDunio_2832%28Pin%20assignment%20table%29.xlsx) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| **MaixDuino Excel Pin Assignment Table** | **V4.30** | **2020-04-28** | [![Dm]][pin-assignment-table-v4.30-20200428.xlsx] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832/MaixDunio%28Pin%20assignment%20table%29.xlsx) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Maixduino_2832) |
| **MaixDuino Datasheet** | **V1.0** | **2019-03-16** | [![Dm]][datasheet-en-v1.0-20190316.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-Maixduino/Specifications/Sipeed%20Maixduino%20Datasheet%20V1.0.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-Maixduino/Specifications) |
| <h3>SDK</h3> |  |  |  |  |  |
| <h4>CH552 8-bit USB Device MCU Firmware</h4> |  |  |  |  |  |
| <h5>8051 Firmware to simulate an FT2232</h5> <p>An USB to Serial Converter firmware running on CH552T. It also can automatically <br/> detect ESP32 & K210 bootloader message, force it enter ISP mode without help <br/> from FLOW CONTROL PINs (DTR/RTS).</p> | [v1.2](https://github.com/diodep/ch55x_dualserial/releases/tag/v1.2) | **2020-12-03** |  | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/factory_firmware/ch552) | [![Go]](https://github.com/diodep/ch55x_dualserial) |
| <h4>ESP32 32-Bit WiFi/BT Radio Firmware</h4> |  |  |  |  |  |
| <h5>Adafruit fork of the Arduino NINA-W102 firmware</h5> <p>This is the Adafruit fork of the Arduino NINA-W102 firmware. The original repository <br/> is located at https://github.com/arduino/nina-fw</p> | **[v1.4.1](https://github.com/sipeed/Maixduino_esp32_fimware/releases/tag/v1.4.1)** | **2020-05-26** |  | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/factory_firmware/esp32) | [![Go]](https://github.com/sipeed/Maixduino_esp32_fimware) |
| <h4>Maix-I M1 64-Bit Maixduino Firmware</h4> |  |  |  |  |  |
| <h5>MaixPy AIoT Micropython for K210 based devices</h5> <p>Refer install documentation in SiPEED Wiki: <br/> https://wiki.sipeed.com/soft/maixpy/zh/get_started/upgrade_maixpy_firmware.html</p> | **[v0.6.2](https://github.com/sipeed/MaixPy/releases/tag/v0.6.2)** | **2020-12-23** |  | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/MaixPy/release/master) | [![Go]](https://github.com/sipeed/MaixPy) |
| <h5>Arduino Core for K210 based devices</h5> <p>Refer install documentation in SiPEED Wiki: <br/> https://maixduino.sipeed.com/en/get_started/install.html</p> | **[v0.3.11](https://github.com/sipeed/Maixduino/releases/tag/v0.3.11)** | **2019-10-12** |  | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/Maixduino/core) | [![Go]](https://github.com/sipeed/Maixduino) |

[outline-dimension]: electronic/boards/sipeed-maixduino/hdk/outline-dimension.svg "MaixDuino Outline Dimension"
[outline-dimension.dwg]: electronic/boards/sipeed-maixduino/hdk/outline-dimension.dwg "DWG AutoDesk AutoCAD Release 13"
[outline-dimension.dxf]: electronic/boards/sipeed-maixduino/hdk/outline-dimension.dxf "AutoCAD Drawing Exchange Format, version 2000"

[outline-3d-model]: electronic/boards/sipeed-maixduino/hdk/outline-3d-model.png "MaixDuino 3D Model"
[outline-3d-model.stp]: electronic/boards/sipeed-maixduino/hdk/outline-3d-model.stp "ST-DEVELOPER v16.5"

[schematic-2832-20200813-kicad.pdf]: electronic/boards/sipeed-maixduino/hdk/schematic-2832-20200813-kicad.pdf "MaixDuino KiCad Schematic 2832 (printable)"
[assembly-drawing-2832-20200530-kicad.pdf]: electronic/boards/sipeed-maixduino/hdk/assembly-drawing-2832-20200530-kicad.pdf "MaixDuino KiCad Assembly Drawing 2832 (printable)"

[pin-assignment-table-2832-20200530.xlsx]: electronic/boards/sipeed-maixduino/hdk/pin-assignment-table-2832-20200530.xlsx "MaixDuino Excel Pin Assignment Table 2832 (working sheet)"
[pin-assignment-table-v4.30-20200428.xlsx]: electronic/boards/sipeed-maixduino/hdk/pin-assignment-table-v4.30-20200428.xlsx "MaixDuino Excel Pin Assignment Table v4.30 (working sheet)"
[datasheet-en-v1.0-20190316.pdf]: electronic/boards/sipeed-maixduino/hdk/datasheet-en-v1.0-20190316.pdf "MaixDuino Datasheet (EN), V1.0 (printable)"
