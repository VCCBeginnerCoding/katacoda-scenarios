Messy Terminal? `clear`{{execute}} it.
<hr>

## Defining and calling a function

A function is a named section of a code that performs a specific task. 
This typically involves taking some input, manipulating the input and returning an output.

To call a function, use the name of the function and add parenthesis () at the end.

You will see how there are indentations (tabs or spaces - up to the programmer!) underneath any colons (functions, loops, if statements...).
This tells Python that the code underneath is part of the same block, and without the correct indents Python will not work.

In calling a function at the bottom, there are no indents as this is considered the 'main' function, where the code runs outside of a function 
and executes the rest of our script.

```python
# Creating a function called my_function()
def my_function(): 
  # The function will then print this string
  print("Hello from a function") 

# calling my_function()
my_function() 
```{{copy}}

## Passing data to the function

We can also pass data to the function, by adding it inside the parentheses as <mark>arguments</mark>:

```python
def print_name(name):
  print("My name is " + name)

print_name("Aymen")
print_name("Emma")
print_name("Sandra")
print_name("Yasmin")
```{{copy}}

Functions can take more than one argument, and when you call them you must pass in the amount specified:

```python
def print_car_details(make, model):
  print("The car is " + make + " " + model)

print_car_details("ford", "fiesta")
print_car_details("Skoda", "Octavia")
print_car_details("Citroen", "C1")
```{{copy}}

## Tuples
In python, tuples are used to store multiple items in a single variable. 

For example:

```python
thistuple = ("apple", "banana", "cherry")
print(thistuple)
```{{copy}}


If you have varying lengths of variables to pass, you can use the <mark>*args</mark> annotation to pass in your arguments.

This denotes a tuple.

```python
def my_dog_tuple(*dogs):
  print("The youngest dog is " + dogs[2])

my_dog_tuple("Toby", "Max", "Bob")
```{{copy}}

## Keyword arguments

Arguments can also be sent with the <mark>key = value syntax</mark>. The order it is passed in does not matter in this case.

```python
def my_cat_values(cat3, cat1, cat2):
  print("The smallest cat is " + cat3)

# Note that the order of the variables is different to the arguments in the function
my_cat_values(cat1="fido", cat2="sophie", cat3="felix")
```{{copy}}

If the argument passed in has <mark>**args</mark> these are known as 'kwargs' (keyword arguments), and allow us to pass in varying lengths of key-value pairs.
We can then access each argument based on its key.

```python
def kwargs(**kid):
  print("His last name is " + kid["lname"])

kwargs(fname = "Tobias", lname = "Refsnes")
```{{copy}}

## Default values
A default value can be set, which will be used if no value is passed:

```python
def favourite_show(show = "Lucifer"):
  print(show)

favourite_show("American horror story")
favourite_show()
```{{copy}}

## Passing in different data types
Python allows for different data types (Strings, Lists, Tuples...) to be passed in and treated as that data type.

This means a function could accept different data types:

```python
def print_argument(data):
  for x in data:
    print(x)

fruits = ["apple", "banana", "cherry"]
sentance = "Hello world"

print_argument(fruits)
print_argument(sentance)
```{{copy}}

## Return
We can use the <mark>return</mark> keyword to return a value:

```python
def calculator(value):
  return value * 10

print(calculator(3))
print(calculator(5))
print(calculator(9))
```{{exec}}

## The Pass statement
You cannot have a blank function, but if you need to have a function as a placeholder (eg. for future code), you can use the <mark>pass</mark> keyword

```python
def placeholder():
  pass
    
placeholder()
```{{copy}}


<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
