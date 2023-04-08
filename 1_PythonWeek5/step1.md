# Challenges
Choose a game and either work in pairs (pair programming) or individually.

Messy Terminal? `clear`{{execute}} it.
<hr>

## 1.
Word Jumble:
* This game involves taking a word and scrambling the letters, then asking the user to unscramble the word.
* The user wins if they unscramble the word correctly.
* Can you extend the program so that the user can enter their own words before starting the game?
* Use this code to randomly jumble a word from the words list:
```python
import random

# List of words to choose from
words = ["apple", "banana", "orange", "grape", "kiwi"]

# Choose a random word
word = random.choice(words)

# Scramble the letters in the word
jumble = ""
while word:
    position = random.randrange(len(word))
    jumble += word[position]
    word = word[:position] + word[(position + 1):]
```


## 2.
Hangman
* Choose a random word from a list of words
* Show the user a series of underscores, one for each letter in the word
* Ask the user to guess a letter
* If the letter is in the word, reveal the position(s) of the letter in the underscores
* If the letter is not in the word, deduct one life from the user's total lives
* Repeat until the user guesses the word or runs out of lives
* Hint: `["_"] * len(word)` use this to generate the number of underscores for a word
* 

## 3.
Rock Paper Scissors
* Ask the user to choose rock, paper, or scissors
* Generate a random choice for the computer
* Determine the winner based on the rules of the game (rock beats scissors, scissors beat paper, paper beats rock)
* Keep track of the score and play again until the user decides to quit
* Use this code to generate a random answer from the computer:
```python
import random
game_options = ["rock", "paper", "scissors"]
computer_choice = random.choice(game_options)
```

