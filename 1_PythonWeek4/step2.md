# For Loops
A for loop is used to iterate over a sequence. It has the following characteristics:
* Starts with the keyword "**for**"
* A variable name to store the current item in the sequence
* The keyword "**in**"
* The sequence to iterate over 

Where while loops are useful when you need to loop other code an unknown number of times. For loops are useful for repeating code a specified number of times or to iterate over a sequence.

A sequence can be a string or a list.
## Iterating Over a Sequence
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

## Range
When can use the `range()` function to loop through our code a specified number of times.
```python
for i in range(5):
  print(i)
```{{exec}}
The code above will output the value of `i` for each iteration of the loop. The range function has 3 different variations that take up to 3 parameters. You can find out more about the range function [here](https://www.w3schools.com/python/ref_func_range.asp)

Just like with while loops we can use the keyword `break` in our loop. `break` stops the loop at that point. 

We can also use `continue` command to execute the loop again from the top without running the remaining code in the loop body that is below the `continue` command.

```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
```{{copy}}

## Looping through Multiple Sequences at the Same Time
You can use the `zip()` function to iterate over multiple sequences at the same time.
```python
items = ["apples", "bananas", "carrots"]
quantities = [3, 7, 2]

for item, quantity in zip(items, quantities):
  print(f"{item}: {quantity}")
```{{exec}}
Note! If one of the sequences has more items than the other, the for loop will only iterate until all the items in the smaller sequence has been iterated.

## Enumerate
The enumerate function is useful when you need to iterate over code that requires both the value of the item and it's index position in the sequence.
```python
fruits = ["apple", "banana", "cherry"]
for index, item in enumerate(fruits):
  print(f"Fruit: {item} at index: {index}")
```{{exec}}

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
* Define a list with 5 fruit.
* By looping over the first list, create a new list that only has the items from the first list that have an even index position.

## 4.
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