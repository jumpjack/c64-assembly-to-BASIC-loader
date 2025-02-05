# BASIC V2 Machine Language loader

I added to the original 6502 compiler a button to create a BASIC loader,
which loads in memory all the needed data; then you will be able to copy
the program and paste it into  VICE emulator with ALT+INS.

You can launch the ML program using the SYS command suggested by the loader itself.

- [Original page](https://jumpjack.github.io/c64-assembly-to-BASIC-loader)
- [With BASIC loader creator](https://jumpjack.github.io/c64-assembly-to-BASIC-loade/index-my.html)

I also fixed a bug which always showed dump and disassembly starting from $0600: now they start from address specified in "* = $xxxx" directive.

## Emulator memory map

Memory locations $200 to $5ff map to the screen pixels (1024 of them). The screen is 32 x 32 pixels in size. Different values wil draw different colour pixels.
