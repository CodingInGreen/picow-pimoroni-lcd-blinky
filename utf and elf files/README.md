Prove that all your hardware works first

Code and output binaries here:
https://github.com/9names/picow_blinky/releases/tag/1.0.0

1) Power your pico-w with the boot2 button pressed. 
2) Mount it when asked.
3) Drag flash_nuke.uf2 on to the drive, wait a few seconds, turn it off.

4) Try attaching to it via probe-rs

probe-rs attach picow_blinky.elf --chip rp2040 --protocol swd

5) If that works, try run

probe-rs run picow_blinky.elf --chip rp2040 --protocol swd