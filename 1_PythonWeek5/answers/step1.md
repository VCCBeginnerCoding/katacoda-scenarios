# Module 5 part 1 Answers

## 1.
Word Jumble:
* This game involves taking a word and scrambling the letters, then asking the user to unscramble the word.
* The user wins if they unscramble the word correctly.
```python
import random

# List of words to choose from
words = ["apple", "banana", "orange", "grape", "kiwi"]

# Ask the user to add their own words
while True:
    add_words = input("Do you want to add your own words? (y/n) ").lower()
    if add_words == "y":
        new_word = input("Enter a new word: ")
        words.append(new_word)
    elif add_words == "n":
        break
    else:
        print("Invalid input. Please enter 'y' or 'n'.")

# Choose a random word
word = random.choice(words)

# Scramble the letters in the word
jumble = ""
while word:
    position = random.randrange(len(word))
    jumble += word[position]
    word = word[:position] + word[(position + 1):]

# Welcome message and instructions
print("Welcome to Word Jumble!")
print("Unscramble the letters to make a word.")
print("Enter 'quit' to quit the game.")

# Game loop
while True:
    print("The jumbled word is:", jumble)
    guess = input("Enter your guess: ").lower()

    # Check if the user wants to quit
    if guess == "quit":
        break

    # Check if the guess is correct
    if guess == word:
        print("Correct! You win!")
        break
    else:
        print("Sorry, that's not correct. Try again.")
```

## 2.
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
```python
import random

# Define the game options
game_options = ["rock", "paper", "scissors"]

# Set the initial score to 0
user_score = 0
computer_score = 0

# Play the game until the user decides to quit
while True:
  # Ask the user to choose rock, paper, or scissors
  user_choice = input("Choose rock, paper, or scissors (or q to quit): ")

  # If the user chooses to quit, end the game
  if user_choice.lower() == "q":
    print("Final score: User:", user_score, "Computer:", computer_score)
    break

  # Generate a random choice for the computer
  computer_choice = random.choice(game_options)
  print("Computer chooses", computer_choice)

  # Determine the winner based on the rules of the game
  if user_choice.lower() == "rock":
    if computer_choice == "scissors":
      print("You win!")
      user_score += 1
    elif computer_choice == "paper":
      print("Computer wins!")
      computer_score += 1
    else:
      print("It's a tie!")
  elif user_choice.lower() == "paper":
    if computer_choice == "rock":
      print("You win!")
      user_score += 1
    elif computer_choice == "scissors":
      print("Computer wins!")
      computer_score += 1
    else:
      print("It's a tie!")
  elif user_choice.lower() == "scissors":
    if computer_choice == "paper":
      print("You win!")
      user_score += 1
    elif computer_choice == "rock":
      print("Computer wins!")
      computer_score += 1
    else:
      print("It's a tie!")
  else:
    print("Invalid input. Please try again.")

  # Print the current score
  print("Score: User:", user_score, "Computer:", computer_score)

```

## 3.
Hangman
* Choose a random word from a list of words
* Show the user a series of underscores, one for each letter in the word
* Ask the user to guess a letter
* If the letter is in the word, reveal the position(s) of the letter in the underscores
* If the letter is not in the word, deduct one life from the user's total lives
* Repeat until the user guesses the word or runs out of lives
```python
import random

# Define a list of words to choose from
word_list = ["python", "java", "javascript", "ruby", "php"]

# Choose a random word from the list
word = random.choice(word_list)

# Create a list of underscores, one for each letter in the word
underscores = ["_"] * len(word)

# Set the number of lives for the player
lives = 6

# Play the game until the player guesses the word or runs out of lives
while lives > 0:
    # Print the current state of the underscores
    print(" ".join(underscores))

    # Ask the player to guess a letter
    guess = input("Guess a letter: ")

    # Check if the guessed letter is in the word
    found_letter = False
    for i in range(len(word)):
        if word[i] == guess:
            # If the guessed letter is in the word, reveal the position(s) of the letter in the underscores
            underscores[i] = guess
            found_letter = True

    if not found_letter:
        # If the guessed letter is not in the word, deduct one life from the player's total lives
        lives -= 1
        print("Sorry, that letter is not in the word. You have", lives, "lives left.")

    # Check if the player has guessed all the letters in the word
    if "_" not in underscores:
        print("You win! The word was", word)
        break

# If the player runs out of lives, they lose the game
if lives == 0:
    print("You lose! The word was", word)

```