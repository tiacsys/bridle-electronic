# Maix-I M1/M1w – AI Core Module with Kendryte K210

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-26</strong></em></small>
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

<span style="width:256px;float:right;">[![module-m1w-top-bot]][module-m1w-top-bot]</span>
<span style="width:256px;float:right;">[![module-m1-top-bot]][module-m1-top-bot]</span>

[module-m1w-top-bot]: electronic/components/sipeed/Maix-I/module-m1w-top-bot.png "SiPEED Maix-I M1w"
[module-m1-top-bot]: electronic/components/sipeed/Maix-I/module-m1-top-bot.png "SiPEED Maix-I M1"

The **SiPEED Maix-I M1/M1w** module is a purpose-built SoM (System-on-Module)
designed for applications that combine AI (Artificial Intelligence)
technologies with the IoT (Internet of Things) infrastructure, or AIoT
(Artificial Intelligence of Things). Within the Maix-I module's compact
package is a [K210] RISC-V Microcontroller, one [TMI7003] 3-channel DC-DC
power management IC (PMIC), and one [GD25LQ128] for maximum of 16 MB on-module
Flash memory. The **SiPEED Maix-I M1w** module version additionally integrates
the Espressif [ESP8285], a specially designed [ESP8266] for wearable devices,
and thus also offers WiFi radio support. An integrated KPU (Neural Network
Processor) offers 0.25 TOPS @ 0.3 W, 400 MHz, and 0.5 TOPS when overclocked
to 800 MHz. A flexible FPIOA (Field Programmable IO Array) allows mapping up
to 255 functions to all 48 GPIOs on the chip. The Maix-I module also features
an integrated APU (Audio Processor), which supports up to 8 audio sources
with a sample rate of up to 192 kHz. Additional accelerators and peripherals
include AES Accelerator, SHA256 Accelerator, FFT Accelerator, OTP, OTP,
UART, WDT, IIC, SPI, I2S, and more.

The SiPEED Maix-I M1/M1w module is supplied in a compact 72 pin 1" square
(25mm x 25mm) package (full pin lead out), ideal for space-constrained IoT
applications.

[K210]: index.php?dir=electronic/components/canaan/K210 "Canaan Kendryte K210"
[ESP8266]: https://www.espressif.com/en/products/socs/esp8266 "Tensilica L106 32-bit RISC single-core, 160 kB RAM, IEEE 802.11 b/g/n WiFi radio"
[ESP8285]: https://www.espressif.com/en/news/espressif-announces-esp8285-wi-fi-chip-wearable-devices "Espressif Announces ESP8285 Wi-Fi Chip with up to 2 MB Flash for Wearable Devices"
[GD25LQ128]: https://www.gigadevice.com/flash-memory/gd25lq128c "128 Mbit SPI NOR Flash"
[TMI7003]: https://en.toll-semi.com/product/167.html "3-channels highly integrated power management IC"

| SiPEED Maix-I M1 (top & bottom) | SiPEED Maix-I M1w (top & bottom) | SiPEED Maix-I M1/M1w |
|::|::|::|
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1-top]][module-m1-top]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1w-top]][module-m1w-top]</div></div> | <div style="background-color:white;"><div style="width:100%;display:inline-block">[![module-m1w-top-erode]][module-m1w-top-erode]</div></div> |
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1-top-fccid]][module-m1-top-fccid]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1w-top-fccid]][module-m1w-top-fccid]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1-m1w-3d-model]][module-m1-m1w-3d-model]</div></div> |
| <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1-bot]][module-m1-bot]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1w-bot]][module-m1w-bot]</div></div> | <div style="background-color:white;"><div style="width:75%;display:inline-block">[![module-m1-m1w-footprint]][module-m1-m1w-footprint]</div></div> |

[module-m1-top]: electronic/components/sipeed/Maix-I/module-m1-top.png "SiPEED Maix-I M1 PCB V1.0 Assembly (top)"
[module-m1-top-fccid]: electronic/components/sipeed/Maix-I/module-m1-top-fccid.png "SiPEED Maix-I M1 V1.11 PCB Assembly (top) with new cage"
[module-m1-bot]: electronic/components/sipeed/Maix-I/module-m1-bot.png "SiPEED Maix-I M1 PCB Assembly (bottom)"

