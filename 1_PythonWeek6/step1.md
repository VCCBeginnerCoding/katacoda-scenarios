# Functions
A function is a named section of a code that performs a specific task. 
This typically involves taking some input, manipulating the input and returning an output.
Functions are useful as they allow us to abstract complexity in our programs and allow us to reuse the same code multiple times without copying and pasting.

## Defining and Calling Functions
Functions are defined using the `def` keyword followed by the name you wish to give the function. The name of the function is then followed by `()` and then a colon.
You can then call the function by using the name of the function followed by `()`.
```python
def my_function(): 
  print("Hello from a function") 

# calling my_function()
my_function() 
```{{exec}}
Note! The code that should be ran by the function needs to be indented to tell python that the code belongs to the function.

## Parameter Functions
You can also pass data to a function, the data you pass to a function is referred to as parameters or arguments.

```python
def sayHi(name, fav_number):
    print(f"Hi {name.title()}! I heard your favourite number is {fav_number}")

sayHi("james", 4)
```{{exec}}

Note! It is good programming practice to specify the data type of your parameters. Here is an improved version of the code above.
```python
def sayHi(name: str, fav_number: int):
    print(f"Hi {name.title()}! I heard your favourite number is {fav_number}")

sayHi("james", 4)
```{{exec}}

The above example shows how you can provide the parameter values in the order they are expected by the function. You can also provide the parameters in any order you like, however, you must then use the name of the parameter.

```python
def sayHi(name: str, fav_number: int):
    print(f"Hi {name.title()}! I heard your favourite number is {fav_number}")

sayHi("james", 4)
sayHi(fav_number=4, name="james")
```{{exec}}

## Default Parameter Values
You can define default values for your parameters which can make those paramters optional.
```python
def sayHi(name: str, fav_number: int = None):
    print(f"Hi {name.title()}!")

    if fav_number is None:
        print(f"I don't know you favourite number")
    else:
        print(f"I heard your favourite number is {fav_number}")
```{{exec}}

### Difference between Positional and Keyword Argurments
Note! There are two types of arguments (parameters), positional and keyword. When you do not define a default value for an argument it is treated as a positional argument. While arguments with a default value are considered as keyword arguments.

All your positional arguments must be defined before your keyword arguments.

## Returning Data
Functions can also return data; this is achieved using the `return` keyword followed by the data you want to return.

```python
def get_is_even_number(number: int):
    if number % 2 == 0:
        return "even"
    else:
        return "odd"

print(f"The number 7 is {get_is_even_number(7)}")
print(f"The number 10 is {get_is_even_number(10)}")
print(f"The number 13 is {get_is_even_number(13)}")
print(f"The number 16 is {get_is_even_number(16)}")
```{{exec}}

Note! It is good programming practice to also specify the return type of a function. Here is an improved version of the code above.

```python
def get_is_even_number(number: int) -> str:
    if number % 2 == 0:
        return "even"
    else:
        return "odd"

print(f"The number 7 is {get_is_even_number(7)}")
print(f"The number 10 is {get_is_even_number(10)}")
print(f"The number 13 is {get_is_even_number(13)}")
print(f"The number 16 is {get_is_even_number(16)}")
```{{exec}}

Note! If your function does not return any value, you should specify the return type as `None`.

# Exercises:
## 1
Build a function that takes a user's name and favourite colour. Ouput a greeting message stating their name and favourite colour.

## 2
* Build a function that askes the user for an integer input
* The function should return True or False indicating if the number provided by the user is a multiple of 7 or not

## 3
Build a function that takes two numbers and returns the average.

