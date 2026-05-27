# Nixie Tube Watch
![nixieWatch](https://github.com/user-attachments/assets/fd05f7c0-7c1e-4064-a6ba-4a5cfec3e1ec)

## Objective: Build an analog watch from scratch using cathode ray Nixie tubes from the 1950s.

- Sourced compact custom PCBs designed by [@valendorn](https://www.youtube.com/@valendorn) to keep the form factor of the watch as small as possible.
- Assembled the watch case using resin and CNC-cut glass.
- Flashed the time-keeping firmware (written in C) onto the watch's PIC-16 MCU.

## Build Process
- It took me around half a year to source the PCBs, gather all the components, and assemble the watch.
    - All the parts I used are in the 'nixie-list.xlsx' file for reference.
    - 'watch-PCB.png' contains a diagram of the PCB I worked from.
- Initially, my watch display consisted of a small OLED screen, but I quickly scrapped that idea once I found out about Nixie tubes.
- I had minimal soldering and electronics-assembly experience before making my Nixie tube watch, so I learned most of these skills on the go lol.

## Firmware
- The watch runs time-keeping firmware written in C on a PIC-16 MCU. I didn't author the firmware — credit goes to the original author; I'm including it here so the build is reproducible.
    - The `.hex` files contain the compiled firmware for the watch.
    - The firmware was compiled using the MPLAB IDE for its built-in PIC MCU support.
    - PIC MCUs are flashed with `.hex` files (due to limited memory space), so the C source is compiled down to hex before upload.
- I used a 16-pin to 32-pin DIP adapter to connect my PIC-16 MCU to my computer and flash the firmware.
    - I worked with a PICkit 3 to transfer the hex file from my computer to the MCU.

## Credits
- **PCB design:** [@valendorn](https://www.youtube.com/@valendorn) — the entire PCB layout and schematic for this watch is his work. This build wouldn't have been possible without it.
- **Firmware:** PIC-16 time-keeping firmware in this repo was not written by me; I used it as-is to drive the watch.

## Datasheets & Additional Info
- [YT video explaining my build process and the science behind Nixie tubes](https://www.youtube.com/watch?v=iHFu8EpVipM&t=4s)
- [The excel file](/nixie-list.xlsx) contains the list of all the components I used for the watch, including links for vendors that you can buy them from.
- [IN-16 Nixie Tube Datasheet](https://www.tube-tester.com/sites/nixie/dat_arch/IN-16_02.pdf).
