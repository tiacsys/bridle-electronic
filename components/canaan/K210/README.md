# Kendryte K210 – SoC for machine vision and machine hearing

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2022-10-24</strong></em></small>
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

<span style="width:256px;float:right;">[![chip-top-bot]][chip-top-bot]</span>

[chip-top-bot]: electronic/components/canaan/K210/chip-top-bot.png "Canaan Kendryte K210"

Kendryte K210 is a system-on-chip (SoC) that integrates machine vision and
machine hearing capabilities. It uses TSMC's ultra-low power 28-nanometer
advanced manufacturing process, with RISC-V dual-core 64-bit processors, and
has good power consumption performance and stability and reliability. Kendryte
K210 is located in the SoC of the AI and IoT market, and it is also a very
convenient MCU.

The Chinese meaning of Kendryte is Kanzhi(堪智), and Kanzhi is derived from
Geophysical Prospecting, means researching intelligence. The main application
field of this chip is the Internet of Things field, and it is developed in the
field of Internet of Things, so it is Prospecting; this chip mainly provides
Artificial intelligence solutions are explored in the field of artificial
intelligence, so they are intellectual exploration.

## Specifications

<span style="width:33%;float:right;background-color:white;">[![block-digram-soc]][block-digram-soc]</span>

[block-digram-soc]: electronic/components/canaan/K210/block-digram-soc.svg "Kendryte K210 SoC Block Diagram"

1. **Performance**:
   * *Processor*: RISC-V Dual Core 64-bit IMAFDC (RV64GC) at up to 400 MHz,
     with *Floating Point Unit* (FPU) and 32/32 KiB I-/D-Cache on each core
   * *Hardware Accelerator*: one *Knowledge Processing Unit* (KPU)
     for high performance *Convolutional Neural Network* (CNN), one
     *Audio Processing Unit* (APU) for machine hearing and one
     *Fast Fourier Transform* (FFT) Acceleration Unit for powerful
     algorithm development of machine vision and hearing
   * *Image Recognition*: QVGA@60fps / VGA@30fps on *Digital Video Port* (DVP)
   * *Voice Recognition*: Microphone arrays
   * *Unique programmable IO array*: *Field Programmable IO Array* (FPIOA)
     allows users to map 255 internal functions to 48 free IOs on the chip
1. **Safety**:
   * Advanced encryption hardware accelerator（AES)
   * Read - only memory（OTP）SHA256
   * Firmware encryption
1. **Power Consumption**:
   * Scenario power consumption < 1 W
   * Power consumption of Chip  < 300 mW
1. **Limits**:
   * *Temperature range*: -40°C to 125°C
   * *Dual voltage IO*: 3.3 V / 1.8 V
1. **Scalability**:
   * *Operating system*: FreeRTOS
   * *Network model*: TinyYOLOv2 (after pruned)
   * *Deep learning framework*: TensorFlow, Keras, Darknet
   * *Peripherals*: FPIOA, UART, GPIO, SPI etc.

The K210 includes two 64-bit RISC-V CPU cores, each with a built-in independent
FPU. The K210 features a FFT Accelerator for high performance complex FFT
calculations. As a result, for most machine learning algorithms, the K210 has
high-performance processing power. The K210 embeds AES and SHA256 algorithm
accelerators to provide users with basic security features. The K210 features
high-performance, low-power SRAM and powerful DMA for superior data throughput.
The K210 has a wide range of peripheral units: DVP, JTAG, OTP, FPIOA, GPIO,
UART, SPI, RTC, I2S, I2C, WDT, Timer and PWM, for a large number of application
scenarios.

### FPU Specification

* **IEEE754-2008** compliant high-performance pipelined FPU.
* F extension: single-precision floating point instructions.
* D extension: double-precision floating point instructions.
* Hardware single-precision and double-precision division.
* Hardware single-precision and double-precision square roots.
* Core 0 and Core 1 each have a separate FPU, and both cores are capable
  of high performance hardware floating point calculations.

### FFT Accelerator

The FFT accelerator is a hardware implementation of the
Fast Fourier Transform (FFT):

* 64-point, 128-point, 256-point or 512-point length.
* FFT and IFFT operation modes.
* 32-bit or 64-bit input data width.
* Supports pure-real, pure-imaginary or complex input data.
* DMA transfer support.

### Audio Processor (APU)

The APU pre-processing module is responsible for the pre-processing of voice
direction and voice data output. The functional characteristics of the APU
preprocessing module are:

* Up to 8 channels of audio input data, ie 4 stereo channels.
* Simultaneous scanning pre-processing and beamforming for sound sources
  in up to 16 directions.
* Supports one active voice stream output.
* 16-bit wide internal audio signal processing.
* Support for 12-bit, 16-bit, 24-bit, and 32-bit input data widths.
* Multi-channel direct raw signal output.
* Up to 192kHz sample rate.
* Built-in FFT unit supports 512-point FFT of audio data.
* Uses system DMAC to store output data in system memory.

### Neural Network (Knowledge) Processor (KPU)

The KPU is a general-purpose neural network processor with built-in convolution,
batch normalization, activation, and pooling operations. It can detect faces or
objects in real time. The specific characteristics are as follows:

* Supports the fixed-point model that the mainstream training framework
  trains according to specific restriction rules.
* There is no direct limit on the number of network layers, and each layer
  of convolutional neural network parameters can be configured separately,
  including the number of input and output channels, and the input and
  output line width and column height.
* Support for 1x1 and 3x3 convolution kernels.
* Support for any form of activation function.
* The maximum supported neural network parameter size for real-time work
  is 5 MiB to 5.9 MiB.
* The maximum supported network parameter size when working in non-real
  time is (flash size - software size).

