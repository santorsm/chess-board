# Lab 11: Numpy Arrays

[PR](https://github.com/santorsm/chess-board/pull/1)

## Overview

Construct chess boards like it’s 1980; no prebuilt images, just the power of arrays and pixel art

## Feature Tasks and Requirements

[X] render out chess boards with red and blue queens on them

[X] the only pieces are queens and each queen is represented by a blue or red square

[X] an 8 x 8 grid of alternating black and white squares; the queens are red and blue squares

[X] Each board will have one red and one blue queen at different coordinates

[X] In addition to displaying the board you’ll need to identify if the queens are “under attack” based on their coordinates

## Implementation Notes

define a `ChessBoard` class
[X] should contain an 8x8 grid - Each cell in grid should have a color represented in RGB format. - black = (0,0,0) - white = (1,1,1) - blue = (0,1,1) - red = (1,.2,0)
[X] should have `add_red` method that accepts a row and column as input which colors corresponding cell
[X] should have `add_blue` method that accepts a row and column as input which colors corresponding cell
[X] should have `render` method that displays the chess board on screen with red and blue shown in correct locations
[X] should have `is_under_attack` method that return boolean if red is under attack by a blue piece horizontally, vertically or diagonally

## User Acceptance Tests

[X] queens on same row should be “under attack”
[X] queens on same column should be “under attack”
[X] queens on same diagonal should be “under attack”
[X] queens with any other coordinates should NOT be “under attack”

**NOTE**: Include assert statements directly in your notebook verifying the behavior above

## Stretch Goal

- Enlarge the chessboard to allow for pixel art drawn pieces. 16x16 ought to be enough
- Add more attacking queens.
- Add opacity to cell colors.

## Configuration

Use `poetry` to create `chess-board` project.

**NOTE**: do NOT use `poetry new` for this project. If you did use new command the easiest thing is to delete the folder and start again with instructions below.

$ mkdir chess-board
$ cd chess-board
$ poetry init -n
$ poetry add numpy matplotlib jupyterlab
$ poetry shell
$ touch chess_board.ipynb
open chess-board folder in vscode

open chess_board.ipynb and VS Code Jupyter Server should start

Use the `chess-board` folder as the root of your project’s git repository.

## Documentation

Roger provided several pieces of useful information which have been annotated in the comments in the Jupityer Notebook

help with "UNDER ATTACK" logic from [Check if a Queen can attack a given cell on chessboard](https://www.geeksforgeeks.org/check-if-a-queen-can-attack-a-given-cell-on-chessboard/)
