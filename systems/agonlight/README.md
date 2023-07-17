# Agon light™ and AgonLight2

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2023-07-15</strong></em></small>
</div>

## About

### Agon light™

<span style="width:256px;float:right;">[![system-v1-iso]][system-v1-iso]</span>

[system-v1-iso]: electronic/systems/agonlight/system-v1-iso.jpg "Agon light™"

**Agon light™** is a fully open-source 8-bit microcomputer and
microcontroller in one small, low-cost board, built with state-of-the-art
21st-century technology. It has two claims to fame, the fastest and cheapest
8-bit microcomputer ever made and the world's sole standalone, instant-on,
BASIC-programmed microcontroller that dispenses with a host PC and sketch
compilation. To find out more about what makes Agon light™ unique, useful
and attractive, please visit the [official website].

Agon light™'s architecture takes inspiration from the classical mainframe with
terminal structure. Its 'mainframe' or processor subsystem includes the CPU
proper (an eZ80 running at 18.432 MHz), system memory (parallel SRAM, 512KB),
a µSD-card slot and several general-purpose I/O lines. The 'terminal' or
Audio/Video subsystem contains an ESP32-PICO-D4 system-on-a-chip running at
240 MHz, 8MB of memory (pSRAM) and ports for video (VGA), audio and keyboard
(PS/2). Agon light™ takes 5V input power either from its USB or GPIO port.

[official website]: https://www.thebyteattic.com/p/agon.html

### AgonLight2

<span style="width:256px;float:right;">[![system-v2-iso]][system-v2-iso]</span>

[system-v2-iso]: electronic/systems/agonlight/system-v2-iso.jpg "AgonLight2"

**AgonLight2** is a re-design of the original Open Source Hardware design of
**Agon light™** made by Bernardo Kastrup a.k.a. [TheByteAttic]. The firmware
is developed by Dean Belfield a.k.a. [breakintoprogram]. The European Union
computer company [OLIMEX] Ltd. has created [a lower-cost version of Agon light™]
(fully compatible with the original) and sells it for just EUR 50 (w/o VAT)
fully assembled, programmed and tested.

[TheByteAttic]: https://github.com/TheByteAttic
[breakintoprogram]: https://github.com/breakintoprogram
[OLIMEX]: https://github.com/OLIMEX
[a lower-cost version of Agon light™]: https://www.olimex.com/Products/Retro-Computers/AgonLight2/open-source-hardware

