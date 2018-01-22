### TIC TAC TOE

  A second version of the game tic tac toe using different logic and minimax to make it unbeatable

## How to play
  * Clone the git repository and change into its directory.
  * In the terminal run ``` ruby tic-tac-toe.rb```
  * You will be prompted to choose 'x' or 'o'.
  * You will be prompted to choose a position from the options.
    - top left
    - top middle
    - top right
    - middle left
    - middle middle
    - middle right
    - bottom left
    - bottom middle
    - bottom right
  * After you make a move, the computer will make a move until the game is over.

## Implementation
Board: initializes a new game of 3X3 cells, is responsible for setting and getting of values for the grid and deciding win, lose or draw

Cell: writes O or X  as per player input

Game: has responsibility of Board and Players - each make move and counter move

Player: has responsibility of the names of 2 players and corresponding inputs of 'X' and 'O'

Winning combinations

The Board is represented as an array of of 3 nested arrays of (0 to 8)indices. The WINNING COMBINATIONS are a constant, so as the board knows which combinations are a winner.

As player you will be prompted to make a move. The move options are

```
2.4.0 :001 > example_array = [
2.4.0 :002 >     [1, 2, 3],
2.4.0 :003 >     [4, 5, 6],
2.4.0 :004 >     [7, 8, 9]
2.4.0 :005?>   ]
=> [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
so example_array[0][1] => 2
```
The ```winner?``` is true if WINNING COMBINATIONS values match and are a "String".