[module-m1w-top]: electronic/components/sipeed/Maix-I/module-m1w-top.png "SiPEED Maix-I M1w PCB V1.0 Assembly (top)"
[module-m1w-top-fccid]: electronic/components/sipeed/Maix-I/module-m1w-top-fccid.png "SiPEED Maix-I M1w V1.11 PCB Assembly (top) with FCCID label on cage"
[module-m1w-top-erode]: electronic/components/sipeed/Maix-I/module-m1w-top-erode.png "SiPEED Maix-I M1w PCB Assembly (top) w/o cage"
[module-m1w-bot]: electronic/components/sipeed/Maix-I/module-m1w-bot.png "SiPEED Maix-I M1w PCB Assembly (bottom)"

## Specifications

<span style="width:33%;float:right;background-color:white;">[![block-digram-som]][block-digram-som]</span>

[block-digram-som]: electronic/components/sipeed/Maix-I/block-digram-som.png "SiPEED Maix-I M1/M1w SoM Block Diagram"

* CPU: RISC-V Dual Core 64-bit, 400 Mhz adjustable
* FPU Specifications: IEEE754-2008 compliant high-performance pipelined FPU
* Debugging Support: High-speed UART and JTAG interface for debugging
* Neural Network Processor (KPU):
  * Supports the fixed-point model that the mainstream training framework
    trains according to specific restriction rules
  * Support for 1x1 and 3x3 convolution kernels
  * Support for any form of activation function
  * Supported neural network parameter size: 5 MiB to 5.9 MiB
* Audio Processor (APU):
  * Up to 8 channels of audio input data, (4 stereo channels)
  * Simultaneous scanning pre-processing and beamforming for sound sources
    in up to 16 directions
  * Supports one active voice stream output
  * 16-bit wide internal audio signal processing
  * Support for 12-bit, 16-bit, 24-bit, and 32-bit input data widths
  * Multi-channel direct raw signal output
  * Up to 192 kHz sample rate
  * Built-in FFT unit supports 512-point FFT of audio data
  * Uses system DMAC to store output data in system memory
* Static Random-Access Memory (SRAM):
  * 6MiB of on-chip general-purpose SRAM memory
  * 2MiB of on-chip AI SRAM memory
* Field Programmable IO Array (FPIOA/IOMUX): Allows mapping of
  255 internal functions to 48 free IOs on the chip
* Digital Video Port (DVP): Maximum frame size 640 x 480
* FFT Accelerator: The Hardware implementation
  of the Fast Fourier Transform (FFT)
* Software Development Kit Support:
  * FreeRtos
  * MicroPython Support 
* Machine vision: Machine vision based on convolutional neural network
* Machine hearing: High-performance microphone array processor
* Hardware Specifications:
  * Supply voltage: 5.0±0.2 V
  * Supply current: >300 mA
  * Temperature rise: <30 K
  * Operating temperature range: -30℃ to +85℃
  * Dimensions: 25mm x 25mm x 1mm
  * Weight: 8g

