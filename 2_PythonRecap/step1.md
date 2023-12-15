# Data Types, Casting, Input & Output

## Python Primitive Data Types
* int
* float
* str
  * string concatination using + and f-strings
* chr
* bool
* None

## Composite Data Types
* list
* tuple

With sequences such as lists, tuples, and strings, you can use the `len()` function to find the total number of items in the sequence.
```python
a = [1,2,3,4,5,6,7]
print(len(s))
```{{exec}}

You can also access specific items in the sequence by using its index position.
```python
a = [2, 4, 74, -4, 901, 3]
print(a[0])
print(a[5])
print(a[-1])
print(a[-3])
print(a[2:-1])
print(a[:]) # returns the whole list
print(a[::-1]) # reverses the sequence
```{{exec}}

## Data Type Casting
Data type casting is when you convert the data type of a variable from one data type to another.
Note! You can use the `type()` function to find out the type of a variable.
```python
a = "12.5"
print(a, type(a))
b = float(a)
print(b, type(b))
```{{exec}}

## Output
You can use the `print()` function to output a message onto the terminal.
### Simple Output
```python
print("Hello World!")
```{{exec}}
### Outputting multiple items
You can print multiple items at the same time, however, you must sepearte them using a comma, especially if they are of other data types.
```pyhton
name = "Ben"
favourite_number = 7
print(name, favourite_number)
```{{exec}}

## Getting Input from the Terminal
We can ask the user to give us a value via the terminal using the `input()` function. Remember, when using the input function the data entered by the user will be treated as a string; and must be casted if you want to use it as another data type.
```python
name = input("Enter your name: ")
age = int(input("Enter your age"))
print(f"Hello {name}! You said you are {age} years old!")
```{{exec}}

# Exercise
* Ask the user for their age.
* Using their age, display the message "You were born in the year YEAR_BORN"