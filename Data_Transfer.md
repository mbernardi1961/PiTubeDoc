Getting stuff onto your Beeb

The BBC Micro has a lot of communion ports to provide expandability, and many of these are now being used in ways unexpected when it was originally designed. The PiTubeDirect being a case in point.

Back in the 1980s storage was very expensive (sharing a Winchester hard drive made Econet economical) so the idea of 1TB storage available to simply plug into your home computer was science fiction.

So originally there were 5 ways to get data onto your Beeb.
Tape - Historically the original and cheapest method, but very slow and unreliable
ROM - Fast, but can't write to it, and replacement required dismantling (both issues fixed over time)
Disk - While initially expensive to buy the floppy disk drives, the 5" disks were fairly inexpensive (but now difficult to get hold of). Winchester drives not included as cannot be used to get data from outside except..
Econet - Allows sharing of Winchester drives to multiple BBC Micros, so once data copied to (using one of the other methods) can be used by all on the network.
Serial - Used with a cable to connect to another computer or a modem to allow access to other computers via the phone line.

So how have times changed?

5" floppies are now unobtainable, and while 3" floppies are still found, floppy emulators seem to be most common.

GOTEK - connects to floppy drive interface, uses usb storage, available from RetroClinic with appropriate Beeb interface.

Compact Flash Hard Drive - connects to 1MHz bus and acts like a Winchester Disk (I have one installed myself). Supplied as a kit by RetroClinic. Not easy to copy stuff to it, but once on works like magic.

SD card reader - Multiple types inexpensive, but usually requiring a ROM to be installed.

MasterSD, Acorn BBC Master SD Card Interface Cartridge
http://ramtop-retro.uk/mastersd.html
This uses the Master ROM cartridge interface to provide a SD Card reader, a MMFS ROM filing system (https://github.com/hoglet67/MMFS), and a spare sideways RAM bank. 

Econet is fairly expensive to set up, though it's cheaper now than originally. An interface has to be added to the Beeb, and a server needs to be setup. originally this was another Beeb, but now a Raspberry Pi can be setup with a special hat and software for a lot less (this is still the most expensive option) and does allow for internet connectivity.

Serial - This is the cheapest option, that doesn't require any modification of the Beeb (by instally a new ROM or hardware). An appropriate cable will be needed, and a PC of some sort to act as a host.
