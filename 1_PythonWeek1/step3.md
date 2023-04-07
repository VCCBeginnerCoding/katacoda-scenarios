# Numbers

Python supports three types of numbers – `int`, `float`, and `complex`. Integers do not have a decimal point, while floats do. Complex is mostly used in geometry and scientific calculations (so ignore them for now). You can also convert numbers into strings, which Python will treat as text (so no more multiplications afterwards).

*Integer and float*
```
a = 4
b = 4.0
print(a+b)
```{{exec}}

*Float printed out as an integer*
```
a = 4.2
print(a)
print(int(a))
```{{exec}}

*Integer printed out as a float*
```
a = 4
print(a)
print(float(a))
```{{exec}}


If you want a user to enter a number that you can then manipulate in Python (for example, multiplying the user's age by 5) you'll want to make sure that Python understands it's a number instead of a string. After all, you can't do maths on text/string.

`input()` will return what Python "thinks" is best, but you can tell Python exactly what variable type you want by doing the following:

```
number = int(input("Enter a number"))
print(number)
```{{exec}}

<hr>

# Text
You already know the variable type for text - it's `string`.

<hr>

# Other Data Types
There are many more data types that you'll learn about in future lessons, many of which will take the knowledge from this session and find practical day to day uses for them.

<hr>

# Practical Uses
Floating-point real numbers can't be represented with exact precision due to hardware limitations, so `print(0.1 + 0.2)` gives 
```
print(0.1 + 0.2)
-> 0.30000000000000004
```
This is obviously not entirely correct. That's where integers or number rounding can come in handy in certain scenarios.

```
print(0.1 + 0.2)
print(round(0.1 + 0.2)) # rounds to no decimal place
print(round(0.1 + 0.2, 1)) # rounds to 1 decimal place
```{{exec}}

# Exercises
## Exercise 1
- Use `input` to ask a user for their age.
- Subtract 1 from that and print it.
- There's a chance that it results in an error.
- So let's convert the input into an integer before subtracting 1 and printing.

## Exercise 2
Ask user for a number and print out the square.
* Added challenge to print out in a sentence, eg if 5 is entered, print “The square of 5 is 25”

## Exercise 3
Ask user for the length and height of a rectangle and print out the area.

## Exercise 4
Ask user for 3 different numbers and print out the sum of the 3 numbers.
* Can you print out the average?

## Exercise 5
Ask user for a number and print out the previous and next number.

[Click here for solutions.](https://github.com/VCCBeginnerCoding/katacoda-scenarios/blob/main/1_PythonWeek1/answers/step3.md)


# You Finished Part 2!
Kahoot Time!!!