| one diagram to understand how KPU works |
|::|
| <div style="background-color:white;padding-top:100px;padding-bottom:50px;">[![workflow-digram-kpu]][workflow-digram-kpu]</div> |
|  |
| **internal structure of the KPU** |
| <div style="background-color:white;padding-top:100px;padding-bottom:50px;">[![block-digram-kpu]][block-digram-kpu]</div> |

[workflow-digram-kpu]: electronic/components/canaan/K210/workflow-digram-kpu.svg "Kendryte K210 KPU Workflow Diagram"
[block-digram-kpu]: electronic/components/canaan/K210/block-digram-kpu.svg "Kendryte K210 KPU Block Diagram"

## References

* *HTML(2022-10-24)*: [Product Page]
  – *Canaan Kendryte K210 Product Center*
* *HTML(2022-10-24)*: [Developer Resources]
  – *SDK, HDK, Documentation, Toolchain, ...*

[Product Page]: https://canaan.io/product/kendryteai "Kendryte K210"
[Developer Resources]: https://canaan.io/developer "Canaan Developer Resources"

| Name | Versions | Date | Mirror | Original | Storage |
|:-|::|::|::|::|::|
|  |  |  |  |  |  |
| <span style="width:96px;float:right;">[![kd233-top]][kd233-top]</span> <h3>HDK</h3> |  |  |  |  |  |
| **Kendryte KD233 Board Schematic V02** | **V0.2.0** | **2018-11-27** | [![Dm]][Kendryte_test_board_V0_2.pdf] | [![Do]](https://canaan.io/wp-content/uploads/2020/02/Kendryte_test_board_V0_2.pdf) | |
| **Kendryte KD233 Board Schematic V01** | V0.1.0 | 2018-10-10 | [![Dm]][Kendryte_test_board_V0_1.pdf] | [![Do]](https://canaan.io/wp-content/uploads/2020/02/Kendryte_test_board_V0_1-1.pdf) | |
| <h4>K210 Model Demo on KD233 Board</h4> |  |  |  |  |  |
| **Kendryte K210 Model Download Guide** | **V0.4.1** | **2019-06-05** | [![Dm]][Model_download_guide.pdf] | [![Do]](https://canaan.io/wp-content/uploads/2020/04/Model_download_guide.pdf) |  |
| **Kendryte K210 Face Detection Demo** | **V0.1.0** | **2018-10-11** | [![Cm]][demo.kfpkg_.zip] | [![Co]](https://canaan.io/wp-content/uploads/2020/04/demo.kfpkg_.zip) |  |
| <h4>Paddle Pi K210 Demo Board</h4> |  |  |  |  | [![Go]](https://github.com/kendryte/PaddlePi) |
| <span style="width:64px;float:right;">[![paddlepi-top-v1.3]][paddlepi-top-v1.3]</span> <span style="width:64px;float:right;">[![paddlepi-bot-v1.3]][paddlepi-bot-v1.3]</span> | **V1.3** |  |  |  | [![Go]](https://github.com/kendryte/PaddlePi/tree/master/documents/PaddlePi_V1.3) |
| <span style="width:64px;float:right;">[![paddlepi-top-v1.2]][paddlepi-top-v1.2]</span> | V1.2 |  |  |  | [![Go]](https://github.com/kendryte/PaddlePi/tree/master/documents/PaddlePi_V1.2) |
|  | V1.0 |  |  |  | [![Go]](https://github.com/kendryte/PaddlePi/tree/master/documents/PaddlePi_V1.0) |
| <h4>Documentations</h4> |  |  |  |  |  |
| **Kendryte K210 Datasheet** | **[V0.1.5][kendryte-doc-datasheet-v0.1.5-20181011]** | **2018-10-11** | [![Dm]][kendryte_datasheet_20181011163248_en.pdf] | [![Do]](https://cdn.hackaday.io/files/1654127076987008/kendryte_datasheet_20181011163248_en.pdf) | [![Go]](https://github.com/kendryte/kendryte-doc-datasheet) |
| **Kendryte K210 – KPU Workflow Giagram** |  | **2019-01-29** | [![Dm]][kendryte_kpu_workflow_diagram_20190129_cn_en.pdf] | [![Do]](https://dl.sipeed.com/fileList/MAIX/SDK/Document/KPU%20diagram.pdf) | [![Fo]](https://dl.sipeed.com/shareURL/MAIX/SDK/Document) |
|  |  |  |  |  |  |
| <h3>SDK</h3> |  |  |  |  |  |
| **Kendryte Standalone SDK** | **[V0.5.6][kendryte-standalone-sdk-v0.5.6-20190517]** | **2019-05-17** | [![Cm]][kendryte-standalone-sdk-0.5.6.zip] | [![Co]](https://github.com/kendryte/kendryte-standalone-sdk/archive/refs/tags/V0.5.6.zip) [![Co]](https://canaan-creative.com/wp-content/uploads/2020/03/kendryte-standalone-sdk-0.5.6.zip) | [![Go]](https://github.com/kendryte/kendryte-standalone-sdk) |
| **Kendryte FreeRTOS SDK** | **[V0.7.0][kendryte-freertos-sdk-v0.7.0-20181221]** | **2018-12-20** | [![Cm]][kendryte-freertos-sdk-0.7.0.zip] | [![Co]](https://github.com/kendryte/kendryte-freertos-sdk/archive/refs/tags/v0.7.0.zip) [![Co]](https://canaan.io/wp-content/uploads/2020/02/kendryte-freertos-sdk-0.7.0-1.zip) | [![Go]](https://github.com/kendryte/kendryte-freertos-sdk) |
| <h4>Documentations</h4> |  |  |  |  |  |
| **Kendryte Standalone SDK Programming Guide** | **[V0.3.0][kendryte-doc-standalone-programming-guide-v0.3.0-20190311]** | **2019-03-26** | [![Dm]][kendryte_standalone_programming_guide_20190311144158_en.pdf] | [![Do]](https://canaan.io/wp-content/uploads/2020/02/kendryte_standalone_programming_guide_20190311144158_en.pdf) | [![Go]](https://github.com/kendryte/kendryte-doc-standalone-programming-guide) |
| **Kendryte FreeRTOS SDK Programming Guide** | **[V0.1.0][kendryte-doc-freertos-programming-guide-v0.1.0-20190311]** | **2019-03-26** | [![Dm]][kendryte_freertos_programming_guide_20190311143226_en.pdf] | [![Do]](https://canaan.io/wp-content/uploads/2020/02/kendryte_freertos_programming_guide_20190311143226_en-1.pdf) | [![Go]](https://github.com/kendryte/kendryte-doc-freertos-programming-guide) |
|  |  |  |  |  |  |
| <h3>Toolchain</h3> |  |  |  |  |  |
| <h4>K210 RISC-V 64-bit</h4> |  |  |  |  | [![Go]](https://github.com/kendryte/kendryte-gnu-toolchain) |
| **kendryte-toolchain-win-amd64** | **[V8.2.0][kendryte-toolchain-v8.2.0-20190409]** | **2020-09-03** | [![Cm]][kendryte-toolchain-win-amd64-8.2.0-20190409.zip] | [![Co]](https://github.com/kendryte/kendryte-gnu-toolchain/releases/download/v8.2.0-20190409/kendryte-toolchain-win-amd64-8.2.0-20190409.zip) [![Co]](https://canaan.io/wp-content/uploads/2020/09/kendryte-toolchain-win-amd64-8.2.0-20190409.zip) |  |
| **kendryte-toolchain-win-i386** | **[V8.2.0][kendryte-toolchain-v8.2.0-20190409]** | **2020-09-03** | [![Cm]][kendryte-toolchain-win-i386-8.2.0-20190409.zip] | [![Co]](https://github.com/kendryte/kendryte-gnu-toolchain/releases/download/v8.2.0-20190409/kendryte-toolchain-win-i386-8.2.0-20190409.zip) |  |
| **kendryte-toolchain-ubuntu-amd64** | **[V8.2.0][kendryte-toolchain-v8.2.0-20190409]** | **2020-09-03** | [![Cm]][kendryte-toolchain-ubuntu-amd64-8.2.0-20190409.tar.xz] | [![Co]](https://github.com/kendryte/kendryte-gnu-toolchain/releases/download/v8.2.0-20190409/kendryte-toolchain-ubuntu-amd64-8.2.0-20190409.tar.xz) |  |
| **kendryte-toolchain-osx-mojave** | **[V8.2.0][kendryte-toolchain-v8.2.0-20190409]** | **2020-09-03** | [![Cm]][kendryte-toolchain-osx-mojave-8.2.0-20190409.tar.xz] | [![Co]](https://github.com/kendryte/kendryte-gnu-toolchain/releases/download/v8.2.0-20190409/kendryte-toolchain-osx-mojave-8.2.0-20190409.tar.xz) |  |
| **kendryte-toolchain-osx-darwin-m1** | **[V8.2.0][kendryte-toolchain-v8.2.0-20190409]** | **2020-09-03** | [![Cm]][kendryte-toolchain-osx-darwin-m1-8.2.0-20210717.tar.xz] | [![Co]](https://github.com/kendryte/kendryte-gnu-toolchain/releases/download/v8.2.0-20190409/kendryte-toolchain-osx-darwin-m1-8.2.0-20210717.tar.xz) |  |
| <h4>K210 MicroPython & OpenMV</h4> |  |  |  |  | [![Go]](https://github.com/kendryte/K210-Micropython-OpenMV) |
| **xpack-riscv-none-embed-gcc-8.3.0-1.9-win32-x64** | **[V8.3.0-1.9][xpack-riscv-none-embed-gcc-8.3.0-1.9-20210402]** | **2021-04-02** | [![Cm]][xpack-riscv-none-embed-gcc-8.3.0-1.9-win32-x64.zip] | [![Co]](https://canaan.io/wp-content/uploads/2021/04/3.zip) |  |
| **xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x64** | **[V8.3.0-1.9][xpack-riscv-none-embed-gcc-8.3.0-1.9-20210402]** | **2021-04-02** | [![Cm]][xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x64.tar.gz] | [![Co]](https://canaan.io/wp-content/uploads/2021/04/2.tar.gz) |  |
| **xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x32** | **[V8.3.0-1.9][xpack-riscv-none-embed-gcc-8.3.0-1.9-20210402]** | **2021-04-02** | [![Cm]][xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x32.tar.gz] | [![Co]](https://canaan.io/wp-content/uploads/2021/04/1.tar.gz) |  |
| *(based on **xPack GNU RISC-V Embedded GCC**:*<br/>*use hard-float sqrt instead of soft-float one)* | [V8.3.0-1.2][riscv-none-embed-gcc-xpack-8.3.0-1.2-20200703] | 2020-07-03 | **DIFF**: [![Dm]][xpack-riscv-none-embed-gcc-8.3.0-1.2-to-1.9.diff] | | [![Go]](https://github.com/xpack-dev-tools/riscv-none-embed-gcc-xpack) |
| <h5>xPack GNU RISC-V Embedded GCC Changes</h5> | V8.3.0<br/>1.2 to 1.9 | 2020-09-25 |  |  |  |
| <h6 style="text-align:center;">[bj-wanghz/riscv-newlib][bj-wanghz/riscv-newlib/sifive-master-xpack-canaan]</h6> |  |  |  |  |  |
| <em style="float:right;">sqrt needs to be conditional on the existance of FP registers</em> | **78aa4f9** | 2020-09-25 |  |  | [![Go]](https://github.com/bj-wanghz/riscv-newlib/commit/78aa4f9) |
| <em style="float:right;">Use hard-float sqrt instead of soft-float one</em> | **82cf035** | 2020-09-22 |  |  | [![Go]](https://github.com/bj-wanghz/riscv-newlib/commit/82cf035) |
| <h6 style="text-align:center;">[xpack-dev-tools/riscv-gcc][xpack-dev-tools/riscv-gcc/sifive-gcc-8.3.0-xpack]</h6> |  |  |  |  |  |
| <em style="float:right;">add support for riscv-none-embed-*</em> | **e5ac1b5** | 2019-10-30 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-gcc/commit/e5ac1b5) |
| <h6 style="text-align:center;">[xpack-dev-tools/riscv-binutils-gdb][xpack-dev-tools/riscv-binutils-gdb/sifive-binutils-2.32-xpack]</h6> |  |  |  |  |  |
| <em style="float:right;">Merge branch 'sifive-binutils-2.32' into sifive-binutils-2.32-xpack</em> | **4b773a4** | 2019-10-30 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/4b773a4) |
| <em style="float:right;">Merge commit '03d23d5' into sifive-binutils-2.32</em> | **afbdd26** | 2019-10-30 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/afbdd26) |
| <em style="float:right;">add support for riscv-none-embed-*</em> | **82b51c7** | 2019-04-16 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/82b51c7) |
| <em style="float:right;">Merge pull request #3 from sifive/sifive-7-integration</em> | **1642671** | 2019-04-05 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/1642671) |
| <em style="float:right;">RISC-V: Compress 3-operand beq/bne against x0.</em> | **162c2e5** | 2019-04-04 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/162c2e5) |
| <em style="float:right;">Add support for SiFive CLIC CSRs.</em> | **8020f18** | 2019-02-22 |  |  | [![Go]](https://github.com/xpack-dev-tools/riscv-binutils-gdb/commit/8020f18) |
| <h5>Documentations</h5> |  |  |  |  |  |
| **K210-MicroPython & OpenMV User Manual** | **V1.1.0** | **2021-04-20** | [![Dm]][k210_micropython_openmv_user_manual_20210420_en.pdf] | [![Do]](https://github.com/kendryte/K210-Micropython-OpenMV/raw/master/doc/K210-MicroPython%26OpenMV%20Manual%20v1.1-en(20210420).pdf) | [![Go]](https://github.com/kendryte/K210-Micropython-OpenMV/tree/master/doc) |
| **RT-Thread: Getting Started of QEMU (Windows)** | **[V4.1.1][rt-thread-v4.1.1-20220822]** | **2022-10-24** | [![Dm]][RT-Thread_Getting-Started-of-QEMU_Windows_221024.pdf] | [![Wo]](https://www.rt-thread.io/document/site/documentation/quick_start_qemu/quick_start_qemu) | [![Go]](https://github.com/RT-Thread/rt-thread/blob/master/documentation/quick-start/quick_start_qemu/quick_start_qemu.md) |
| **RT-Thread: Getting Started of QEMU (Ubuntu)** | **[V4.1.1][rt-thread-v4.1.1-20220822]** | **2022-10-24** | [![Dm]][RT-Thread_Getting-Started-of-QEMU_Ubuntu_221024.pdf] | [![Wo]](https://www.rt-thread.io/document/site/documentation/quick_start_qemu/quick_start_qemu_linux) | [![Go]](https://github.com/RT-Thread/rt-thread/blob/master/documentation/quick-start/quick_start_qemu/quick_start_qemu_linux.md) |
| <h4>OpenOCD for Kendryte RISC-V</h4> |  |  |  |  | [![Go]](https://github.com/kendryte/openocd-kendryte) |
| *Binary Dependencies für win32* |  |  | [![Cm]][WindowsTools.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.3/WindowsTools.zip) [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.2/WindowsTools.zip) [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.1/WindowsTools.zip) |  |
| **Kendryte OpenOCD for win32** | **[V0.2.3][kendryte-openocd-v0.2.3-20190221]** | **2019-02-21** | [![Cm]][kendryte-openocd-0.2.3-win32.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.3/kendryte-openocd-0.2.3-win32.zip) |  |
| **Kendryte OpenOCD for Ubuntu x86_64** | **[V0.2.3][kendryte-openocd-v0.2.3-20190221]** | **2019-02-21** | [![Cm]][kendryte-openocd-0.2.3-ubuntu64.tar.gz] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.3/kendryte-openocd-0.2.3-ubuntu64.tar.gz) |  |
| **Kendryte OpenOCD for win32** | [V0.2.2][kendryte-openocd-v0.2.2-20190117] | 2019-01-17 | [![Cm]][kendryte-openocd-0.2.2-win32.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.2/kendryte-openocd-0.2.2-win32.zip) |  |
| **Kendryte OpenOCD for Ubuntu x86_64** | [V0.2.2][kendryte-openocd-v0.2.2-20190117] | 2019-01-17 | [![Cm]][kendryte-openocd-0.2.2-ubuntu64.tar.gz] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.2/kendryte-openocd-0.2.2-ubuntu64.tar.gz) |  |
| **Kendryte OpenOCD for MacOS** | **[V0.2.2][kendryte-openocd-v0.2.2-20190117]** | **2019-01-17** | [![Cm]][kendryte-openocd-0.2.2-macos.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.2/kendryte-openocd-0.2.2-macos.zip) |  |
| **Kendryte OpenOCD for win32** | [V0.2.1][kendryte-openocd-v0.2.1-20190109] | 2019-01-09 | [![Cm]][kendryte-openocd-0.2.1-win32.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.1/kendryte-openocd-0.2.1-win32.zip) |  |
| **Kendryte OpenOCD for Ubuntu x86_64** | [V0.2.1][kendryte-openocd-v0.2.1-20190109] | 2019-01-09 | [![Cm]][kendryte-openocd-0.2.1-ubuntu64.tar.gz] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.1/kendryte-openocd-0.2.1-ubuntu64.tar.gz) |  |
| **Kendryte OpenOCD for MacOS** | [V0.2.1][kendryte-openocd-v0.2.1-20190109] | 2019-01-09 | [![Cm]][kendryte-openocd-0.2.1-macos.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/v0.2.1/kendryte-openocd-0.2.1-macos.zip) |  |
| **Kendryte OpenOCD for win32** | [V0.1.3][kendryte-openocd-v0.1.3-20180913] | 2018-09-13 | [![Cm]][kendryte-openocd-0.1.3-win32.zip] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/0.1.3/kendryte-openocd-0.1.3-win32.zip) [![Co]](https://canaan.io/wp-content/uploads/2020/04/kendryte-openocd-0.1.3-win32.zip) |  |
| **Kendryte OpenOCD for Ubuntu x86_64** | [V0.1.3][kendryte-openocd-v0.1.3-20180913] | 2018-09-13 | [![Cm]][kendryte-openocd-0.1.3-ubuntu64.tar.gz] | [![Co]](https://github.com/kendryte/openocd-kendryte/releases/download/0.1.3/kendryte-openocd-0.1.3-ubuntu64.tar.gz) [![Co]](https://canaan.io/wp-content/uploads/2020/04/kendryte-openocd-0.1.3-ubuntu64.tar.gz) |  |
|  *(TAP Declaration IdCode: `0x04e4796b`)* |  |  |  |  |  |
| <h4>CMake</h4> |  |  |  |  | [![Go]](https://github.com/Kitware/CMake) |
| **cmake-win32-x86** | [V3.14.4][cmake-3.14.4-20190514] |  | [![Cm]][cmake-3.14.4-win32-x86.zip] | [![Co]](https://github.com/Kitware/CMake/releases/download/v3.14.4/cmake-3.14.4-win32-x86.zip) | |
| **cmake-win64-x64** | [V3.14.4][cmake-3.14.4-20190514] | 2020-09-03 | [![Cm]][cmake-3.14.4-win64-x64.zip] | [![Co]](https://github.com/Kitware/CMake/releases/download/v3.14.4/cmake-3.14.4-win64-x64.zip) [![Co]](https://canaan.io/wp-content/uploads/2020/09/cmake-3.14.4-win64-x64.zip) |  |
| **cmake-linux-x86_64** | [V3.14.4][cmake-3.14.4-20190514] |  | [![Cm]][cmake-3.14.4-Linux-x86_64.tar.gz] | [![Co]](https://github.com/Kitware/CMake/releases/download/v3.14.4/cmake-3.14.4-Linux-x86_64.tar.gz) | |
| **cmake-darwin-x86_64** | [V3.14.4][cmake-3.14.4-20190514] |  | [![Cm]][cmake-3.14.4-Darwin-x86_64.tar.gz] | [![Co]](https://github.com/Kitware/CMake/releases/download/v3.14.4/cmake-3.14.4-Darwin-x86_64.tar.gz) | |
|  |  |  |  |  |  |
| <h3>CanMV</h3> |  |  |  |  |  |
| **CanMV IDE** | **V2.9.2** | **2022-09-28** | [![Cm]][canmv-ide-windows-v2.9.2-30-g65f7289-20220928.zip] | [![Co]](https://canaan.io/wp-content/uploads/2022/09/canmv-ide-windows-v2.9.2-30-g65f7289-20220928.zip) |  |
|  |  |  |  |  |  |
| <h3>Kendryte IDE</h3> |  |  |  |  | [![Go]](https://github.com/kendryte/kendryte-ide) |
| **Visual Studio Code based IDE** | alpha/beta | 2019 |  | [![Co]](http://kendryte-ide.s3-website.cn-northwest-1.amazonaws.com.cn/) |  |

[kd233-top]: electronic/components/canaan/K210/hdk/Kendryte-KD223.jpg "Kendryte KD233 Board Top View"
[Kendryte_test_board_V0_2.pdf]: electronic/components/canaan/K210/hdk/Kendryte_test_board_V0_2.pdf "Kendryte KD233 Board Schematic V02"
[Kendryte_test_board_V0_1.pdf]: electronic/components/canaan/K210/hdk/Kendryte_test_board_V0_1.pdf "Kendryte KD233 Board Schematic V01"

[Model_download_guide.pdf]: electronic/components/canaan/K210/hdk/model/Model_download_guide.pdf "Kendryte K210 Model Download Guide"
[demo.kfpkg_.zip]: electronic/components/canaan/K210/hdk/model/demo.kfpkg_.zip "Kendryte K210 Face Detection Demo"

[paddlepi-top-v1.3]: electronic/components/canaan/K210/hdk/paddlepi/v1.3-pcb-assembly-top-pcba.jpg "Paddle Pi K210 Demo Board V1.3 Top View"
[paddlepi-bot-v1.3]: electronic/components/canaan/K210/hdk/paddlepi/v1.3-pcb-assembly-bot-pcba.jpg "Paddle Pi K210 Demo Board V1.3 Bottom View"
[paddlepi-top-v1.2]: electronic/components/canaan/K210/hdk/paddlepi/v1.2-pcb-assembly-top.jpg "Paddle Pi K210 Demo Board V1.2 Top View"

[kendryte-doc-datasheet-v0.1.5-20181011]: https://github.com/kendryte/kendryte-doc-datasheet/tree/8e9b414 "Kendryte K210 Datasheet v0.1.5 (2018-10-11)"
[kendryte_datasheet_20181011163248_en.pdf]: electronic/components/canaan/K210/docs/kendryte_datasheet_20181011163248_en.pdf "Kendryte K210 Datasheet"
[kendryte_kpu_workflow_diagram_20190129_cn_en.pdf]: electronic/components/canaan/K210/docs/kendryte_kpu_workflow_diagram_20190129_cn_en.pdf "Kendryte K210 – One Diagram Understand How KPU Work"

[kendryte-standalone-sdk-v0.5.6-20190517]: https://github.com/kendryte/kendryte-standalone-sdk/releases/tag/V0.5.6 "Kendryte Standalone SDK v0.5.6 (2019-05-17)"
[kendryte-standalone-sdk-0.5.6.zip]: electronic/components/canaan/K210/sdk/kendryte-standalone-sdk-0.5.6.zip "Kendryte Standalone SDK"
[kendryte-freertos-sdk-v0.7.0-20181221]: https://github.com/kendryte/kendryte-freertos-sdk/releases/tag/v0.7.0 "Kendryte FreeRTOS SDK v0.7.0 (2018-12-21)"
[kendryte-freertos-sdk-0.7.0.zip]: electronic/components/canaan/K210/sdk/kendryte-freertos-sdk-0.7.0.zip "Kendryte FreeRTOS SDK"

[kendryte-doc-standalone-programming-guide-v0.3.0-20190311]: https://github.com/kendryte/kendryte-doc-standalone-programming-guide/tree/143df47 "Kendryte Standalone SDK Programming Guide v0.3.0 (2019-03-11)"
[kendryte_standalone_programming_guide_20190311144158_en.pdf]: electronic/components/canaan/K210/docs/kendryte_standalone_programming_guide_20190311144158_en.pdf "Kendryte Standalone SDK Programming Guide"
[kendryte-doc-freertos-programming-guide-v0.1.0-20190311]: https://github.com/kendryte/kendryte-doc-freertos-programming-guide/tree/74195b1 "Kendryte FreeRTOS SDK Programming Guide v0.1.0 (2019-03-11)"
[kendryte_freertos_programming_guide_20190311143226_en.pdf]: electronic/components/canaan/K210/docs/kendryte_freertos_programming_guide_20190311143226_en.pdf "Kendryte FreeRTOS SDK Programming Guide"

[kendryte-toolchain-v8.2.0-20190409]: https://github.com/kendryte/kendryte-gnu-toolchain/releases/tag/v8.2.0-20190409 "Kendryte GNU Toolchain v8.2.0 (2019-04-09)"
[kendryte-toolchain-win-amd64-8.2.0-20190409.zip]: electronic/components/canaan/K210/toolchain/kendryte-toolchain-win-amd64-8.2.0-20190409.zip "kendryte-toolchain-win-amd64"
[kendryte-toolchain-win-i386-8.2.0-20190409.zip]: electronic/components/canaan/K210/toolchain/kendryte-toolchain-win-i386-8.2.0-20190409.zip "kendryte-toolchain-win-i386"
[kendryte-toolchain-ubuntu-amd64-8.2.0-20190409.tar.xz]: electronic/components/canaan/K210/toolchain/kendryte-toolchain-ubuntu-amd64-8.2.0-20190409.tar.xz "kendryte-toolchain-ubuntu-amd64"
[kendryte-toolchain-osx-mojave-8.2.0-20190409.tar.xz]: electronic/components/canaan/K210/toolchain/kendryte-toolchain-osx-mojave-8.2.0-20190409.tar.xz "kendryte-toolchain-osx-mojave"
[kendryte-toolchain-osx-darwin-m1-8.2.0-20210717.tar.xz]: electronic/components/canaan/K210/toolchain/kendryte-toolchain-osx-darwin-m1-8.2.0-20210717.tar.xz "kendryte-toolchain-osx-darwin-m1"

[xpack-riscv-none-embed-gcc-8.3.0-1.9-20210402]: https://github.com/kendryte/K210-Micropython-OpenMV/tree/0c70920 "K210 MicroPython & OpenMV v8.3.0-1.9 (2021-04-02)"
[xpack-riscv-none-embed-gcc-8.3.0-1.9-win32-x64.zip]: electronic/components/canaan/K210/toolchain/micropython-openmv/xpack-riscv-none-embed-gcc-8.3.0-1.9-win32-x64.zip "xpack-riscv-none-embed-gcc-8.3.0-1.9-win32-x64"
[xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x64.tar.gz]: electronic/components/canaan/K210/toolchain/micropython-openmv/xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x64.tar.gz "xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x64"
[xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x32.tar.gz]: electronic/components/canaan/K210/toolchain/micropython-openmv/xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x32.tar.gz "xpack-riscv-none-embed-gcc-8.3.0-1.9-linux-x32"

[riscv-none-embed-gcc-xpack-8.3.0-1.2-20200703]: https://github.com/xpack-dev-tools/riscv-none-embed-gcc-xpack/releases/tag/v8.3.0-1.2 "xPack GNU RISC-V Embedded GCC v8.3.0-1.2 (2020-07-03)"
[xpack-riscv-none-embed-gcc-8.3.0-1.2-to-1.9.diff]: electronic/components/canaan/K210/toolchain/micropython-openmv/xpack-riscv-none-embed-gcc-8.3.0-1.2-to-1.9.diff "Canaan Changes from v8.3.0-1.2 to v8.3.0-1.9"

[bj-wanghz/riscv-newlib/sifive-master-xpack-canaan]: https://github.com/xpack-dev-tools/riscv-newlib/compare/sifive-master-xpack...bj-wanghz:riscv-newlib:sifive-master-xpack-canaan "Commit history on SiFive RISC-V Newlib for Canaan"
[xpack-dev-tools/riscv-gcc/sifive-gcc-8.3.0-xpack]: https://github.com/sifive/riscv-gcc/compare/sifive-gcc-8.3.0...xpack-dev-tools:riscv-gcc:sifive-gcc-8.3.0-xpack "Commit history on SiFive RISC-V GCC for Canaan"
[xpack-dev-tools/riscv-binutils-gdb/sifive-binutils-2.32-xpack]: https://github.com/sifive/riscv-binutils-gdb/compare/sifive-binutils-2.32...xpack-dev-tools:riscv-binutils-gdb:sifive-binutils-2.32-xpack "Commit history on SiFive RISC-V Binutils/GDB for Canaan"

[k210_micropython_openmv_user_manual_20210420_en.pdf]: electronic/components/canaan/K210/toolchain/micropython-openmv/k210_micropython_openmv_user_manual_20210420_en.pdf "K210-MicroPython & OpenMV User Manual"

[rt-thread-v4.1.1-20220822]: https://github.com/RT-Thread/rt-thread/releases/tag/v4.1.1 "RT-Thread v4.1.1 (2022-08-22)"
[RT-Thread_Getting-Started-of-QEMU_Windows_221024.pdf]: electronic/components/canaan/K210/toolchain/micropython-openmv/RT-Thread_Getting-Started-of-QEMU_Windows_221024.pdf "RT-Thread: Getting Started of QEMU (Windows)"
[RT-Thread_Getting-Started-of-QEMU_Ubuntu_221024.pdf]: electronic/components/canaan/K210/toolchain/micropython-openmv/RT-Thread_Getting-Started-of-QEMU_Ubuntu_221024.pdf "RT-Thread: Getting Started of QEMU (Ubuntu)"

[kendryte-openocd-v0.2.3-20190221]: https://github.com/kendryte/openocd-kendryte/releases/tag/v0.2.3 "Kendryte OpenOCD v0.2.3 (2019-02-21)"
[WindowsTools.zip]: electronic/components/canaan/K210/toolchain/openocd/WindowsTools.zip "Binary Dependencies für win32"
[kendryte-openocd-0.2.3-win32.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.3-win32.zip "Kendryte OpenOCD for win32"
[kendryte-openocd-0.2.3-ubuntu64.tar.gz]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.3-ubuntu64.tar.gz "Kendryte OpenOCD for Ubuntu x86_64"
[kendryte-openocd-v0.2.2-20190117]: https://github.com/kendryte/openocd-kendryte/releases/tag/v0.2.2 "Kendryte OpenOCD v0.2.2 (2019-01-17)"
[kendryte-openocd-0.2.2-win32.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.2-win32.zip "Kendryte OpenOCD for win32"
[kendryte-openocd-0.2.2-ubuntu64.tar.gz]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.2-ubuntu64.tar.gz "Kendryte OpenOCD for Ubuntu x86_64"
[kendryte-openocd-0.2.2-macos.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.2-macos.zip "Kendryte OpenOCD for MacOS"
[kendryte-openocd-v0.2.1-20190109]: https://github.com/kendryte/openocd-kendryte/releases/tag/v0.2.1 "Kendryte OpenOCD v0.2.1 (2019-01-09)"
[kendryte-openocd-0.2.1-win32.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.1-win32.zip "Kendryte OpenOCD for win32"
[kendryte-openocd-0.2.1-ubuntu64.tar.gz]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.1-ubuntu64.tar.gz "Kendryte OpenOCD for Ubuntu x86_64"
[kendryte-openocd-0.2.1-macos.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.2.1-macos.zip "Kendryte OpenOCD for MacOS"
[kendryte-openocd-v0.1.3-20180913]: https://github.com/kendryte/openocd-kendryte/releases/tag/0.1.3 "Kendryte OpenOCD v0.1.3 (2018-09-13)"
[kendryte-openocd-0.1.3-win32.zip]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.1.3-win32.zip "Kendryte OpenOCD for win32"
[kendryte-openocd-0.1.3-ubuntu64.tar.gz]: electronic/components/canaan/K210/toolchain/openocd/kendryte-openocd-0.1.3-ubuntu64.tar.gz "Kendryte OpenOCD for Ubuntu x86_64"

[cmake-3.14.4-20190514]: https://github.com/Kitware/CMake/releases/tag/v3.14.4 "CMake v3.14.4 (2019-05-14)"
[cmake-3.14.4-win32-x86.zip]: electronic/components/canaan/K210/toolchain/cmake/cmake-3.14.4-win32-x86.zip "cmake-win32-x86"
[cmake-3.14.4-win64-x64.zip]: electronic/components/canaan/K210/toolchain/cmake/cmake-3.14.4-win64-x64.zip "cmake-win64-x64"
[cmake-3.14.4-Linux-x86_64.tar.gz]: electronic/components/canaan/K210/toolchain/cmake/cmake-3.14.4-Linux-x86_64.tar.gz "cmake-linux-x86_64"
[cmake-3.14.4-Darwin-x86_64.tar.gz]: electronic/components/canaan/K210/toolchain/cmake/cmake-3.14.4-Darwin-x86_64.tar.gz "cmake-darwin-x86_64"

[canmv-ide-windows-v2.9.2-30-g65f7289-20220928.zip]: electronic/components/canaan/K210/toolchain/canmv/canmv-ide-windows-v2.9.2-30-g65f7289-20220928.zip "CanMV IDE"

## Comments

### K210 MicroPython & OpenMV Framework with RT-Thread

<span style="width:66%;float:right;background-color:white;">[![k210_micropython_openmv_framework_20210420_en]][k210_micropython_openmv_framework_20210420_en]</span>

[k210_micropython_openmv_framework_20210420_en]: electronic/components/canaan/K210/toolchain/micropython-openmv/k210_micropython_openmv_framework_20210420_en.png "K210-MicroPython & OpenMV Framework with RT-Thread"

1. [OpenMV](https://openmv.io/)
   [![iGo]](https://github.com/openmv)
1. [MicroPython](https://micropython.org/)
   [![iGo]](https://www.github.com/micropython)
1. [RT-Thread](https://www.rt-thread.io/)
   [![iGo]](https://github.com/RT-Thread)
   1. Software Package [MicroPython](https://packages.rt-thread.org/en/detail.html?package=micropython)
      [![iGo]](https://github.com/RT-Thread-packages/micropython)
   1. Software Package [OpenMV](https://packages.rt-thread.org/en/detail.html?package=openmv)
      [![iGo]](https://github.com/RT-Thread-packages-by-SummerGift/openmv)
   1. Software Package [K210-SDK](https://packages.rt-thread.org/en/detail.html?package=K210-SDK)
      [![iGo]](https://github.com/RT-Thread-packages/kendryte-k210-sdk)
   1. Software Package [kendryte-sdk](https://packages.rt-thread.org/en/detail.html?package=kendryte-sdk)
      [![iGo]](https://github.com/RT-Thread-packages/kendryte_sdk)
   1. Software Package [kendryte-demo](https://packages.rt-thread.org/en/detail.html?package=kendryte-demo)
      [![iGo]](https://github.com/BernardXiong/kendryte-demo)
1. [Kendryte](https://kendryte.com/)
   [![iGo]](https://github.com/kendryte)

### OpenOCD for Kendryte RISC-V

The Kendryte OpenOCD forks from riscv-openocd, improved for Kendryte K210:

- [Why need special Kendryte OpenOCD](https://github.com/kendryte/openocd-kendryte/wiki/Overview#why-need-kendryte-openocd)
- [RISC-V External Debug Support Version 0.11](https://static.dev.sifive.com/riscv-debug-spec-0.11nov12.pdf)
- [Fork of OpenOCD that has RISC-V support](https://github.com/riscv/riscv-openocd)

#### OpenOCD Configuration Script

- https://github.com/kendryte/openocd-kendryte/wiki/Configuration
- https://github.com/kendryte/openocd-kendryte/blob/master/tcl/kendryte.cfg
  ```tcl
  # debug adapter
  interface jlink
  # optional: jlink serial 000504401724

  transport select jtag
  adapter_khz 3000

  # server port
  gdb_port 3333
  telnet_port 4444

  # add cpu target
  set _CHIPNAME riscv

  jtag newtap $_CHIPNAME cpu -irlen 5 -expected-id 0x04e4796b

  set _TARGETNAME $_CHIPNAME.cpu
  target create $_TARGETNAME riscv -chain-position $_TARGETNAME

  # command
  init
  halt
  ```

#### OpenOCD Guidance

- [User's Guide](https://github.com/kendryte/openocd-kendryte/wiki/User's-Guide)
- [Debugging with GDB](https://github.com/kendryte/openocd-kendryte/wiki/Debugging-with-GDB)
- [Build on Windows](https://github.com/kendryte/openocd-kendryte/wiki/Build-on-Windows)
- [Build on Linux](https://github.com/kendryte/openocd-kendryte/wiki/Build-on-Linux)
- [Build on MacOSX](https://github.com/kendryte/openocd-kendryte/wiki/Build-on-OSX)

### Linux on Kendryte K210

- Damien Le Moal: [original buildroot for K210 Linux patches](https://github.com/damien-lemoal/buildroot/tree/k210-v21)
  – publish date 2022-07-20
- Damien Le Moal: [modified buildroot for Linux build toolchain](https://github.com/damien-lemoal/riscv64-nommu-buildroot)
  – publish date 2021-04-02
- Patchwork: [RISC-V Kendryte K210 support improvements](https://patchwork.kernel.org/project/linux-clk/list/?series=401137&state=%2A&archive=both)
  – publish date 2020-12-02
- Huang Rui: [K210 run linux nommu (From Damien Le Moal's patch)](https://github.com/vowstar/k210-linux-nommu)
  – publish date 2020-02-24

- [Booting 64-bit RISC-V noMMU Linux with rootfs loaded from SDcard on Sipeed Maix Bit](https://www.luffca.com/2021/08/linux-k210-sdcard-maix-bit)
  – publish date 2021-08-28 
- [RISC-V For Linux 5.8 Finishes Bringing Up The Kendryte K210, Adds KGDB Support](https://www.phoronix.com/news/RISC-V-Changes-Linux-5.8)
  – publish date 2020-06-07
- [Linux 5.7 Begins Landing Support For The Kendryte K210](https://canaan.io/759.html)
  – publish date 2020-05-26
- [Linux 5.7 Begins Landing Support For The Kendryte K210 Dual-Core RISC-V SoC](https://www.phoronix.com/news/Linux-5.7-RISC-V)
  – publish date 2020-04-09
- [How to Build & Run Linux on Kendryte K210 RISC-V NOMMU Processor](https://www.cnx-software.com/2020/02/17/how-to-build-run-linux-on-kendryte-k210-risc-v-nommu-processor)
  – publish date 2020-02-17
- [Western Digital Made RISC-V Linux & BusyBox Boot on Sipeed Maix Go Board](https://www.cnx-software.com/2019/12/03/western-digital-risc-v-linux-busybox-boot-sipeed-maix-go-board)
  – publish date 2019-12-03
