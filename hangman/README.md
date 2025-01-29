# Hangman - Coding Task

## Overview
**Hangman** is a classic word-guessing game where players attempt to guess a hidden word by suggesting letters. If the player makes too many incorrect guesses, they lose the game.

## Task Description
The goal is to implement a **text-based** version of Hangman. The game should:
- Select a **random word** from a predefined list.
- Display the **partially guessed word**, replacing unknown letters with `_`.
- Allow the player to **guess one letter at a time**.
- Keep track of **incorrect guesses** and limit them to a set number (e.g., 6).
- End the game when the player either **guesses the word correctly** or **exceeds the maximum wrong guesses**.

## Example Game Flow

```
# Game starts
Hidden word: _ _ _ _ _  
Incorrect guesses left: 6  

> Guess a letter: e

Hidden word: _ _ e _ _  
Incorrect guesses left: 6  

> Guess a letter: x

Hidden word: _ e _ _ _  
Incorrect guesses left: 5  

> Guess a letter: l

Hidden word: _ e l l _  
Incorrect guesses left: 5  

> Guess a letter: h

Hidden word: h e l l _  
Incorrect guesses left: 5  

> Guess a letter: l (already guessed)

Invalid input. Try again.

> Guess a letter: o

Hidden word: h e l l o  
Congratulations! You guessed the word.
```

## Requirements
- The game should be **playable via the command line**.
- The word list can be hardcoded into the script.
- The game should **handle duplicate guesses gracefully** (e.g., show a warning but don’t penalize the player).
- The game should display the **current state of the word** after each guess.
- The game should track and display **remaining incorrect guesses**.
- Implement **basic input validation** (e.g., ignore numbers, special characters, and empty input).

## Word List
Use the following predefined list of words for the game:
```
word_list = ["python", "developer", "hangman", "keyboard", "monitor", "laptop", "program", "terminal", "function", "variable"]
```

## Constraints
- The words will only contain **lowercase letters** (no spaces or special characters).
- The game should allow **exactly 6 incorrect guesses** before ending.
- No UI framework should be used – it should be fully text-based.

## Expected Input/Output
Example function signature:
```python
hangman()
```

## Expected behavior:
- The game starts with a random word from a predefined list.
- The player is prompted to guess letters.
- The game displays feedback after each guess.
- The game ends when the player wins or reaches the max incorrect attempts.
