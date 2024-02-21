Using a serial connection

There are a number of options once you have an appropriate cable made up.

Kermit - There is a rather old version of BBC Kermit which combined with C-Kermit provides a robust and reliable system.
Require settings;

Setup C-Kermit - Direct Serial Port

set modem type none        ; There is no modem
set line /dev/ttyS0        ; Specify device name
;set carrier-watch off      ; If DTR and CD are not cross-connected
set speed 9600            ; Or other desired speed
set flow rts/cts           ; If RTS and CTS are cross-connected
;set flow xon/xoff          ; If you can't use RTS/CTS
set parity even            ; (or "mark" or "space", if necessary)
;set stop-bits 2            ; (rarely necessary)
connect                    ; Enter Connect (terminal) state

BBC Micro Kermit
set baud 9600
set flow cts/rts
set parity even

UPURS - Fast serial transfer utilities for the BBC Micro
https://www.retro-kit.co.uk/UPURS/

ROMless Serial Filing System for the BBC Micro
https://github.com/gfoot/serialfs

XFER 

