# Module 4 Part 2 Answers:
## 1.
* Write a Python program that asks the user to enter an integer and counts the number of digits in the integer.
* Use a for loop to iterate through each digit in the integer.
* Print the total count of digits in the integer.
```python
num = int(input("Enter an integer: "))
count = 0
for digit in str(num):
    count += 1
print("Total number of digits:", count)
```

## 2.
* Write a Python program that asks the user to enter a string and prints the reverse of the string.
* Use a for loop to iterate through each character in the string.
* Challenge, can you detect a palindrome? This is where the word is the same when reversed e.g. noon
   * If the word entered is a palindrome, let the user know!
```python
string = input("Enter a string: ")
reverse = ""
for char in string:
    reverse = char + reverse
print("Reverse of the string:", reverse)
```

Challenge:
```python
string = input("Enter a string: ")
reverse = ""
for char in string:
    reverse = char + reverse

print("Reverse of the string:", reverse)

if string == reverse:
    print("The string is a palindrome!")
else:
    print("The string is not a palindrome.")
```

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

```python
import random
number = random.randint(1, 20)
for i in range(3):
    guess = int(input("Guess a number between 1 and 20: "))
    if guess == number:
        print("Congratulations! You guessed the number.")
        break
else:
    print("Sorry, you didn't guess the number. The number was: " + str(number) + ".")
```

Challenge:
```python
import random

start = int(input("Enter the starting number: "))
end = int(input("Enter the ending number: "))
number = random.randint(start, end)

guesses = int(input("How many guesses do you want? "))
for i in range(guesses):
    guess = int(input("Guess a number between " + str(start) + " and " + str(end) + " : "))
    if guess == number:
        print("Congratulations! You guessed the number.")
        break
    else:
        print("Sorry, that was incorrect.")
else:
    print("Sorry, you didn't guess the number. The number was " + str(number) + ".")
```