#### Features

  * *processor subsystem* for main firmware operations (**MOS**):
    * *eZ80F92*: **eZ80** Zilog eZ80Acclaim!® 8-bit processor at 18.432 MHz
      with **128KB Flash** and **8KB SRAM**
    * *AS7C34096A*: **512KB** external **SRAM** at 100 MHz (10ns, parallel SRAM)
    * 2x **UART** with independent baud rate generators (VDP serial link and [UEXT] connector)
    * 1x **SPI** with independent clock rate generator (34-pin and [UEXT] connector)
    * 1x **I2C** with independent clock rate generator (34-pin and [UEXT]/[ACCESS.bus] connector)
    * 6x **16-bit Counter/Timers** with clock dividers and direct I/O drive
    * 1x **RTC** with on-chip 32 kHz oscillator
    * 1x **WDT**
    * 13x **GPIO** at 34-pin connector
    * **MicroSD** card connector for runtime environments (**BBC BASIC**)
    * OLIMEX **[UEXT]** connector
    * Philips/DEC  **[ACCESS.bus]** connector
    * Zilog **ZDI** connector for programming the eZ80’s **Quark™ MOS** firmware
  * *terminal subsystem* for Audio/Video-IO (**VDP**):
    * *ESP32-PICO-D4*: **ESP32** Xtensa® 32-bit LX6 dual core co-processor at 240 MHz
      with on-chip **448KB Flash** and **520KB SRAM** and **4MB** on-module **Flash**
      at 133 MHz (serial Flash) as *System-in-Package* (**SiP**) module
    * *APS6404L-3SQR*: **8MB** external **SRAM** at 133 MHz (7.5 ns, serial pSRAM)
    * 2x **UART** for programming (2-wire RxD/TxD) and VDP serial link (4-wire RxD/TxD/CTS/RTS)
    * 1x **SDIO** for external serial pSRAM (6-wire SIO[0-3]/SCL/SCS)
    * 1x **DAC** for audio output channel
    * 8x **GPIO** for VGA video output (6-bit RGB222 with VS/HS)
    * 2x **GPIO** for PS/2 keyboard (KDAT/KCLK)
    * 2x **GPIO** for VDP to MOS link handshake (ITRP/VS)
    * 4x **64-bit Counter/Timers** with clock 16-bit dividers and direct I/O drive
    * 1x **RTC** with additional **2x8KB SRAM** and on-chip 32 kHz oscillator
    * 3x **WDT** (2x MAIN-WDT and 1x RTC-WDT)
    * 1x **Crypt** (AES/RSA/SHA)
    * 7x **GPIO** at 34-pin connector
    * **VDP full-duplex high-speed serial link** (1.152 MBit/s, flow control)
    * **Audio** jack output (2 identical mono channels, shared with Buzzer)
    * **VGA** output (various modes, 64 colors)
    * (USB)/**PS2** keyboard, **only PS/2 over USB connector**
    * **USB 2.0** port for power and via **CP2104** USB-UART bridge for
      programming the ESP32’s **Quark™ VDP** firmware
  * *miscellaneous*:
    * Li-Po battery charger and step-up converter
    * **5V powered by USB** and runs **internally at 3.3V** with 5V tolerant inputs
    * Buzzer (via **Quark™ VDP** firmware)
    * Reset button
    * 6 mount holes
    * Dimensions: **(106 x 65) mm**

[UEXT]: https://www.olimex.com/Products/Modules/UEXT
[ACCESS.bus]: https://en.wikipedia.org/wiki/ACCESS.bus

#### Hardware revision changes for AgonLight2

Board revision can be identified by the white print. It is printed on the
board itself. Boards were designed with KiCad.

##### Hardware revision B (initial release)

First public release. Major changes compared to hardware revision A:

  1. VGA and audio jack moved to the left 1mm;
  2. ZDI connector pinout fixed;
  3. R22 now 2.2K, moved between B and C of transistor for feedback;
  4. Improved the logo print;
  5. R41 now NA;
  6. Improved keyboard design, R35 and R36 now NA;
  7. R17 now 10K.

##### Hardware revision A (preliminary, unrleased)

Initial take over from EasyEDA to KiCad v5.

### AgonLight2-Proto

<span style="width:256px;float:right;">[![system-diyproto-iso]][system-diyproto-iso]</span>

[system-diyproto-iso]: electronic/systems/agonlight/system-diyproto-iso.jpg "AgonLight2-Proto"

**AgonLight2-Proto** is a small extension DIY kit compatbile with AgonLight2.
It allows you to fast prototype concepts and ideas with the AgonLight2 8-bit
microcomputer. LEDs, resistors, IDC connector are not soldered. It is also
[distributed under the same name AgonLight2-Proto] by the European Union
computer company [OLIMEX] Ltd.

[distributed under the same name AgonLight2-Proto]: https://www.olimex.com/Products/Retro-Computers/AgonLight2-Proto/open-source-hardware

#### Features

  * **Female-IDC connector 34 pin** for connection to AgonLight2's **GPIO header**
  * 3mm **RED LED for 5V** power indication
  * 3mm **GREEN LED for 3.3V** power indication
  * 2 x 2k PTH resistors for the LEDs
  * **Sea-of-pads spaced at 2.54mm**
  * GND and 3.3V bus connecting vertically all pads on the left edge
  * GND and 5V bus connecting vertically all pads on the right edge
  * Dimensions: **(100 x 80) mm**
  * 3 x distance spacers for keeping the board horizontal when ICD connector
    is attached to AgonLight2's GPIO

#### Hardware revision changes for AgonLight2

Board revision can be identified by the white print. It is printed on the
board itself. Boards were designed with KiCad.

##### Hardware revision A (initial release)

Initial created with KiCad v7.

## Design Data

### [AgonLight2](https://github.com/OLIMEX/AgonLight2)

  * [Schematic Rev B](https://github.com/OLIMEX/AgonLight2/raw/main/HARDWARE/AgonLight2_Rev_B/AgonLight2_Rev_B.pdf)
  * [KiCad Files Rev B](https://github.com/OLIMEX/AgonLight2/tree/main/HARDWARE/AgonLight2_Rev_B)
  * [Gerber Files Rev B](https://github.com/OLIMEX/AgonLight2/tree/main/HARDWARE/AgonLight2_Rev_B/Gerbers)
  * [BOM Rev B](https://github.com/OLIMEX/AgonLight2/raw/main/HARDWARE/AgonLight2_Rev_B/AgonLight2_Rev_B_BOM.ods)

#### [AgonLight2-Proto](https://github.com/OLIMEX/AgonLight2-Proto)

  * [Schematic Rev A](https://github.com/OLIMEX/AgonLight2-Proto/raw/main/HARDWARE/AgonLight2-PROTO_Rev_A/AgonLight2-PROTO_Rev_A.pdf)
  * [KiCad Files Rev A](https://github.com/OLIMEX/AgonLight2-Proto/raw/main/HARDWARE/AgonLight2-PROTO_Rev_A)
  * [Gerber Files Rev A](https://github.com/OLIMEX/AgonLight2-Proto/raw/main/HARDWARE/AgonLight2-PROTO_Rev_A/Gerbers)
  * [BOM Rev A](https://github.com/OLIMEX/AgonLight2-Proto/raw/main/HARDWARE/AgonLight2-PROTO_Rev_A/AgonLight2-PROTO_Rev_A-BOM.ods)

### [Agon light™](https://github.com/TheByteAttic/AgonLight)

  * [Schematic R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Design/Schematic_AgonLight_R1.0.pdf)
  * [Layers & Races R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Design/AgonLight_R1.0_Layers%26Traces.pdf)
  * [EasyEDA Backup R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Design/AgonLight_R1.0_EasyEDA_Backup.zip)
  * [Gerber Files R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Manufacturing/Gerber_PCB_AgonLight_R1.0.zip)
  * [Pick & Place R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Manufacturing/PickAndPlace_PCB_AgonLight_R1.0.csv)
  * [BOM R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/Manufacturing/BOM_PCB_AgonLight_R1.0.csv)
  * [Dimensions R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/3D%20model/Agon%20light%20PCB%20dimensions.png)
  * [3D Model R1.0](https://github.com/TheByteAttic/AgonLight/raw/main/3D%20model/AgonLight_R1.0_PCB_3Dmodel.zip)

## Software

  * [MicroSD card files for Agon light™ R1.0](https://github.com/TheByteAttic/AgonLight/tree/main/uSD%20card%20files)
  * [Quark™ MOS 1.00 or later](https://github.com/breakintoprogram/agon-mos)
  * [Quark™ VDP 1.00 or later](https://github.com/breakintoprogram/agon-vdp)
  * [Quark™ BBC BASIC](https://github.com/breakintoprogram/agon-bbc-basic)

## Documentation

  * [AgonLight2 Rev B User Manual](https://github.com/OLIMEX/AgonLight2/raw/main/DOCUMENTATION/AgonLight2-user-manual.pdf)
  * [Agon light™ R1.0 Manual](https://github.com/TheByteAttic/AgonLight/raw/main/Agon%20light%20R1.0%20Manual.pdf)
  * [Agon light™ Quick Start Guide](https://github.com/TheByteAttic/AgonLight/raw/main/Agon%20light%20Quick%20Start%20Guide.pdf)
  * [Agon light™ Firmware Installation Guide](https://github.com/TheByteAttic/AgonLight/raw/main/Agon%20light™%20Firmware%20Installation%20Guide.pdf)
  * [Agon Quark™ Official Firmware Documentation Wiki](https://github.com/breakintoprogram/agon-docs/wiki)
  * [Agon Quark™ Supplemental Programmers Documentation Wiki](https://github.com/envenomator/Agon/wiki)
  * [Agon Quark™ Collection of code, docs and libraries](https://github.com/envenomator/Agon)
  * [Agon Quark™ BBC BASIC manual](https://oldpatientsea.github.io/agon-bbc-basic-manual/0.1/index.html)
    – asciidoctor sources on [GitHub](https://github.com/oldpatientsea/agon-bbc-basic-manual) by Tim Delmare a.k.a. [oldpatientsea]

[oldpatientsea]: https://github.com/oldpatientsea

## Toolbox and Utilities

  * [Agon light™ improved native eZ80 assembler](https://github.com/envenomator/agon-ez80asm)
    by Jeroen Venema a.k.a. [envenomator] (`agon-ez80asm`) provides exactly the
    same features as the Agon Quark™ BBC BASIC interpreter built-in (inline)
    assembler but for native usage on host for cross-assembly
  * [Agon light™ emulator](https://github.com/astralaster/agon-light-emulator)
    by Sascha Schneider a.k.a. [astralaster] written in Rust that uses its own
    [Agon light™ VDP emulation](https://github.com/astralaster/agon-light-vdp) and the
    [Agon light™ CPU (eZ80F92) emulation](https://github.com/tomm/agon-cpu-emulator)
    by Tom Morton
  * [Agon HEXLOAD utility](https://github.com/envenomator/agon-hexload)
  * [Quark™ MOS firmware update utility](https://github.com/envenomator/agon-flash),
    [Quark™ MOS ZDI flash utility](https://github.com/envenomator/agon-flash)
    by Jeroen Venema a.k.a. [envenomator] allows users to update/change the
    firmware of the eZ80 CPU without the need to have a Zilog USB Smart Cable
    option for doing so
  * [Agon Electron HAL](https://github.com/S0urceror/AgonElectronHAL),
    [Agon Electron Flash](https://github.com/S0urceror/AgonElectronFlash), and
    [Agon ZDI Load](https://github.com/S0urceror/agon-zdi-load)
    by Mario Smit a.k.a. [S0urceror] to unbrick your Agon during firmware
    experimentation again without the original Zilog USB Smart Cable option
  * [Small utils for Agon light™](https://github.com/nihirash/Agon-MOS-Tools)
    by Alexander Sharikhin a.k.a. [nihirash]
  * [Quark™ MOS Template for SDCC projects](https://github.com/nihirash/Agon-MOS-SDCC-Template)
    by Alexander Sharikhin a.k.a. [nihirash]
  * [AgDev – Agon light™ port of the TI-84 Plus CE C/C++ toolchain](https://github.com/pcawte/AgDev)
    by Paul Cawte a.k.a. [pcawte], based on LLVM toolchain,
    generating eZ80 ADL code and fasmg eZ80 assembler and linker
  * [native eZ80 (Z80) disassembler](https://github.com/pcawte/eZ80-dis)
    by Paul Cawte a.k.a. [pcawte], based on LLVM toolchain

[envenomator]: https://github.com/envenomator
[astralaster]: https://github.com/astralaster
[S0urceror]: https://github.com/S0urceror
[nihirash]: https://github.com/nihirash
[pcawte]: https://github.com/pcawte

## Operating Systems and Runtime Environments

  * [Agon Electron OS](https://github.com/S0urceror/AgonElectronOS)
    by Mario Smit a.k.a. [S0urceror] with two personalities: CP/M 2.2 machine
    having 64kB at it's disposal and can run CP/M DSK images (128 byte sectors)
    and MSX-DOS machine that can run CP/M and MSX-DOS programs on MS-DOS
    compatible DSK images (512 byte sectors, 9 sectors, 80 tracks, 2 sides)
  * [CP/M 2.2 for Agon light™ and AgonLight2)](https://github.com/nihirash/Agon-CPM2.2)
    by Alexander Sharikhin a.k.a. [nihirash] that doesn't require reflashing
    the Quark™ VDP firmware, but that cause terminal issues
  * [CP/M 2.2 for Agon light™ and AgonLight2 with FAT file system formatted SD card](https://bitbucket.org/cocoacrumbs/agon-light-cpm)
    by Koen van Nieuwehoven a.k.a. [cocoacrumbs] that needs a
    [specific version of the Quark™ VPD firmware](https://bitbucket.org/cocoacrumbs/agon-vpd-cpm)
    to provide an ANSI VT100 terminal emulator for CP/M
  * [Native FORTH interpreter](https://github.com/lennart-benschop/agon-forth)
    by Lennart Benschop

[cocoacrumbs]: https://bitbucket.org/cocoacrumbs

## Applications and Games

  * [Sokoban game for Agon light™](https://github.com/envenomator/agon-sokoban)
    by Jeroen Venema a.k.a. [envenomator]
  * [Rocks'n'Diamonds-like game for Agon light™](https://github.com/nihirash/Agon-rokky)
    by Alexander Sharikhin a.k.a. [nihirash]
  * [Snail – fast Gopher browser for Agon light™ and AgonLight2](https://github.com/nihirash/Agon-MOS-Tools/tree/main/esp8266/snail)
    by Alexander Sharikhin a.k.a. [nihirash]

## Hard- and Software Components

### Zilog eZ80F92

* [eZ80Acclaim!® Flash MCU eZ80F92/eZ80F93 Product Specification](http://www.zilog.com/docs/ez80acclaim/ps0153.pdf)
* [Crystal Oscillator/Resonator Guidelines for eZ80 and eZ80Acclaim!®](http://www.zilog.com/docs/ez80acclaim/appnotes/tn0013.pdf)
* [eZ80Acclaim!® Design for Debug](http://www.zilog.com/docs/ez80acclaim/appnotes/tn0035.pdf)

#### [Zilog Software Download Page](https://www.zilog.com/index.php?option=com_zcm&task=sdlp&Itemid=74)

* [eZ80 CPU User Manual](http://www.zilog.com/docs/um0077.pdf)
* [eZ80 C Compiler User Manual](http://www.zilog.com/docs/ez80/devtools/um0055.pdf)
* [How To Make eZ80 Code Execute Faster With Copy To RAM](http://www.zilog.com/docs/appnotes/an0151.pdf)
* [Setting Interrupts with the eZ80 CPU](http://www.zilog.com/docs/appnotes/an0170.pdf)
* [Setting Interrupts in ADL Mode on eZ80190, eZ80L92, eZ80F92, and eZ80F93 Devices](http://www.zilog.com/docs/appnotes/tn0021.pdf)
* [Setting Interrupts in Z80 Mode on eZ80190, eZ80L92, eZ80F92, and eZ80F93 Devices](http://www.zilog.com/docs/appnotes/tn0023.pdf)

##### `SD00078` [Zilog Developer Studio II (ZDSII) eZ80Acclaim! v5.3.5](https://www.zilog.com/index.php?option=com_zcm&task=view&soft_id=54&Itemid=74)

  * [Zilog Developer Studio II (ZDSII) eZ80Acclaim! v5.3.5 – README](https://www.zilog.com/software/readme/SD00078readme.txt)
  * [Zilog Developer Studio II eZ80Acclaim! – User Manual](http://www.zilog.com/docs/devtools/um0144.pdf)

##### `SD00079` [Zilog Smart Flash Programmer (SFP) v2.4.0](https://www.zilog.com/index.php?option=com_zcm&task=view&soft_id=55&Itemid=74)

  * [Smart Flash Programmer (SFP) v2.4.0 – README](https://www.zilog.com/software/readme/SD00079readme.txt)
  * [Smart Flash Programmer (SFP) – Product Brief](http://www.zilog.com/docs/devtools/pb0158.pdf)
  * [Smart Flash Programmer (SFP) – Quick Start Guide](http://www.zilog.com/docs/devtools/qs0058.pdf)

#### `ZUSBASC0200ZACG` [eZ80Acclaim!® USB Smart Cable](https://www.zilog.com/index.php?option=com_product&task=dev_tool_detail&DevToolKit=ZUSBASC0200ZACG)

  * [eZ80Acclaim!® Smart Cable – Flyer](https://www.zilog.com/docs/ez80/fl0200.pdf)
  * [eZ80Acclaim!® Smart Cable – User Manual](https://www.zilog.com/docs/ez80/um0296.pdf)

#### `ZUSBSC00100ZACG` [USB Smart Cable](https://web.archive.org/web/20201025190155/https://www.zilog.com/index.php?option=com_product&task=dev_tool_detail&DevToolKit=ZUSBSC00100ZACG)

  * [USB Smart Cable – Flyer](https://www.zilog.com/docs/fl0180.pdf)
  * [USB Smart Cable – User Manual](http://www.zilog.com/docs/devtools/um0181.pdf)

#### `ZENETSC0100ZACG` [Ethernet Smart Cable](https://web.archive.org/web/20201025194044/https://www.zilog.com/index.php?option=com_product&task=dev_tool_detail&DevToolKit=ZENETSC0100ZACG)

  * [Ethernet Smart Cable – User Manual](https://www.zilog.com/docs/devtools/um0207.pdf)

### Espressif ESP32-PICO-D4

#### Espressif [ESP32 Resources Page](https://espressif.com/products/hardware/esp32/resources)

  * [ESP32 Datasheet v4.3](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
  * [ESP32 Series SoC Errata v2.6](https://www.espressif.com/sites/default/files/documentation/esp32_errata_en.pdf)
  * [ESP32 Chip Revision v3.0 User Guide v1.3](https://www.espressif.com/sites/default/files/documentation/esp32_chip_revision_v3_0_user_guide_en.pdf)
  * [ESP32 Technical Reference Manual v5.0](https://www.espressif.com/sites/default/files/documentation/esp32_technical_reference_manual_en.pdf)
  * [ESP32 Hardware Design Guidelines v3.3](https://www.espressif.com/sites/default/files/documentation/esp32_hardware_design_guidelines_en.pdf)
  * [ESP32 Audio Design Guidelines v1.0](https://www.espressif.com/sites/default/files/documentation/esp32_audio_design_guidelines__en.pdf)
  * [ESP32 Bluetooth Architecture v1.1](https://www.espressif.com/sites/default/files/documentation/esp32_bluetooth_architecture_en.pdf)
  * [ESP32 BT&BLE Dual-mode Bluetooth v1.0](https://www.espressif.com/sites/default/files/documentation/btble_coexistence_demo_en.pdf)
  * [ESP32 Bluetooth Networking User Guide v1.2](https://www.espressif.com/sites/default/files/documentation/esp32_bluetooth_networking_user_guide_en.pdf)
  * [ESP32-PICO-D4 Datasheet v2.0](https://www.espressif.com/sites/default/files/documentation/esp32-pico-d4_datasheet_en.pdf)

#### Espressif [ESP-IDF Programming Guide v5.1](https://docs.espressif.com/projects/esp-idf/en/v5.1/esp32)

  * [ESP32 Flash Encryption Guide](https://docs.espressif.com/projects/esp-idf/en/v5.1/esp32/security/flash-encryption.html)
  * [JTAG Debugging for ESP32](https://docs.espressif.com/projects/esp-idf/en/v5.1/esp32/api-guides/jtag-debugging/index.html)
  * https://github.com/espressif/esp-idf
    * https://github.com/espressif/esp-idf/releases/tag/v5.1
    * https://docs.espressif.com/projects/esp-idf/en/v5.1/esp32/esp-idf-en-v5.1-esp32.pdf
    * [ESP-IDF RTOS SDK v5.1](https://github.com/espressif/esp-idf/releases/download/v5.1/esp-idf-v5.1.zip)

#### Espressif [ESP-AT User Guide v2.4.0.0](https://docs.espressif.com/projects/esp-at/en/release-v2.4.0.0/esp32)

  * [ESP32 AT Instruction Set and Examples](https://docs.espressif.com/projects/esp-at/en/release-v2.4.0.0/esp32/AT_Command_Set/index.html)
  * https://github.com/espressif/esp-at
    * https://github.com/espressif/esp-at/releases/tag/v2.4.0.0
    * https://docs.espressif.com/projects/esp-at/en/release-v2.4.0.0/esp32/esp-at-en-v2.3.0.0_esp32c3-182-g6e9756e7-esp32.pdf
    * [ESP32-PICO-D4 AT Bin v2.4.0.0](https://github.com/espressif/esp-at/files/8739825/ESP32-PICO-D4_AT_Bin_V2.4.0.0.zip)

#### Espressif [Audio Development Guide (latest)](https://docs.espressif.com/projects/esp-adf/en/latest)

  * https://espressif-docs.readthedocs-hosted.com/_/downloads/esp-adf/en/latest/pdf/
  * https://github.com/espressif/esp-adf

#### Espressif [ESP-Jumpstart (latest)](https://docs.espressif.com/projects/esp-jumpstart/en/latest)

  * https://espressif-docs.readthedocs-hosted.com/_/downloads/esp-jumpstart/en/latest/pdf/
  * https://github.com/espressif/esp-jumpstart

## References

### [breakintoprogram: Dean Belfield – Agon](http://www.breakintoprogram.co.uk/hardware/computers/agon)

  * [Motherboard](http://www.breakintoprogram.co.uk/hardware/computers/agon/motherboard)
  * [Development Toolchain](http://www.breakintoprogram.co.uk/hardware/computers/agon/development-toolchain)
  * [Memory Map](http://www.breakintoprogram.co.uk/hardware/computers/agon/memory-map)

### [olimex: OLIMEX Ltd – Agon light™](https://olimex.wordpress.com/category/agonlight)

  * [AgonLight2-Proto simple prototyping board for AgonLight2 retro Z80 computer](https://olimex.wordpress.com/2023/06/13/agonlight2-proto-simple-prototyping-board-for-agonlight2-retro-z80-computer)
  * [AgonLight2 update: embedded Hello world in BBC basic](https://olimex.wordpress.com/2022/12/22/agonlight2-update-embedded-hello-world-in-bbc-basic)
  * [AgonLight2 now is officially certified by OSHWA as Open Source Hardware](https://olimex.wordpress.com/2022/12/22/agonlight2-now-is-officially-certified-by-oshwa-as-open-source-hardware)
  * [AgonLight Open Source Hardware Retro Computer Running BBC Basic was captured in KiCad and updated by Olimex](https://olimex.wordpress.com/2022/12/09/agonlight-open-source-hardware-retro-computer-running-bbc-basic-was-captured-in-kicad-and-updated-by-olimex)

### [cocoacrumbs: Koen van Nieuwehoven – EZ80](https://www.cocoacrumbs.com/categories/ez80)

  * [Getting the Agon light™ SD Card to work under NuttX](https://www.cocoacrumbs.com/blog/2023-06-14-getting-the-sd-card-to-work-on-nuttx)
    – [NuttX v9.1.1 branch `ccc_dev_branch`](https://bitbucket.org/cocoacrumbselectronics/nuttx-9.1.1/branch/ccc_dev_branch)
  * [Running NuttX on the AgonLight2](https://www.cocoacrumbs.com/blog/2023-06-09-running-nuttx-on-the-agonlight2)
  * [Running NuttX on the eZ80](https://www.cocoacrumbs.com/blog/2023-06-08-running-nuttx-on-the-ez80)
  * [Running NuttX on the eZ80](https://www.cocoacrumbs.com/blog/2023-06-08-running-nuttx-on-the-ez80)
  * [Building NuttX for the eZ80 on Linux](https://www.cocoacrumbs.com/blog/2023-06-07-building-nuttx-for-the-ez80-on-linux)

### [cocoacrumbs: Koen van Nieuwehoven – RETRO COMPUTING](https://www.cocoacrumbs.com/categories/retro-computing)

  * [Using the Zilog Developer Studio II (ZDS II) for the eZ80 on Linux](https://www.cocoacrumbs.com/blog/2023-04-28-using-zilog-zds-ii-on-linux)
  * [Deciphering Zilog's lod file format](https://www.cocoacrumbs.com/blog/2023-01-01-reading-zilogs-lod-file-format)
  * [Experimenting with the LLVM/Clang toolchain for the Zilog ezZ0](https://www.cocoacrumbs.com/blog/2021-12-28-experimenting-with-the-llvm-toolchain-for-the-ez80)
    – [ez80-LLVM-toolchain](https://bitbucket.org/cocoacrumbselectronics/ez80-llvm-toolchain)
    : shell script that builds the LLVM/Clang toolchain with the Z80/ez80 backend
    – [minimal-C-runtime](https://bitbucket.org/cocoacrumbselectronics/minimal-c-runtime)
    : minimal amount of code to run this simple C code

* [electronics-lab: Saumitra Jagdale – Agon light](https://www.electronics-lab.com/agon-light-is-a-fully-open-source-8-bit-microcomputer-and-microcontroller)

## System Block Diagram

| <div style="background-color:white;">[![cpu-block-diagram]][cpu-block-diagram]</div> |
|::|
| System Block Diagram v1 |

[cpu-block-diagram]: electronic/systems/agonlight/system-diagram.png "System Block Diagram v1"

## System GPIO Pinouts

| <div style="background-color:white;">[![gpio-pinouts]][gpio-pinouts]</div> |
|::|
| System GPIO Pinouts v1 |

[gpio-pinouts]: electronic/systems/agonlight/system-gpio-pinouts.png "System GPIO Pinouts v1"
