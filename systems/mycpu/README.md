# MyCPU

<div style="display:flex;justify-content:right;">
<small><em>project update on: <strong>$Format:%cs$ with <mark><a href="https://github.com/tiacsys/bridle-electronic/commits/$Format:%h$" title="$Format:%B$" target="_blank">$Format:%h$</a></mark></strong></em></small>
</div>
<div style="display:flex;justify-content:right;">
<small><em>all data checked on <strong>2023-06-23</strong></em></small>
</div>

## About

<span style="width:256px;float:right;">[![system-iso]][system-iso]</span>

[system-iso]: electronic/systems/mycpu/system-iso.jpg "MyCPU (7400-CMOS)"

**MyCPU** is a homebrew CPU that was primary developed for fun. It is a
simple 8-bit processor that is completely built with simple discrete logic
gates of the [74xx CMOS series]. Over the years the project has grown, and
now MyCPU is the brain of a real Personal Computer. The project is totally
open source, and everybody is invited to participate and contribute to the
project.

[74xx CMOS series]: https://en.wikipedia.org/wiki/List_of_7400-series_integrated_circuits

* [MyCPU](http://www.mycpu.eu/)
  – [Self-Build Guides](http://mynor.org/mycpu/guides-e.htm#guides)
  * [MyCPU Processor Selfbuild Guid v20150724e](http://www.mynor.org/mycpu/downloads/MyCPU23_Selfbuild-Guide_150724.zip)
  * [Memory Unit Selfbuild Guide v20150724](http://www.mynor.org/mycpu/downloads/Memory_Selfbuild-Guide_160901.zip)
  * [Multi-I/O Unit Selfbuild Guide v20150724](http://www.mynor.org/mycpu/downloads/Multi-IO_Selfbuild-Guide_150724.zip)
  * [Interrupt Controller Selfbuild Guide v20150724](http://www.mynor.org/mycpu/downloads/IntCtrl_Selfbuild-Guide_150724.zip)
  * [IDE Controller Selfbuild Guide v20150724](http://www.mynor.org/mycpu/downloads/IdeCtrl_Selfbuild-Guide_150724.zip)
  * [VGA Graphic Unit Selfbuild Guide v20150724](http://www.mynor.org/mycpu/downloads/GraphicUnit_Selfbuild-Guide_150724.zip)
  * [Ethernet Interface Controller v20150724](http://www.mynor.org/mycpu/downloads/EthCtrl_Selfbuild-Guide_150724.zip)
  * [Power-Supply for MyCPU v20150724](http://www.mynor.org/mycpu/downloads/PowerSupply_Selfbuild-Guide_150724.zip)
  * [Register-Monitor v20120729](http://www.mynor.org/mycpu/downloads/regmon_120729.zip)
  * [Gerber Files v20210703](http://www.mynor.org/mycpu/downloads/mycpu_gerber_files_20210703.zip)

* Software
  * [Operating System Software v1.25-20160902](http://www.mynor.org/mycpu/downloads/mycpu-software_160902.zip) (Kernel v3.1)
  * [Emulator v8.0-20160902](http://www.mynor.org/mycpu/downloads/cpuemu8.zip)
  * [Emulator v7.0-20141010](http://www.mynor.org/mycpu/downloads/cpuemu7.zip)
  * [ANSI C-Compiler v1.8](http://www.mynor.org/mycpu/downloads/cc65-2.11.0-mycpu-1.8.zip)
  * [Cross Assembler "MyCA" v1.10](http://www.mynor.org/downloads/myca-1.10.zip)
    – [MyCA - The Cross Assembler](http://mynor.org/mycpu/myca.htm)

* Documentation:
  * [MyCPU v2.3 Introduction](http://www.mynor.org/mycpu/downloads/MyCPU23_Introduction.pdf)
  * [Article in the European Physical Journal](http://mynor.org/mycpu/epj03.htm)
  * [Open Office Documents](http://www.mynor.org/mycpu/downloads/documents_150724.zip)
  * [I/O-Address Mapping of Peripheral Devices](http://mynor.org/mycpu/downloads/IO-Addresses.pdf)

* [MyCPU Compact](http://mynor.org/mycpu/mycpucompact.htm)
  * [Schematic v1.0](http://www.mynor.org/mycpu/downloads/mycpucompact-schematics_v1.0.pdf)
  * [Eagle Files v1.0](http://www.mynor.org/mycpu/downloads/MyCPU-Compact-Board_v1.0.zip)
  * [VHDL Files and Tools v20100824](http://www.mynor.org/mycpu/downloads/MyCPU-Compact-Sources_2010-08-24.zip)

* [BudgeTronics Product Page – backplane PCB](https://www.budgetronics.eu/en/building-kits/mycpu-backplane-pcb/a-25889-20)
* [BudgeTronics Product Page – complete PCB set](https://www.budgetronics.eu/en/building-kits/mycpu-complete-pcb-set-20-pieces/a-25886-20)
  * [building instructions](https://www.budgetronics.eu/data/mediablocks/mycpu.zip)

## References

* [HELKUEB: Thomas Heller – MyCPU](https://www.helkueb.de/links/mycpu)

* [picoOS](https://picoos.sourceforge.net/)
  ```
  cvs -z3 -d:pserver:anonymous@a.cvs.sourceforge.net:/cvsroot/picoos co -P contrib
  cvs -z3 -d:pserver:anonymous@a.cvs.sourceforge.net:/cvsroot/picoos co -P picoos
  cvs -z3 -d:pserver:anonymous@a.cvs.sourceforge.net:/cvsroot/picoos co -P sitedoc
  ```

## CPU Block Diagram

| <div style="background-color:white;">[![cpu-block-diagram]][cpu-block-diagram]</div> |
|::|
| CPU Block Diagram v1 |

[cpu-block-diagram]: electronic/systems/mycpu/MyCPU_OldSite/pic_block.gif "CPU Block Diagram v1"
