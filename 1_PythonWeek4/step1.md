# While Loops
Messy Terminal? `clear`{{execute}} it.
<hr>

There are two main form of loops in Python. The For loop and the While loop!
We're going to spend this session focusing on while loops.  
They have these characteristics:
* Start with the keyword **while**
* Use a condition to determine if the program should continue to loop
* The condition is followed by a **:**
* The body of the loop is indented by +1 tab (4 spaces)
* A main body of the loop that contains code that will be executed each time the program loops

While loops execute a set of statements as long as a condition(s) is met:

What will happen in each of the following programs?
```
i = 1
while i < 3:
    print(i)
    i += 1
print("loop has finished")
```{{copy}}

```
i = 1
while i <= 3:
    print(i)
    i += 1
```{{copy}}

```
i = 1
while i == 3:
    print(i)
    i += 1
```{{copy}}

```
i = 1
while True:
    print(i)
    i += 1
```{{copy}}

## Keywords:
Within the body of the loop we have the following keywords we can use in our code:
* continue - stop at the current line of code and go back to the top of the loop body
* break - break out of the loop regardless of if the condition is still true or not

```
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
```{{copy}}

```
i = 0
while i < 6:
    i += 1
    if i == 3:
        break
    print(i)
```{{copy}}

# Exercises:
## 1.
Use a WHILE loop to keep asking the user to enter a password if the password entered is not “PASSWORD”.
* Added challenge – keep a count of the number of times a user enters a password and print the number of tries at the end.

## 2.
Use a WHILE loop to keep asking the user to enter a score between 1 and 10.
* The loop finishes if the user enters 0.
* Use a variable called `total` to keep the total score.
* Print the total score at the end.
* Added Challenge:
  * If the number entered is not between 1 and 10, tell the user it needs to be between 1 and 10 and to try again
  * At the end of the loop:
    * Print out the total score
    * The number of scores entered
    * The average score.
    * The highest and lowest score.
    * (Hint - You might want to store these as variables and update them during the loop)


## 3.
Copy this code to the start of your program. This will set the variable `random_number` to a random number between 1 and 100
```
import random
random_number = random.randint(1, 100)
```{{copy}}
* Use a WHILE loop to create a number guessing game where the user will try to guess the `random_number`.
* Exit the loop when the number entered is the same as the random number generated.
* Added Challenge:
    * Print out the number of tries the user needed to guess the number at the end of the game.
    * Help the user guess the random number by printing “too high” or “too low” depending on their guess. 
