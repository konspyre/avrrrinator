# avrrrinator

These are the Eagle source files for the Avrrrinator, a Bus Pirate 3 to AVR ISP adapter. 

### Which should I choose?


#### [Avrrrinator Rev. A](hardware/revA)

![Avrrrinator Rev A2](hardware/revA/images/avrrinator-a2-bp.png)

Straight Bus Pirate to AVR breakout with 5v/3.3v selection. No logic level
translation. Simple and works.

#### Avrrrinator Rev. B

Soon (ETA: when Half Life 3 is released). You probably don't want to wait for this. Mostly for very specific use cases.

![Avrrrinator Rev B1](hardware/revB/images/avrrrinator-b-preview.png)

Revision B isn't a program-many-AVRs-at-once board\*, but lets you connect more than one AVR for individual programming. This is great for prototyping and flipping different bits on two identical circuits (low power projects, debugging, etc). 

\* Saying parallel would be confusing since old-school parallel programmers are out there
