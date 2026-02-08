# 📘 Assignment: Hangman Game Challenge

## 🎯 Objective

Build a command-line Hangman game in Python to practice string manipulation, loops, conditionals, and user input handling. Students will implement game logic, track game state, and provide clear user feedback.

## 📝 Tasks

### 🛠️ Core Game Mechanics

#### Description
Implement the core Hangman game: randomly choose a word from a predefined list, accept single-letter guesses, reveal correct letters in the word, and track remaining attempts until the player wins or loses.

#### Requirements
Completed program should:
- Use a predefined list of words and select one at random.
- Accept single-letter input and validate it (ignore invalid or repeated inputs).
- Display current progress in "_ _ a _ _" format with spaces between characters.
- Track and display remaining incorrect attempts (e.g., 6 attempts).
- End the game with a clear win message when all letters are revealed or a lose message when attempts reach zero.
- Keep a visible list of incorrect letters guessed.

Example input/output:
```text
Welcome to Hangman!
Word: _ _ _ _ _
Guess a letter: a
Correct! Word: _ a _ _ _
Incorrect guesses left: 6
Guess a letter: z
Wrong. Wrong letters: z
Incorrect guesses left: 5
...
```

### 🛠️ Enhancements and User Experience

#### Description
Add optional features that improve usability and code quality: difficulty levels, replay option, and modular code structure.

#### Requirements
Completed program should:
- Provide at least two difficulty options (e.g., Easy = 8 attempts, Hard = 5 attempts).
- Offer a "Play again?" prompt after game end and correctly restart or exit.
- Display wrong guesses and remaining attempts each turn.
- Organize code into functions (e.g., choose_word(), display_progress(), handle_guess(), main()) and include brief inline comments.
- (Optional) Persist a simple high-score or stats file recording wins/losses across sessions.
