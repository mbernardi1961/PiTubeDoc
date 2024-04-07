# PiTubeDoc
<b>What to do once you have a PiTubeDirect fitted to your BBC Micro?</b>

So you have just got a PiTubeDirect (https://github.com/hoglet67/PiTubeDirect/wiki) fitted, but what do you do next?

First some examples for each CoPro core (somewhat out of date) - https://github.com/hoglet67/PiTubeDirect/wiki/Examples-for-each-CoPro-core

Boot disk images for varaious CoProcessor cores. - http://www.retroclinic.com/docs/CoPro_Bootdisks.zip & https://mdfs.net/Software/Tube/


Overview of BBC Micro Second Processors - https://sites.google.com/site/jamesskingdom/Home/computers-exposed/bbc-micro-second-processors

Current Default Setting (65C102) https://chrisacorns.computinghistory.org.uk/8bit_Upgrades/Acorn_ADC06_65C102CoPro.html

Master 512 (80186) - http://www.cowsarenotpurple.co.uk/bbccomputer/master512/index.html - https://www.g7jjf.com/512_disc_images.htm -  https://mdfs.net/Software/BBCBasic/M512/

PANOS (32016) - https://chrisacorns.computinghistory.org.uk/Panos.html - https://mdfs.net/Software/Tube/32016/

ARM 2 - https://mdfs.net/Software/Tube/ARM/ - https://www.sprow.co.uk/bbc/armcopro.htm 
<!-- Arthur C compiler will work on ARM2 copro mode if you just set the executables to have load/exec address &8000
comes with suitable headers and runtime libraries too, just have to patch load/exec address so that the copro loads 
at the usual place for Arthur/RISC OS absolute executables. -->

CP/M (Z80) - https://www.g7jjf.com/acornz80_disc_images.htm -  https://mdfs.net/Software/Tube/Z80/

PDP-11 - https://mdfs.net/Software/PDP11/

Flex (6809) - https://mdfs.net/Software/Tube/6809/ - https://chrisacorns.computinghistory.org.uk/docs/Acorn/Tech/Acorn_FLEXfor6809.pdf

ReCo6502 65C816 512K - https://www.zeridajh.org/hardware/reco6502/index.html

And in alpha testing<br>
RISC-V - https://github.com/hoglet67/PiTubeDirect/wiki/RISC-V-Co-Pro-Notes


# Full list of Co-Processors available in current (hognose) stable version.

DIP CPU		Speeed		Startup banner

0	65C02		(Fast)		"Acorn TUBE 65C102 Co-Processor"<br>
1 65C02		3MHz		"Acorn TUBE 6502 64K"<br>
2	65C102		(Fast)		"Acorn TUBE  65C102 Co-Processor" (configured as default)<br>
3	65C102		4MHz		"Acorn TUBE  65C102 Co-Processor"<br>
4 Z80 (1.21)	8MHz		"Acorn TUBE Z80 64K 1.21" <br>
5	Z80 (2.0)		32MHz		"Acorn TUBE Z80 64K 2.00"	<br>
6	Z80 (2.2c)		56MHz		"Acorn TUBE Z80 64K 2.2c"	<br>
7	Z80 (2.30)	112MHz		"Acorn TUBE Z80 64K"	<br>
8	80286		16MHz		"Acorn TUBE 80186 896K"<br>
9	MC6809		4MHz		"6809 TUBE 64K 1.05" (ctrl+shift+break to get prompt)<br>
10	68000		16MHZ		Not Implemented<br>
11	PDP-11		32MHz		"PDP11 TUBE 64K 0.30 "<br>
12	ARM2		32MHz		"Native Acorn ARM Second Processor 4096K"<br>
13	32016		32MHz		"Pandora 32000 V2.00 1024 KB"<br>
14	Disable		Host  		"Acorn MOS"<br>
15	ARM Native	1000MHz		"Native ARM Co Processor 1000MHz" (clean boot to get to prompt)<br>
16	LIB65C02 64K	unknown		"Acorn TUBE 6502 64K"<br>
17	LIB65C02 256K	Turbo 		"Acorn TUBE 6502 256K"<br>
18	65C816 (Dossy) unknown		"Dossytronics 65816 Tube"<br>
19	65C816 (ReCo)	14.7MHz		"ReCo6502 65C816 512K (14.7 MHz)"<br>
20	OPC5LS		unknown		"OPC5LS Co Processor"<br>
21	OPC6		unknown		"OPC6 Co Processor"<br>
22	OPC7		unknown		"OPC7 Co Processor"<br>
24	65C02 (JIT)	(Fast)		"Acorn TUBE 6502 64K"<br>
28 	Ferranti F100-L	unknown		"Ferranti F100-L	(32K words)"<br>

The CPU can be selected by using *FX 151,230,n, and comes into effect at the next Break.<br>
(Fast) is the fastest the ARM core can run depending on the version of Raspberry Pi.

The latest development version (Indigo) is alpha code, but includes a few changes:<br>
8	Change CoPro name from 80286 to 80186<br>
23	New RISC-V Co processor<br>
24	65C02 Co Processor (JIT) now default CoPro<br>
