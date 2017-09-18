# Tetris in C++
------------

## Overview
This is a slightly altered version of tetris build as a part of the CS 246 course at the University of Waterloo. 

This project is the final group project for the course and it was completed by Ali Sabet, Hyunjin Lee, and myself. 

Since it is part of the course work, I cannot share the entire source of the project. So instead, I will share a compiled version of the project and some documentations.

## Commands
- left/right/down: Moves the live block to the left/right/down if possible
- clockwise/counterclockwise: Rotates the block 90 degrees clockwise/counterclockwise if possible
- drop: Drops the live block (as many down as possible), this command generates the next block
- levelup: Increases the level by one, the current live block is not affected
- leveldown: Decreases the level by one, the current live block is not affected
- restart: Clears the board and score

### extra functionally
Entering the part of the command will execute the command, as long as it is not ambiguous.

For example:
- d executes drop
- cl executes clockwise
- lef executes left
- le/level executes nothing (as it can refer to levelup or leveldown)

## Note
The original project was meant for linux command line, the following functionally does not work in the windows executable file:
- level 1 and level 2 (these two levels relies on an external file passed via the command-line as they do not generate block automatically)
- Xwindows view (the optional graphical view, disabled in the windows version)
- set seed (using the command-line to set seed for the random block generator)