**FCC**: [2AS7P-SIPEED-M1W](https://fccid.io/2AS7P-SIPEED-M1W)
         (FRN: [0028444578](https://apps.fcc.gov/cores/searchDetail.do?frn=0028444578))

| SiPEED Maix-I M1 Pinout | SiPEED Maix-I M1w Pinout |
|::|::|
| <div style="background-color:white;">[![module-m1-pinout]][module-m1-pinout]</div> | <div style="background-color:white;">[![module-m1w-pinout]][module-m1w-pinout]</div> |

[module-m1w-pinout]: electronic/components/sipeed/Maix-I/module-m1w-pinout.png "SiPEED Maix-I M1w Pinout"
[module-m1-pinout]: electronic/components/sipeed/Maix-I/module-m1-pinout.png "SiPEED Maix-I M1 Pinout"

## References

* *HTML(2022-10-26)*: [Product Page]
  – *SiPEED Maix-I M1 – AI Core Module with Kendryte K210*
* *HTML(2022-10-26)*: [Developer Resources]
  – *Specification, Downloads, Datasheets, ...*
* *GIT(2022-10-26)*: [kflash.py]
 – *a Python-based Kendryte K210 UART ISP Utility* ([pypi kflash])
* *GIT(2022-10-26)*: [kflash_gui], last release was v1.8.1 on Jun 20, 2022
  – *cross platform GUI wrapper for [kflash.py]*

[Product Page]: https://sipeed.com/solution.html "Maix-I M1/M1w"
[Developer Resources]: https://wiki.sipeed.com/hardware/zh/maix/core_module.html "SiPEED AI Core Module Resources"
[kflash.py]: https://github.com/sipeed/kflash.py "SiPEED Kendryte K210 Flash utility on GitHub"
[pypi kflash]: https://pypi.org/project/kflash "SiPEED Kendryte K210 Flash utility on PyPi"
[kflash_gui]: https://github.com/sipeed/kflash_gui "SiPEED Kendryte K210 Flash GUI utility on GitHub"

| Name | Versions | Date | Mirror | Original | Storage |
|:-|::|::|::|::|::|
|  |  |  |  |  |  |
| <h3>HDK</h3> |  |  |  |  |  |
| <span style="width:96px;float:right;">[![module-m1-m1w-6032-wson8]][module-m1-m1w-6032-wson8]</span> **Maix-I M1/M1w DXF Module Outline** *(by Altium)* | **V1.11** | **2021-02-21** | [![Dm]][module-m1-m1w-6032-wson8.dxf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/M1w_6032_WSON8.DXF) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11) |
| **Maix-I M1/M1w DWG Module Outline** *(by VariCAD Viewer)* | **V1.11** | **2021-02-21** | [![Dm]][module-m1-m1w-6032-wson8.dwg] |  |  |
| <span style="width:96px;float:right;">[![module-m1-m1w-footprint]][module-m1-m1w-footprint]</span> **Maix-I M1/M1w DXF Carrier Footprint** *(by Altium)* | **V1.11** | **2020-09-23** | [![Dm]][module-m1-m1w-footprint.dxf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/M1%26M1W%20footprint.dxf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11) |
|  |  | 2020-04-28 |  | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/M1%26M1W%20footprint.dxf) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20M1W.rar) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13) |
| **Maix-I M1/M1w DWG Carrier Footprint** *(by VariCAD Viewer)* | **V1.11** | **2020-09-23** | [![Dm]][module-m1-m1w-footprint.dwg] |  |  |
| <span style="width:96px;float:right;">[![module-m1-m1w-3d-model]][module-m1-m1w-3d-model]</span> **Maix-I M1/M1w STEP Module 3D Model** *(by Altium)* | **V1.11** | **2020-08-05** | [![Dm]][module-m1-m1w-3d-model.stp] | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/3D_model) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20M1W.rar) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/3D_model) |
| <h4>Maix-I M1/M1w Symbol and Footprint</h4> |  |  |  |  |  |
| <em style="float:right;">EESchema-LIBRARY Version 2.3 (<code>.lib</code>) for <strong>KiCad</strong></em> |  | 2020-04-28 | [![Dm]][kicad/M1&M1W.lib] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/Kicad_lib/M1%26M1w.lib) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/Kicad_lib) |
| <em style="float:right;">Footprint Library (<code>.kicad_mod</code>) for <strong>KiCad</strong></em> |  | 2020-04-28 | [![Dm]][kicad/M1&M1W.kicad_mod] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/Kicad_lib/M1%26M1W.kicad_mod) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/Kicad_lib) |
| <em style="float:right;">Schematic Library Editor Binary File Version 5.0 (<code>.SchLib</code>) for <strong>Altium</strong></em> |  |  | [![Dm]][altium/M1&M1W.SchLib] | [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20M1W.rar) |  |
| <em style="float:right;">PCB 6.0 Binary Library File (<code>.PcbLib</code>) for <strong>Altium</strong></em> |  |  | [![Dm]][altium/M1&M1W.PcbLib] | [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20M1W.rar) |  |
| <em style="float:right;">OrCAD Windows Library (<code>.olb</code>) for <strong>OrCad</strong></em> |  | 2020-04-28 | [![Dm]][orcad/M1&M1W.PcbLib] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/M1%26M1W.olb) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13) |
| <h4>Maix-I M1 – AI Core Module</h4> |  |  |  |  |  |
| **Maix-I M1 PDF Schematic** *(by KiCad)* | **V1.11** | **2021-11-01** | [![Dm]][module-m1/schematic-v1.11-20211101-kicad.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/M1%20V1.11%28schematic%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11) |
| **Maix-I M1 PDF Schematic** *(by Altium)* |  | 2020-07-30 | [![Dm]][module-m1/schematic-v1.11-20200730-altium.pdf] | [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20M1.rar) |  |
| <h5>Documentations</h5> |  |  |  |  |  |
| **Maix-I M1 Datasheet** | **V1.12** | **2021-10-11** | [![Dm]][module-m1/datasheet-v1.12-20211011.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/Specifications/Sipeed%20M1%20Datasheet%20EN%20V1.12.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/Specifications) |
|  | V1.11 | 2020-07-30 | [![Dm]][module-m1/datasheet-v1.11-20200730.pdf] | [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0636%20Sipeed%20M1%20Datasheet%20V1.11.pdf) |  |
|  | V1.1 | 2019-03-06 | [![Dm]][module-m1/datasheet-v1.1-20190306.pdf] | [![Do]](https://download.kamami.pl/p578357-Sipeed-M1-Datasheet-V1.1.pdf) |  |
| *(published as Specification)* | V1.0 | 2018-11-09 | [![Dm]][module-m1/specification-v1.0-20181109.pdf] | [![Do]](https://myosuploads3.banggood.com/products/20190108/20190108035109SipeedMaix-1SpecificationsENV1.0201811091.pdf) |  |
| <h4>Maix-I M1w – AI Core Module with WiFi</h4> |  |  |  |  |  |
| **Maix-I M1w PDF Schematic** *(by KiCad)* | **V1.11** | **2021-11-01** | [![Dm]][module-m1w/schematic-v1.11-20211101-kicad.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11/M1w%20V1.11%28schematic%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/M1w%20V1.11) |
| **Maix-I M1w PDF Schematic** *(by Altium)* |  | 2019-12-02 | [![Dm]][module-m1w/schematic-v1.11-20191202-altium.pdf] | [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20M1W.rar) |  |
|  | 11.13 (prototype) | 2019-02-19 | [![Dm]][module-m1w/schematic-11.13-proto-20190219-altium.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/M1W_11.13%28Schematic%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13) |
| **Maix-I M1w PDF Assembly Drawing** *(by Altium)* | 11.13 (prototype) | 2019-02-15 | [![Dm]][module-m1w/assembly-drawing-11.13-proto-20190215-altium.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13/M1W_11.13%28Assembly%20drawing%29.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/History/M1%26M1W_11.13) |
| <h5>Documentations</h5> |  |  |  |  |  |
| **Maix-I M1w Datasheet** | **V1.12** | **2021-10-11** | [![Dm]][module-m1w/datasheet-v1.12-20211011.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/HDK/Sipeed-M1%26M1W/Specifications/Sipeed%20M1W%20Datasheet%20EN%20V1.12.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/HDK/Sipeed-M1%26M1W/Specifications) |
|  | V1.11 | 2019-11-26 | [![Dm]][module-m1w/datasheet-v1.11-20191126.pdf] | [![Do]](https://download.kamami.pl/p578358-Sipeed-M1W-Datasheet-V1.11.pdf) [![Do]](https://github.com/May-DFRobot/DFRobot/raw/master/DFR0637%20Sipeed-M1W-Datasheet-V1.11.pdf) |  |
| *(published as User Manual)* | V1.0 | 2018-11-09 | [![Dm]][module-m1w/user-manual-v1.0-20181109.pdf] | [![Do]](https://fccid.io/2AS7P-SIPEED-M1W/User-Manual/User-Manual-4296604.pdf) |  |

[module-m1-m1w-6032-wson8]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-6032-wson8.svg "Maix-I M1/M1w Module Outline"
[module-m1-m1w-6032-wson8.dwg]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-6032-wson8.dwg "DWG AutoDesk AutoCAD Release 13"
[module-m1-m1w-6032-wson8.dxf]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-6032-wson8.dxf "AutoCAD Drawing Exchange Format"

[module-m1-m1w-footprint]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-footprint.svg "Maix-I M1/M1w Carrier Footprint"
[module-m1-m1w-footprint.dwg]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-footprint.dwg "DWG AutoDesk AutoCAD Release 13"
[module-m1-m1w-footprint.dxf]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-footprint.dxf "AutoCAD Drawing Exchange Format"

[module-m1-m1w-3d-model]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-3d-model.png "Maix-I M1/M1w Module 3D Model"
[module-m1-m1w-3d-model.stp]: electronic/components/sipeed/Maix-I/hdk/module-m1-m1w-3d-model.stp "ST-DEVELOPER v16.5"

[kicad/M1&M1W.lib]: electronic/components/sipeed/Maix-I/hdk/kicad/M1&M1W.lib "KiCad EESchema-LIBRARY Version 2.3 with M1&M1W (2020-04-28)"
[kicad/M1&M1W.kicad_mod]: electronic/components/sipeed/Maix-I/hdk/kicad/M1&M1W.kicad_mod "KiCad Footprint Library with M1&M1W (2020-04-28)"

[altium/M1&M1W.SchLib]: electronic/components/sipeed/Maix-I/hdk/altium/M1&M1W.SchLib "Altium Schematic Library"
[altium/M1&M1W.PcbLib]: electronic/components/sipeed/Maix-I/hdk/altium/M1&M1W.PcbLib "Altium PCB Library"

[orcad/M1&M1W.PcbLib]: electronic/components/sipeed/Maix-I/hdk/orcad/M1&M1W.olb "OrCAD Symbol Library (2020-04-28)"

[module-m1/schematic-v1.11-20211101-kicad.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/schematic-v1.11-20211101-kicad.pdf "Maix-I M1 KiCad Schematic V1.11 (printable)"
[module-m1/schematic-v1.11-20200730-altium.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/schematic-v1.11-20200730-altium.pdf "Maix-I M1 Altium Schematic V1.11 (printable)"

[module-m1/datasheet-v1.12-20211011.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/datasheet-v1.12-20211011.pdf "Maix-I M1 Datasheet V1.12"
[module-m1/datasheet-v1.11-20200730.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/datasheet-v1.11-20200730.pdf "Maix-I M1 Datasheet V1.11"
[module-m1/datasheet-v1.1-20190306.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/datasheet-v1.1-20190306.pdf "Maix-I M1 Datasheet V1.1"
[module-m1/specification-v1.0-20181109.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1/specification-v1.0-20181109.pdf "Maix-I M1 Datasheet V1.0"

[module-m1w/schematic-v1.11-20211101-kicad.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/schematic-v1.11-20211101-kicad.pdf "Maix-I M1w KiCad Schematic V1.11 (printable)"
[module-m1w/schematic-v1.11-20191202-altium.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/schematic-v1.11-20191202-altium.pdf "Maix-I M1w Altium Schematic V1.11 (printable)"
[module-m1w/schematic-11.13-proto-20190219-altium.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/schematic-11.13-proto-20190219-altium.pdf "Maix-I M1w Altium Schematic 11.13 prototype (printable)"
[module-m1w/assembly-drawing-11.13-proto-20190215-altium.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/assembly-drawing-11.13-proto-20190215-altium.pdf

[module-m1w/datasheet-v1.12-20211011.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/datasheet-v1.12-20211011.pdf "Maix-I M1w Datasheet V1.12"
[module-m1w/datasheet-v1.11-20191126.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/datasheet-v1.11-20191126.pdf "Maix-I M1w Datasheet V1.11"
[module-m1w/user-manual-v1.0-20181109.pdf]: electronic/components/sipeed/Maix-I/hdk/module-m1w/user-manual-v1.0-20181109.pdf "Maix-I M1w Datasheet V1.0"
