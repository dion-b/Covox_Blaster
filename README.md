# Covox_Blaster
A Covox Speech Thing clone that plugs straight into a parallel header

The Covox Speech Thing is arguably the simplest piece of sound hardware created for the PC, consisting of little more than a resistor ladder DAC and a rudimentary low-pass filter. Because of its relative rarity and extreme simplicity there are already many clone designs. The fact that the patent for the Speech Thing contains a full schematic no doubt helps as well. These clones range from extremely minimal homebrew designs to some commercial sound cards (most notably Aztech Technologies' first generation Soundblaster Pro clones) integrating the functionality.

So, why a new clone? A defining feature of the Speech Thing, and of all common clones not integrated into a sound card/chip is that they are an external design, interfacing with the parallel port of the PC. This means it can be installed without opening the PC case, and can be used on systems with no internal expansion slots. Great. But it also leads to a messy, vulnerable thing sticking out of the back of the PC. If the PC in an internal parallel headers, it should be possible to design a small daughterboard stuck straight into the parallel header. This design is an attempt to do so.

The design is a modified version of my earlier Internal Covox (https://github.com/dion-b/Internal-covox), which was in turn strongly inspired by Serdaco's CVX4 exernal device (available here: https://www.serdashop.com/CVX4) - which is arguably the best clone you can buy at this time. Where the previous design sits on a backplate and connects to the parallel header via a flatcable, this card simply plugs into the header, with a standard MPC-2 connector for audio-out to connect it to the CD audio header on a sound card, or anything else (and external jack).

This setup brings a number of advantages:
- reduced cost; the backplate was the most expensive part of the previous design, the custom flatcable the second most expensive.
- improved fidelity; due to a layout error the previous design required very small resistors which are only available/affordable with 1% tolerance. This design allows the use of standard 0.1% resistors.
- increased flexibility; that MPC-2 cable can be hooked up to a lot more than just sound cards.

One PCB design is suitable for both card-mounted parallel headers (use a straight female 2x13 2.54mm connector) and board mounted ones (use a 90 degree angled female 2x13 2.54mm connector).
