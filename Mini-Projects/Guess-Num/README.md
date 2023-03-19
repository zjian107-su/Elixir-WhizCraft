## Guessing Game

A simple command-line guessing game implemented in Elixir. The game prompts the player to think of a number and attempts to guess it through a series of questions.

### 🥭 How to Play

1. Run the game by executing `elixir guessing_game.exs` in your terminal.

2. Think of a number within the given range.

3. The game will make a guess and display it to you.

4. Respond with "bigger" if the guess is smaller than your number, "smaller" if it's larger, or "yes" if it's correct.

5. Based on your response, the game will adjust its guess and continue until it guesses your number.

6. When the game successfully guesses your number, it will display the message "I knew I could guess your number!"

### 🍎 Implementation

The `GuessingGame` module contains functions to handle the game logic:

- `guess(a, b)`: A helper function that ensures the range is valid by swapping the values if `a` is greater than `b`.
- `guess(low, high)`: The main function that prompts the player to respond to the game's guesses. It uses recursion to continue guessing until it finds the correct number.
- `mid(low, high)`: Calculates the midpoint of the range `(low, high)`.
- `bigger(low, high)`: Adjusts the lower bound of the range based on the player's response of "bigger" and recursively calls `guess` with the updated range.
- `smaller(low, high)`: Adjusts the upper bound of the range based on the player's response of "smaller" and recursively calls `guess` with the updated range.

Enjoy playing the Guessing Game!
