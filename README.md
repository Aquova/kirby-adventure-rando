# KA-Rando

Kirby's Adventure Randomizer

An ability randomizer for Kirby's Adventure for NES.

https://github.com/Aquova/KA-Rando

Written by Austin Bricker (Aquova), 2017

https://twitter.com/Aquova__


## -- Overview --

Programs to randomize the abilities that Kirby will gain from eating enemies in Kirby's Adventure. There are three programs contained within this repository.

First is a .lua script intended to be used with FCEUX or similar lua-compatible emulator and a US ROM of Kirby's Adventure for NES.
The lua script edits the RAM in real time, ensuring a completely random ability each time an enemy is swallowed.

Secondly, there are two programs that edit the ROM, allowing it to be distributed and used with any emulator.
However, while the abilites are randomized, they are always constant within that ROM.
Ex. If a fire enemy now gives you the spark ability, ALL fire enemies will always give you the spark ability.

## -- Usage --

In addition to the files included in the repository, you will also need a US copy of the Kirby's Adventure ROM (which is left to the user to obtain). Follow the instructions in the subcategories below for your operating system/preference.

#### --- Windows ---

Run `KA-Randomize.exe`. Select the options you desire, and select the location of your .nes Kirby's Adventure file. Finish by clicking the 'Randomize' button. The randomized ROM will be saved into the same folder as the original, with the seed appended onto the end of the file name.

#### --- macOS ---

Run `KA-Randomize.app`. Select the options you desire, and select the location of your .nes Kirby's Adventure file. Finish by clicking the 'Randomize' button. The randomized ROM will be saved into the same folder as the original, with the seed appended onto the end of the file name.

#### --- Linux/Python ---

Linux users, or users who want to simply run the Python program itself, have two options.

1. If you have Python3, Qt5, and PyQt installed, you can run the following command in Terminal:

`python3 KA-Randomize.py`

This will open the same application as the PC and Mac binaries.

2. If you just have Python 3, there is a Command Line version of the program, which can be run via:

`python3 KA-Rando-Simple.py`

Make sure that your .nes file is located in the same folder as the program, then simply follow the instructions.

#### --- .Lua Compatible Emulator ---

If your emulator supports Lua scripts (such as FCEUX or Bizhawk), you are welcome to instead use the 'KirbyAbility.lua' script. This script edits the RAM in real time, allowing for complete randomization of Kirby's abilities, meaning that eating enemies of the same type may give different results. However, this script does not change Kirby's color.


## -- Version History --

v2.00 - 11/16/17 - Added GUI interface. Can now select specific Kirby color in addition to randomizing the color. Switched from Python 2 to Python 3

v1.03 - 9/2/17 - Removed need to import data from txt files. Entire program now contained in .py

v1.02 - 6/8/17 - Added option to randomize Kirby's color palette

v1.01 - 5/25/17 - Fixed issues with OS dependancy. The Python program now works on all OS's, and added an exe program for Windows users.

v1.00 - 5/24/17 - Completed the Python program. Enemy abilites are now randomized, supports options for omitting the Star Rod ability or randomizing non-ability enemies.

## -- Known Issues/Future Plans --

Dying with Star Rod disables select button until level completion

Museum enemies are not randomized

Add future support for room order

Possible support for complete color randomization, depending on demand.
