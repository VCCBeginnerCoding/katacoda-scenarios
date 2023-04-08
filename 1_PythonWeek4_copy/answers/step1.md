# Module 4 part 1 Answers
## 1.
Use a WHILE loop to keep asking the user to enter a password if the password entered is not “PASSWORD”.
* Added challenge – keep a count of the number of times use enter a password and print the number of tries at the end.
```python
while True:
    password = input("Enter the password: ")
    if password == "PASSWORD":
        print("Access granted.")
        break
```
Challenge:
```python
count = 0
while True:
    password = input("Enter the password: ")
    count += 1
    if password == "PASSWORD":
        print("Access granted.")
        break
print("Number of tries: ", count)
```

## 2.
Use a WHILE loop to keep asking user to enter a score between 1 and 10.
* The loop finishes if the user enter 0.
* Use a variable called: `Total` to keep the total score.
* Print the total score at the end.
* Added Challenge:
  * Prevent the user from entering a score that is not between 1 and 10
  * At the end of the loop:
    * Print out the total score
    * The number of scores entered
    * The average Score.
    * The highest and lowest score.
    * (Hint - You might want to store these as variables and update them during the loop)

```python
total = 0
while True:
    score = int(input("Enter a score between 1 and 10 (enter 0 to finish): "))
    if score == 0:
        break
    total += score

print("Total score:", total)
```

Challenge:
```python
total = 0
count = 0
highest = 0
lowest = 10

while True:
    score = int(input("Enter a score between 1 and 10 (or 0 to finish): "))
    
    if score == 0:
        break
    elif score < 1 or score > 10:
        print("Invalid score, please enter a score between 1 and 10.")
        continue
    total += score
    count += 1
    if score > highest:
        highest = score
    if score < lowest:
        lowest = score

if count > 0:
    average = total / count
    print("Total score:", total)
    print("Number of scores entered:", count)
    print("Average score:", average)
    print("Highest score:", highest)
    print("Lowest score:", lowest)
else:
    print("No scores entered.")
```

## 3.
Copy this code to the start of your program. This will set the variable `random_number` to a random number between 1 and 100
```
import random
random_number = random.randint(1, 100)
```{{copy}}
* Use a WHILE loop to create a number guessing game where the user will try to guess the `random_number`.
* Exit the loop when the number entered is the same as the random number generated.
* Added Challenge:
    * Print out the number of tires the user needed to guess the number at the end of the game.
    * Help the user guess the random number by printing too high or too low depending on their guess.

```python
import random

random_number = random.randint(1, 100)
guess = 0

while guess != random_number:
    guess = int(input("Guess the random number (between 1 and 100): "))
    
print("Congratulations! You guessed the random bnumber
```

Challenge:
```python
import random
random_number = random.randint(1, 100)

guess = 0
count = 0

while guess != random_number:
    guess = int(input("Guess the random number (between 1 and 100): "))
    count += 1
    if guess < random_number:
        print("Too low, try again!")
    elif guess > random_number:
        print("Too high, try again!")

print("Congratulations! You guessed the random number: " + str(random_number) + " in: " + str(count) + " tries!")
```