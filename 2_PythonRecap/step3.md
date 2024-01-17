# While Loops & For Loops

## While Loops
While Loops are used when you need to iterate through code an unknown amount of times.

A useful use-case for while loops is validating an input given by a user.

```python
number = float(input("Enter a number between 1 - 10 (inclusively)"))
while not (1 <= number >= 10):
  number = float(input("Please try again the number must be between 1 - 10 inclusively"))

print(f"The valid number provided is {number}")
```{{copy}}

## For Loops
For loops are useful when you need to iterate through code a known number of times, such as a fixed number or a sequence.

```python
for i in range(10):
  print(i)

for i in range(2, 11):
  print(i)

for i in range(20, 0, -2):
  print(i)

numbers = [2, 4001,89,103,120]
for number in numbers:
  print(number)

names = ["Jerry", "Rick", "Morty", "Summer", "Beth"]
for index, name in enumerate(names):
  print(index, name)

print("Name\tIQ")
for iq, name in zip(numbers, name):
  print(f"{name}\t{iq}")
```{{copy}}

# Exercise
## 1
* Define a list of names.
* Output each name in the list on a new line.

## 2
* Using a for loop iterate through the range 1 - 21.
* If the number is a multiple of 5 and 3, print the message "FizzBuzz"
* If the number is only a multiple of 3, print the message "Fizz"
* If the number is only a multiple of 5, print the message "Buzz"
* Otherwise, print the number

## 3.0
Adapt exercise 2 so that instead of using a range it will use a list of numbers instead.

### 3.1 Bonus Challenge
* Ask the user to enter a number and store that number in a list.
* Continue to keep asking the user to enter a number until they have entered the word "STOP"
* Adapt exercise 3.0 so that the FizzBuzz program runs on the list of numbers provided by the user.