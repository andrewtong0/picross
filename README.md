# Picross

A recreation of classic puzzle game "Picross" in GM: Studio version 1.4.1763. The majority of the game is handled within the obj_handler object. (Accessible through file directory - re_picross/Picross.gmx/objects/obj_handler.object.gmx - note that lines 1 - 27 are automatically generated within the game engine. There are also some additional lines strung throughout the code that are native to the program that do not display the same as within GM: Studio.

The puzzle generation is modular and can be expanded infinitely, assuming the computer is capable of both displaying and handling your grid specifications. The grid generation is handled in individual line array declaration (which should be in a double for loop instead - one for each dimension), but I haven't gotten around to doing that yet.

Note that while I list plans within the patch notes, there is no guarantee if I will ever get around to troubleshooting the problems.

Patch Notes:
August 9, 2017
// Current Version
- Keybinds are 'R' to clear and generate a new puzzle, and 'C' to clear the current board without generating a new puzzle.
- Currently puzzle generation is random, hence the array generation with random integers from ceiling integer 1, where 1 indicates the presence of a filled square, and 0 as an empty square. Unfortunately, this means that some generated puzzles may have ambiguous solutions, but due to having only one explicit solution, only one of the ambigious solutions currently works.
// Plans
- Create preset levels (preferably as images to add a bit of excitement).
- Improve the general UI of the game.
- If possible, find a way to negate ambiguous puzzles in random generation.
