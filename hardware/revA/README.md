# Avrrrinator Rev. A

This is a single-ended AVR ISP breakout for use with the Bus Pirate v3. It connects directly to the Bus Pirate via a keyed header.

![AVrrrinator Rev A2](images/avrrinator-a2-bp.png)

There is a voltage selection jumper that allows simple switching between the 5v and 3.3v rails provided by the Bus Pirate. Note that while this board allows voltage selection between the Bus Pirate's provided power
rails (5V or 3.3V) that the logic levels are fixed at 3.3v during programming.

## Use

1. Install avrdude

2. Install/plug in your Bus Pirate 3 and make sure that it works on your system. [Bus Pirate AVR programming guide](http://dangerousprototypes.com/docs/Bus_Pirate_AVR_Programming)

3. Plug in all cables, attach the Avrrrinator PCB to the Bus Pirate (note orientation of all cabling before applying power). 
 
4. Set the voltage jumper to your desired level.

5. Write to your AVR breakouts with the following: `avrdude -v -p attiny4313 -c buspirate -P /dev/ttyUSB0 -U flash:w:blinky4313.hex`

Replace: `attiny4313`, `/dev/ttyUSB0`, and `blinky4313.hex` with values from your own environment. 

### Bill of Materials for Revision A
| Quantity | Description | Part number |
| -------- | ----------- | ------ |
| 1        | 6 pin AVR ISP header | [Mouser: 517-9612066404AR](http://www.mouser.com/Search/Refine.aspx?Keyword=517-9612066404AR) |
| 1        | 3 pin breakaway header | 36-pin header: [Mouser: 649-68004-236](http://www.mouser.com/Search/Refine.aspx?Keyword=649-68004-236) / Alternative (3-pin, untested!): [Mouser: 571-1031853](http://www.mouser.com/Search/Refine.aspx?Keyword=571-1031853) |
| 1        | Jumper/Power selector | [Mouser: 151-8033-E](http://www.mouser.com/Search/Refine.aspx?Keyword=151-8033-E) (Red) / [Mouser: 151-8031-E](http://www.mouser.com/Search/Refine.aspx?Keyword=151-8031-E) (Blue) |
| 1 	   | 10 pin PCB to Bus Pirate 3 female connector | [Mouser: 517-8510-4500PL](http://www.mouser.com/Search/Refine.aspx?Keyword=517-8510-4500PL)
| 1 	   | AVR ISP cable (6-pin to 6-pin f/f)\* | [Adafruit: PID 371](http://www.adafruit.com/products/371)

* Colorful (and somewhat odd) alternative at [Digikey P/N: SAM8734-ND](http://www.digikey.com/product-detail/en/IDSD-03-D-06.00-T/SAM8734-ND/3476372). Mouser used to sell a proper 6-pin IDC cable, but they don't anymore (or it is really well hidden).

## Fabrication

**Please note**: Due to the extra I/O pins, this breakout is not readily compatible with a **v4** Bus Pirate.

Get these made at OSHPark by [clicking here](https://oshpark.com/shared_projects/tvIUA78A).

## Assembly

1. Snap 3 pins off of the breakaway header and solder it into the voltage selection area.
2. Solder in the 6-pin ISP header
3. Solder in the Bus Pirate mating header (10 pins).

#### Assembly notes

Most of the difficulty in assembling this board is soldering the 10-pin mating header. There is an alignment line silkscreened on the back
to assist with getting it straight (and in the right orientation). To get a decent result, try soldering one corner pin in, aligning it with 
the silk, and then tacking in an opposite corner.
 
The other headers (power select, 6-pin ISP header) can also be placed with decent precision using this method.

## Todo

Complete assembly writeup (for the brave, just slot in all the components where they fit).

## Notable changes

Revision A2: Silkscreen updates (mostly written on the mask layer), along with BOM change to a direct mounting header.

Revision A1: Initial release. [Previous documentation and BOM](http://open.konspyre.org/blog/2013/01/23/the-avrrrinator-revision-a/).


## Licensing

CC0 Public Domain
