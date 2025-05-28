# Two Player Hangman Game

## Features
- Playable by one or two human players.
- Optional computer player with basic guessing strategy.
- Customizable word list. 
- All letter guesses must be capitalized.


## How to Play (in the Terminal)

**The terminal will show the correctly guessed letters like this:**

`• • A • • `

**Bad guesses will be shown like this:**

`Bad guesses: ['J', 'L']`

**The game also shows how many bad guesses a player has made:** 

`Sarah has made 2 of 4 bad guesses`

`Computer (or second HumanPlayer) has made 0 of 4 bad guesses`

**The game will then ask the HumanPlayer:**

`Sarah, guess a letter or type a word to solve the puzzle: P`

**And then respond with either prompt:**

`There is 1 P in the word!` 

or

`Sorry, Sarah, there is no P in the word.`

**The ComputerPlayer will then take its turn, and the game alternates between players!**

**If both players run out of guesses without solving the word, this message appears:**

`The word was CHANT. Better luck next time.`

## How to Run

- Make sure you have Python 3.x installed.
- No external libraries required (only `argparse`, `re`, `sys`, and `random`).
- My program is designed to run from the terminal.
- To run it, open a terminal and ensure you are in the directory where your script and sample file are saved.


The examples below assume you are using macOS and your program is called `hangman.py` and the input file is called `nounlist.txt`.

If you are using Windows, replace `python3` with `python`.

### Command-line Argument to Run Program
 
This command-line is for two human players (replace `Sarah` and `Owen` with any names): 

`python3 hangman.py nounlist.txt Sarah Owen`

This command-line is for a one human player and the computer player: 

`python3 hangman.py nounlist.txt Sarah -c`
