# Sudoku

A fully-featured Sudoku game built with [CMU Graphics](https://www.cs.cmu.edu/~112/notes/notes-graphics.html) for the CMU 15-112 (Summer 2024) term project. Runs offline as a desktop app with keyboard- or mouse-only play, a backtracking solver, and a hint system (obvious singles/tuples) rather than just a bare playable grid.

## Features

- Runs offline using the desktop-installed version of CMU Graphics
- Screens: splash, menu, help, play, and game-over screens
- Randomly loads hardcoded boards from text files by type, with random transformations based on difficulty level
- Generates random boards based on selected level
- Keyboard-only and mouse-only play modes
- Automatic and manual modes for candidate ("legal") values — in manual mode, toggle shift and enter values to update a cell's legals yourself; in auto mode the board updates them for you
- Incorrect-value indicator (cell turns red when an invalid value is entered)
- Backtracking solver (with optimizations)
- Simple and complex hints: obvious singles and obvious tuples, with hint indication and apply
- Autoplayed singletons

## How to run

1. Copy the code into a folder.
2. Install CMU Graphics and required dependencies.
3. From that folder, run `python runui.py`.

## Controls

**Keyboard**
- Arrows to navigate, enter to select
- `1`–`9` to enter a number in the selected cell
- `h` to show hint, `a` to apply hint, `x` to apply singletons
- `s` to solve, `l` for auto legals, `m` for manual legals (in manual mode, `shift`+`1`–`9` adds/removes legals)
- `r` to start a new game on game over, `b` to go back

**Mouse**
- Click to select a cell
- Click to reset when the game is over
