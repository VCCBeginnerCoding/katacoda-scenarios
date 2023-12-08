# Args, Kwargs and Lambda

## Args
It is also possible to pass an infinite number of positional arguments to function using the `*` operator in front of the name of the argument.

```python
def add(*numbers) -> float:
    total = 0
    for number in numbers:
        total += number
    return total

print(add())
print(add(1))
print(add(1, 3))
print(add(1, 3, 6, 8, 10))
```{{exec}}
Notice that the numbers parameter is treated as a tuple.

## Kwargs
 It is also possible to pass an infinite number of keyword arguments to a function using the `**` operator in front of the name of the argument.

 ```python
def display_info(**info) -> None:
    print(info)

display_info(name="james", age=25, fav_colour="green")
 ```{{exec}}
Notice that the info parameter is treated as a dictionary.

### Checking if a Parameter is Defined Within kwargs
You can check if a specific paramter is passed in the same way you would check if a key is present in a dictionary.

```python
def display_info(**info) -> None:
    if "name" in info.keys():
        print(f"Info about {info['name'].title()}:")
    
    print(info)

display_info(name="james", age=25, fav_colour="green")
print() # Print an empty line to create visual seperation
display_info(age=54, fav_colour="blue")
```{{exec}}

## Lambda Functions
Lambda functions also referred to as anonymous functions are functions that do not have a name assigned to them. They are mostly used for simple 1-line functions that are part of a larger function.

```python
add_one = lambda x: x + 1

num = add_one(4)
print(num)

# The code above is similar to writing
def add_one_alternative(x):
    return x + 1
```{{exec}}

### Real Use Case for Lambda Functions
A real scenrario for using lambda functions is to alter the sorting algorithm using by the .sort() function.
```python
numbers = [3, 5, 8, 9]
# this will sort numbers from lowest to highest
numbers.sort()
print(numbers)

# this will sort numbers from largest to lowest
numbers.sort(key=lambda x: x * -1)
print(numbers)
```{{exec}}

# Exercises:
## 1
Build a function that calculates the average of all the arguments passed to the function.

## 2
* Create a function that accepts kwargs arguments.
* If the argument "name" is provided, output the message "Hello <name>".
* If the argument "age" is provided, output the message "You are <age> years old" 