# ZX1541-Interface
An interface for the Sinclair ZX-81, with which you can use Commodore VC-1541 floppy drives.

![Image of 1541 ZXInterface](https://github.com/DL2DW/ZX1541-Interface/blob/main/Pics/ZX1541_Interface.jpg)

Inspired by this post (https://forum.tlienhard.com/phpBB3/viewtopic.php?f=2&t=3218), I rebuilt the interface. 

The idea originally came from Luis C. Grosso
and was developed in 2004 for the model CZ1500 (a relabelled Timex Sinclair 1500)).

In 2006 Jarek Adamski took up the subject and made some modifications for use with a Sinclair ZX-81.

For this purpose, there is also a website with further information at http://8bit.yarek.pl/interface/zx81.zx1541/index-de.html.

Unfortunately most of the downloads are no longer available there. Whatever files I could find on the internet, I uploaded into this repository. 

I then created a new schematic using the information available there. Additionally some modifications from the above mentioned thread were included.

The board is designed to fit into an old case of the original Sinclair 16kb RAM expansion.

![Image of 1541 ZXInterface PCB](https://github.com/DL2DW/ZX1541-Interface/blob/main/Pics/ZX1541_PCB.jpg)

For the interface to work, a memory expansion is required. Without it there is not enough memory available for the extension to work. The best way to do this is to upgrade the ZX-81 internally.

The interface is equipped with an EEPROM, which contains the firmware. This can be called with the following command:


    RAND USR 8192


In firmware version 1.3 the start screen looks like this:

![Screenshot](https://github.com/DL2DW/ZX1541-Interface/blob/main/Pics/Screenshot.jpg)

## Parts List ##

Here is the list of all required parts

|Designator|Item|Type|
|----------|----|----|
|U1|IS62C256AL-45ULI|SO28|
|U2|AT28C64B-15PC|DIP28|
|U3|74LS139|SO16|
|U4|74LS32|SO14|
|U5|74LS174|SO16|
|U6|74LS365|SO16|
|U7|74LS06|SO14|
|U8|74LS08|SO14|
|Q1|BC807-40|SOT23|
|Q2-3|BCR135|SOT23|
|D1-4, 6-9|LL4148|miniMELF|
|D5|LED red 3mm|THT|
|D10|LED green, 3mm|THT|
|R1,7|680R|0805|
|R2,4,6,8-11,13|1K|0805|
|R3|10K|0805|
|R5|33K|0805|
|R12|4K7|0805|
|C1-7,9|100nF|0805|
|C8|1µF|0805|
|CN2|Pin Header, RM2.54mm, 6pos, right angle|THT|
|JP1|Pin Header, RM2.54, 2pos.|THT|
|SW1|Push button, 6x6mm, right angle|THT|
|For U2|IC Socket 28pos.|DIL28|

Unless otherwise stated:
resistors tolerance 5% or better
Capacitors: X5R or better, 16V or higher

In addition, an approx. 60cm long, 6-core cable, a 6-pin DIN socket in "horseshoe shape" and a 6-pin female connector strip for the connection cable to the floppy is required.
