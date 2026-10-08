# Guess the Number Game

A simple and interactive Python game where you try to guess a randomly generated number. Test your luck and strategy across three difficulty levels!

## About the Game

In this game, the computer thinks of a secret number, and your goal is to guess it before running out of attempts. After each guess, you'll receive a hint telling you if your guess is too high or too low. The game tracks your wins, losses, and total score across multiple rounds.

## Features

- **Three Difficulty Levels:**
  - Easy: Numbers 0-10, 10 attempts, 1 point per win
  - Medium: Numbers 0-20, 6 attempts, 3 points per win
  - Hard: Numbers 0-30, 4 attempts, 5 points per win

- **Game Statistics:** Tracks wins, losses, total games played, and cumulative score
- **Input Validation:** All user inputs are validated to prevent errors
- **Helpful Feedback:** After each guess, you'll see if your guess is too high or too low, and how many attempts remain
- **Multiple Rounds:** Play as many times as you want in one session

## How to Play

1. Run the game (see instructions below)
2. The game will display a welcome message and explain the rules
3. Choose a difficulty level (easy, medium, or hard)
4. The computer will generate a random number
5. Enter your guess (a number)
6. The game will tell you if your guess is too high or too low
7. Keep guessing until you find the correct number or run out of attempts
8. After each game, choose to play again or quit
9. View your final statistics when you exit

## Requirements

- Python 3.6 or higher
- Jupyter Notebook (to run the `.ipynb` file)

## How to Run

Open the `StefanSavic_Python_FirstGameProject_Code.ipynb` file in Jupyter Notebook and run the cells to start playing the game.

## Code Structure

The game is organized into the following functions:

- **`random_num_generator(min_range, max_range)`** - Generates a random number within the specified range
- **`user_input_guess()`** - Gets and validates the player's guess
- **`select_difficulty()`** - Allows the player to choose a difficulty level
- **`play_game()`** - Main game logic for one complete round

### Global Variables

- `wins` - Counts total games won
- `losses` - Counts total games lost
- `total_games` - Counts total games played
- `total_score` - Tracks cumulative points earned

## Example Gameplay

```
Welcome to Guess the Number!
Select a difficulty, guess the secret number, and try to get it right before you run out of attempts!
Hints: 'lower' = too high, 'higher' = too low

Do you want to play Guess the Number? (yes/no): yes
Available difficulties: dict_keys(['easy', 'medium', 'hard'])
please chose a difficulty: easy
Dev test: randomly generated target number: 7

please enter a number: 5
higher - try again Attempts remaining: 9
please enter a number: 8
lower - try again Attempts remaining: 8
please enter a number: 7
correct
You earned 1 points!

Do you want to play again? (yes/no): no
Thanks for playing!

Wins: 1, Losses: 0, Total: 1, Score: 1
```

## Project Features

This project demonstrates key Python concepts:

- **Functions** - Modular code organization
- **Global Variables** - Tracking state across function calls
- **Input Validation** - Error handling with try/except blocks
- **Loops** - While loops for game rounds and input validation
- **Conditional Statements** - If/elif/else for game logic
- **String Formatting** - f-strings for user-friendly output
- **Dictionaries** - Organizing difficulty settings
- **Documentation** - Docstrings and comments explaining code

## Author

Stefan Savic

## Project Conclusion

This game was created as part of a Python learning project. It fulfills the following requirements:

-  Psudocode of game logic
-  Well-organized functions with docstrings
-  Input validation for all user entries
-  Global counters for statistics
-  Clear code with comments and documentation
-  README file with complete instructions

## Notes

- The game includes a temporary debug message showing the target number (for testing purposes)
- Remove or comment out the debug print statement if desired for actual gameplay
- The game uses Jupyter's `clear_output()` to keep the display clean between rounds

---

Enjoy the game and happy guessing!
