
# 📘 Assignment: Hangman Game Challenge

## 🎯 Objective

Build a classic Hangman game in Python that uses strings, loops, and user input to create an interactive word-guessing experience.

## 📝 Tasks

### 🛠️ Set Up the Game Word

#### Description
Create a list of words and randomly choose one for the player to guess. Prepare the game state so the player sees blanks for each letter.

#### Requirements
Completed program should:

- Use a predefined list of words
- Randomly select one word at the start of each round
- Display underscores or blanks for each letter in the word
- Keep the hidden word and guessed letters organized in a simple game state

### 🛠️ Accept Guesses and Track Progress

#### Description
Prompt the player to input letters and update the visible word after each guess.

#### Requirements
Completed program should:

- Ask the user for one letter at a time
- Check whether the letter is in the secret word
- Reveal correctly guessed letters in the current progress display
- Keep a record of letters already guessed
- Show a message when a guess is repeated or incorrect

### 🛠️ End the Game

#### Description
Continue the game until the player either wins or runs out of attempts.

#### Requirements
Completed program should:

- Track the number of incorrect guesses remaining
- End the game when the word is fully guessed
- End the game when the player has no attempts left
- Display a clear win or lose message at the end
