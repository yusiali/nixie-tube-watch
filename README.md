# Nixie Tube Watch
## Objective: Build an analog watch from scratch using cathode ray Nixie tubes from the 1950s.

    ✦ Designed printed circuit boards to keep the form factor of the watch as compact as possible.
    ✦ Created a Qi standard charging module for the watch to charge wirelessly.
    ✦ Built the watch case using resin and CNC-cut glass.
    ✦ Programmed the time functions of the watch in C.
    
## Design Process
    ✦ It took me around half a year to design the final PCB and gather all the components I needed for the watch.
        ✦ All the parts I used are in the 'nixie-list.xlsx' file for reference.   
        ✦ 'watch-PCB.png' contains a diagram of my PCB as well.
    ✦ Initially, my watch display consisted of a small oled screen, but I quickly scrapped that idea once I found out about Nixie tubes.
    ✦ I had minimal soldering and PCB design experience before making my nixie tube watch, so I learned most of these skills on the go lol.

## Coding
    ✦ I coded the time functions in C.
        ✦ the .hex files have the code I wrote for the watch.   
        ✦ I coded on the MPLAB IDE since it has built-in MCU support is easy to use.   
        ✦ MCUs usually take hex files as code (due to memory space) so I converted my code to hex files.
    ✦ I used a 16 pin-32 pin DIP adapter to connect my PIC-16 MCU to my computer and upload the code to it.
        ✦ I worked with a PICkit 3 to transfer files from my computer to the MCU.

    
## Datasheets & Additional Info
    ✦ The xlsx file contains the list of all the components I used for the watch, including links for vendors that you can buy them from.
    ✦ Link for IN-16 Nixie Tube Datasheet: https://www.tube-tester.com/sites/nixie/dat_arch/IN-16_02.pdf
