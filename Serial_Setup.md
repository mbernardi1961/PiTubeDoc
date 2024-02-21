<b>Using a serial connection</b>

There are a number of options once you have an appropriate cable made up. As serial ports on PCs are rare now a USB to serial adaptor can be procured.

<b>XFER</b> - Simple file transfer for BBC Micro
https://www.g7jjf.com/bbc.htm<br>
Requies no software to be installed initially on Beeb, just uses two *FX commands, the the basic program is spooled via the serial port. Versions are available for Windows, x86 Linux & Raspberry Pi.

<b>Kermit</b> -  The New Open-Source Kermit Project - https://www.kermitproject.org/ftp/kermit/historic/<br>
There is a rather old version of BBC Kermit which combined with C-Kermit provides a robust and reliable system.<br>
Required settings;

<em>Setup C-Kermit</em> - Using USB Serial Port

set modem type none        ; There is no modem<br>
set line /dev/ttyUSB0        ; Specify device name<br>
;set carrier-watch off      ; If DTR and CD are not cross-connected
set speed 9600            ; Or other desired speed (max speed in BBC Kermit)<br>
set flow rts/cts           ; If RTS and CTS are cross-connected<br>
;set flow xon/xoff          ; If you can't use RTS/CTS<br>
set parity even            ; (or "mark" or "space", if necessary)<br>
;set stop-bits 2            ; (rarely necessary)<br>
connect                    ; Enter<br> Connect (terminal) state

<em>Setup BBC Micro Kermit</em><br>
set baud 9600<br>
set flow cts/rts<br>
set parity even<br>

<b>UPURS</b> - Fast serial transfer utilities for the BBC Micro
https://www.retro-kit.co.uk/UPURS/

<b>SerialFS</b> - ROMless Serial Filing System for the BBC Micro
https://github.com/gfoot/serialfs<br>
Only available for Linux.
