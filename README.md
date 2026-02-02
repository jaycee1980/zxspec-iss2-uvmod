# ZX Spectrum Issue Two UV Mod

This is a a small modification board to add the autobias circuit for the U and V video signals, present in Issue 3 and later Spectrums, to an Issue 2 Spectrum.

It eliminates the annoying VR1 and VR2 trimmer potentiometers, and thus the need to "tune" the signal for a correct colour picture. This helps enormously as these settings often drift with temperature, and can drift with aging of the ULA. Some ULA's become impossible to "tune" as they age.

Additional thanks to Jim Smith of [Happy Little Diodes](https://www.youtube.com/c/HappyLittleDiodes) as he helped me develop this board. The original inspiration came from [one of his videos](https://www.youtube.com/watch?v=m4PCPcdD4Uw) and after watching it I wondered how do-able it was to adapt an Issue 2 board to use the autobias circuit from the Issue 3 and later, and whether it would help with the "untunaeable" ULA he had in the video.

I proposed prototyping a modification using a circuit on Veroboard, and he tested this out [here](https://www.youtube.com/watch?v=yTBOfa4Heks), including an early revision of the modification board. We revised it a bit so it was neater and easier to fit, and this is the result :)

In [this](https://www.youtube.com/watch?v=-wrouM9OnbY) video Jim shows the final version of the mod board fitted, including the ordering process with [PCBWay](https://www.pcbway.com)

# How to install it

* Solder some wires to the GND, 5V and Y terminals of the mod board PCB
* Remove R38, R39, R40, R41, R56, R63, C52, C53, VR1, VR2 from the Spectrum PCB
* Fit a 470 Ohm 1/4 watt resistor between the right hand terminal of R41, and a +5V supply. Refer to the picture below to see the recommended fitting.

![Placement of the 470 ohm resistor](/pictures/new%20R40.jpg)

* Fit some 2.54mm pitch header pins to the PCB, in the right hand holes where C52, R56, C53 and R63 were fitted (see picture)

![Placement of the pin headers and where to get 5V and Y](/pictures/pin%20headers.jpg)

* Fit the mod board so the header pins go through the appropriate holes on the mod board, and solder in place.
* Solder the wires to the Spectrum PCB to make the appropriate connections. GND can be found on the R63's left hand pad. 5V can be found on the bottom leg of the large 15 ohm resistor next to the ULA, and Y can be found on the Y link underneath the LM1889. Alternatively see the picture above for holes which carry the appropriate signals. You will need to remove some soldermask on the underside of the board if you use those.

The final result should look much like this:
![Fitted mod PCB](/pictures/mod%20fitted.jpg)

# What's included here

Here you will find the EAGLE project files, a schematic, Gerber files, and BOM+CPL files for use with [JLCPCB](https://jlcpcb.com)'s self assembly service.

# Getting PCBs
Jim has a [PCBWay Shared Project](https://www.pcbway.com/project/shareproject/ZX_Spectrum_Issue_Two_UV_Mod_ba1552a4.html)

You can also have them made by [JLCPCB](https://jlcpcb.com) using the BOM, CPL and Gerber files provided

![New mod PCBs](/pictures/built%20pcbs.jpg)

# License

This project is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike (CC BY-NC-SA)](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.

I am not responsible for any Spectrums damaged due to fitting this mod!

If you want to sell prebuilt PCB's on your retro store, please contact me. I will normally grant this provided they are sold for reasonable cost. 
