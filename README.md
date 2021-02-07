# amiga-pi-to-hdmi

This project implements a board which plugs into a big-box Amiga Video Slot
(A2000, A3000, A4000) and uses a Raspberry Pi Zero to process the Amiga
display video in realtime to provide HDMI video output for the computer.

The schematic design is based on the Denise socket Amiga-Digital-Video module
for OCS and ECS Amigas with a 48-pin DIP Denise:
    https://github.com/c0pperdragon/Amiga-Digital-Video

It uses software for the Raspberry Pi Zero that is developed by hoglet67's
multi-platform vintage hardware RGBtoHDMI project:
    https://github.com/hoglet67/RGBtoHDMI

----------------------------------------------------------------------

This board was designed to provide a few options:
    1. The mini HDMI port of the Raspberry Pi Zero may be directly exposed
       to the rear of the computer, allowing one to plug directly into the
       Pi's video port.
    2. The Raspberry Pi Zero may be mounted in a second position which
       allows for an adapter cable so that a full size HDMI port may be
       exposed out the rear of the Amiga.
    3. A full size Raspberry Pi (such as the Pi 2 B+) may be mounted on
       the board with its HDMI port exposed on the rear of the Amiga.

That in all the scenarios above, the Raspberry Pi must be mounted to the
board face-up. This likely means that you will need to de-solder the
connector from the Pi 2 B+ and higher to solder it on the back side of
the Pi. Another option, if you are using a Pi Zero with a top side GPIO
connector already attached, is that you could mount it on the rear of the
board, and run a cable to the rear slot.
