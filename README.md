# Noughts and Crosses (Python)

A noughts and crosses (Tic-Tac-Toe as americans call it) game written in Python on VS code. You can play against a friend or a computer opponent - in the console or with clickable buttons in the bonus section of the notebook.

## Features
- Two-player mode and a vs-computer mode.
-Computer opponent that aims to take winning moves and block yours.
- Full input validation  - invalid input top the game never crashes the game.
- Session stats: games played, wins per player, draws.
-Optional interactive GUI built with ipywidgets (bonus section as the deliverable was achieved before).
## Requirements
- Python 3
-Jupyter notebook or VS code with the Jupyter extension (what the code was created wth).
-ipywidgets for the GUI cell only this can be installed with `%pip install ipywidgets`.


## HOw to play
1. Open `NoughtsandCrosses.ipynb` and run all cells.
- Choose a mode; `1` for two players and `2` to face the computer.
-On your turn, type a number 1-9 to claim that cell. A guide at the start shows which number is which cell.
- Get three in a row to win as you would expect. Type `y` if you want to play again.
-Final statistics are shown when you quit the game.
- For the clickable version, run the last cell in the bonus section.
## How it works 
- The board is a list of 9 strings called `WIN_COMBOS` holds the 8 winning lines, checked after every move.
-The computer simulates each free cell to spot wins and blocks before falling back to a random move.
- Global counters track stats across every game in a session.

## Known Limitations
-The computer only looks one move ahead, so two threats at once can easily beat it - maybe some sort of algorithm could fix this but it is beyond the scope of this mini-project.