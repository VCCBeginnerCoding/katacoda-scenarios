# For Loops
A for loop is used to iterate over a sequence. It has the following characteristics:
* Starts with the keyword "**for**"
* A variable name to store the current item in the sequence
* The keyword "**in**"
* The sequence to iterate over 

The sequence can be a string or a list

```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
print("I have finished the loop")
```{{copy}}

You can also use loops to iterate through a string:

```
for x in "banana":
  print(x)
```{{copy}}

Just like with while loops we can use the keyword `break` in oour loop. `break` stops the loop at that point. 

We can also use `continue` command to execute the loop again from the top without running the remaining code in the loop body that is below the `continue` command.

```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```{{copy}}

# Exercises:
## 1.
* Write a Python program that asks the user to enter an integer and counts the number of digits in the integer.
* Use a for loop to iterate through each digit in the integer.
* Print the total count of digits in the integer.

## 2.
* Write a Python program that asks the user to enter a string and prints the reverse of the string.
* Use a for loop to iterate through each character in the string.
* Challenge, can you detect a palindrome? This is where the word is the same when reversed e.g. noon
  * If the word entered is a palindrome, let the user know!

## 3.
Copy the code below to the start of your python program to generate a random number between 1 and 20:
```
import random
random_number = random.randint(1, 20)
```{{copy}} 
* Use a for loop to give the user three attempts to guess the number.
* If the user guesses the number correctly, print "Congratulations! You guessed the number."
* Otherwise, print "Sorry, you didn't guess the number. The number was X." where X is the randomly generated number.
* Challenge, before the game starts:
  * Ask the user to enter a starting and ending number, generate the random number based on the users starting and ending number
  * Ask the user how many guesses they would like to have, only let them enter this number of guesses
  

# You have completed part 2

Kahoot time!!!