# Chip8Mini

## Introduction

Chip8mini is a CHIP-8 emulator that runs inside the game cabinet.  
The focus is on pixel art in game cabinets.
[Dev notes](https://github.com/jay-kumogata/Chip8Mini/blob/main/doc/220610_DevNotes.md) here.

![](https://github.com/jay-kumogata/Chip8Mini/blob/main/screenshots/amabie08.gif)
![](https://github.com/jay-kumogata/Chip8Mini/blob/main/screenshots/breakout01.gif)
![](https://github.com/jay-kumogata/Chip8Mini/blob/main/screenshots/snake02.gif)
![](https://github.com/jay-kumogata/Chip8Mini/blob/main/screenshots/mastermind01.gif)
![](https://github.com/jay-kumogata/Chip8Mini/blob/main/screenshots/neon01.gif)

## How to Play

- (a) Install the Python3.8 (python-3.8.9.exe), which can be obtained from [here](https://www.python.org/downloads/)
- (b) Install the Pyxel1.7.0 on Python from the command line:  
  - C> pip install pyxel
- (c) Download a sample game (amabie.ch8), which can be obtained from [here](https://github.com/jay-kumogata/PyxelChip8/tree/main/games/amabie)
- (d) From the command line, run:
  - C> python Chip8Mini.py \<ROM file name\>
  - Example: C> python Chip8Mini.py amabie.ch8
- (e) Click [x] when finished

## How to control
  
The keys are mapped as follows.
  
	Original |1|2|3|C| Mapping to |1|2|3|4|
	         |4|5|6|D|            |Q|W|E|R|
	         |7|8|9|E|            |A|S|D|F|
	         |A|0|B|F|            |Z|X|C|V|

## Specification
### Memory
- RAM (200H - F10H)
- Hexadecimal font (F10H -F60H)

### Registers
- Data Registers (V0 .. VF)
- Address Registers (I)
- Timers (Delay and Sound)
- Stack (16 word length and stack pointer)

### Graphics
- Sprite (CHIP-8 Mode: 8 x 1 .. 15)
- Collision Flag
- Hexadecimal font
  
### Instruction set
- CHIP-8 instructions (assignment, arithmetic, conditional branch, subroutine call, draw sprite, etc.)

### Keyboard
- Hexadecimal keyboard
