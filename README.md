# Electrolytes

A Pro Micro based 4x10 ortholinear PCB that's compatible with the Yasui by [rainkeebs](https://github.com/rainkeebs).

Special thanks to [rlbaxter](https://github.com/rlbaxter) for the original [Electrolyte](https://github.com/rlbaxter/electrolyte) and for some ideas present in this PCB.

Some great cases that fit this PCB are the [Umō](https://github.com/pohjolaworks/Umo) by [PohjolaWorks](https://github.com/pohjolaworks) and the case by HaiZeus#0411.

The firmware is currently a work-in-progress.

## Layout and Renders

This PCB supports the all the R2 Yasui layouts as well as some more symmetrical layouts (Centered 4u, MechVault Split, etc.). OLED and RGB breakouts are provided if they are wanted as well a position for a rotary encoder in the bottom left. The KLE can be found [here](http://www.keyboard-layout-editor.com/#/gists/fb9aadbc1251c487f24355c8019214f2).

![Layout](/rev%202.0/Images/keyboard-layout.png)
![Front](/rev%202.0/Images/front.png)
![Back](/rev%202.0/Images/back.png)

## Ordering

Current Status: **Untested** (***Order at your own risk!***)

BOM and CPL files are included in the repository, provided you want the SMD components pre-soldered by the fabricator, but if you are going to order it bare, you will need the following to make it functional:

- Required Components:
  - 31-40 MX Switches (Layout Dependent)
  - Pro-Micro (Drop-in)
  - 2 1x13 Controller Sockets
  - 40 SOD-123 Diodes
- Optional Components:
  - Reset Button

## Notes

- **The current revision (2.0) has two jumpers that need to be soldered for the matrix to be completed as this was done was as a no via challenge.**
- Cut out the _33 and 0.5u WKL layouts to fix the shorting of the original.
- A reset button was added to match the original Yasui, compared to the jumper of revision 1.0.
- The aRGB breakout was moved to near the Pro Micro in hopes that it would make soldering two rows of strips easier.
- A battery breakout was placed on the PCB so a full 1x13 pin header can be installed.
- Flex cuts were removed as they were a hindrance and was to gain PCB routing experience in that aspect.
- Slightly updated the edge cuts and tray-mount hole locations to make it a one-to-one match with the R2 Yasui Plate.
- Flipped the switch right under the Pro Micro USB to account for drop-in Pro Micros that have a USB-C that is not mid-mounted.
- Plating was added to the bottom stabilizer holes so GND can't be accidentally shorted when using screw-in stabilizers.
- The libraries used for this project are my own and [marbastlib](https://github.com/ebastler/marbastlib).
- You need at least KiCad 7 to open the source files.
