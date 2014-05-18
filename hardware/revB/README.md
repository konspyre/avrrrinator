# Avrrrinator Rev. B
![Avrrrinator Rev B1](images/avrrrinator-b-preview.png)

### Bill of Materials for Revision B
| Quantity | Description | Part number | Board Placement |
| -------- | ----------- | ----------- | --------------- |
| 2        | 6 pin AVR ISP header | [Mouser: 517-9612066404AR](http://www.mouser.com/Search/Refine.aspx?Keyword=517-9612066404AR) | ISP CS and ISP AUX (6-pin through-hole footprints) |
| 2        | 0.1"/2.54mm breakaway header (2 pins needed for each) | 36-pin header: [Mouser: 649-68004-236](http://www.mouser.com/Search/Refine.aspx?Keyword=649-68004-236) | AVR CS PWR/AUX PWR pins (two pins each) |
| 2        | Jumper/Power coupler | [Mouser: 151-8033-E](http://www.mouser.com/Search/Refine.aspx?Keyword=151-8033-E) (Red) / [Mouser: 151-8031-E](http://www.mouser.com/Search/Refine.aspx?Keyword=151-8031-E) (Blue) | Jumpers on two-pin CS/AUX power normally placed to close |
| 1        | 10 pin PCB to Bus Pirate 3 female connector | [Mouser: 517-8510-4500PL](http://www.mouser.com/Search/Refine.aspx?Keyword=517-8510-4500PL) | Bus Pirate v3 header (bottom side with keyed slot matching outline) | 
| 2        | AVR ISP cable (6-pin to 6-pin f/f)\* | [Adafruit: PID 371](http://www.adafruit.com/products/371) | N/A |
| 2        | 0603 imperial 0.1µF capacitors | [Mouser: VJ0603Y104JXJPW1BC](http://www.mouser.com/Search/Refine.aspx?Keyword=VJ0603Y104JXJPW1BC) | C1 and C2 |
| 2        | 74HC125 buffers | [Mouser: SN74HC125PWR](http://www.mouser.com/Search/Refine.aspx?Keyword=SN74HC125PWR) | IC1 and IC2 - Match silkscreen circle orientor with IC's |
| 8        | 0603 imperial 10k ohm resistors | [Mouser: CR0603-JW-103GLF](http://www.mouser.com/Search/Refine.aspx?Keyword=CR0603-JW-103GLF) | R1, R2, R3, R4, R5, R6, R7, R8 (or R1-R8) |
| 2        | Surface mount power selection switch | [Mouser](http://www.mouser.com/Search/Refine.aspx?Keyword=PCM12SMTR)/[Digikey](http://www.digikey.com/product-detail/en/PCM12SMTR/401-2016-1-ND/)/[Newark](http://www.newark.com/c-k-components/pcm12smtr/switch-slide-spdt-300ma-through/dp/28C3147): PCM12SMTR | Top and bottom switches (they should fit into the non-plated drills and be somewhat flush with the board | 

* Colorful (and somewhat odd) alternative at [Digikey P/N: SAM8734-ND](http://www.digikey.com/product-detail/en/IDSD-03-D-06.00-T/SAM8734-ND/3476372). Mouser used to sell a proper 6-pin IDC cable, but they don't anymore (or it is really well hidden).

### Alternative connector for Bus Pirate to Avrrrinator Rev. B

Exchanging the Bus Pirate <-> Avrrrinator connector for these two items allows the Avrrrinator PCB to be located further away from the Bus Pirate. This was the method used in early prototypes (it isn't recommended since things just end up flopping everywhere).

| Quantity | Description | Part number |
| -------- | ----------- | ----------- |
| 1        | 10-pin IDC cable | [Adafruit: 370](adafru.it/370) |
| 1        | 10-pin box connector | [Mouser: 538-90130-1110](http://www.mouser.com/Search/Refine.aspx?Keyword=5538-90130-1110) |
