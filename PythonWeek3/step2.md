# Functions!

## What are functions?

A function is a relationship between one or more inputs and a set of outputs. In mathamatics, a function is normally represented as:

z = f(x,y)

Here, f is a function that operates on the input *x* and *y*. The output of the function is *z*. However, in programming, functions are much more generalised and versatile.

In programming, a function is a defined block of code that encapuslates a specific task or related group of tasks.
## Defining a function

To define a function in python, we use the <mark>def</mark> keytag

`def my_function():
  print("Hello from a function")
`{{execute}}

## Calling a function

To call a function, use the name of the function and add parentesis at the end:

`def my_function():
  print("Hello from a function")

my_function()
`{{execute}}

## Passing data to the function

We can also pass data to the function, by adding it inside the parentheses:

`def print_name(name):
    print("My name is " +name)

print_name("Dan")
print_name("Justin")
print_name("Ellie")`{{execute}}

Functions can take more than one argument:
`def print_car_details(make,model):
    print("The car is " +make + " " + model)

print_name("ford, fiesta")
print_name("Skoda, Octavia")
print_name("Citroen, C1")`{{execute}}

<mark:> But it can go wrong! </mark>

If the code expects two arguments and you give it one (or vise versa) it will throw an error:

Functions can take more than one argument:
`def print_car_details(make,model):
    print("The car is " +make + " " + model)

print_name("ford")
`{{execute}}

## Tuples
In python, tuples are used to store muliple items in a single variable. 

For example:

`thistuple = ("apple", "banana", "cherry")
print(thistuple)`{{execute}}

When creating functions, if you don't know the number of arguements to be passed, you can use a tuple:

`def my_dog_list(*dogs)
    print("The youngest dog is " + dogs[2])

my_dog_list("Toby", "Max", "Bob")
`{{execute}}


## Keyword arguments

Arguments can also be sent with the <mark>key = value syntax</mark>. The order does not matter in this case.

`def my_cat_list(cat1, cat2, cat3)
    print("The smallest cat is " +cat3)

my_cat_list(cat3="fido", cat2="sophie", cat1="felix")
`{{execute}}

If the number of keyword arguments that will be passed the function at two asterisk: <mark>**</mark> before the parameter name in the function definition
This way the function will receive a dictionary of arguments, and can access the items accordingly:

`def my_function(**kid):
  print("His last name is " + kid["lname"])

my_function(fname = "Tobias", lname = "Refsnes")`{{execute}}


## Default values
A default value can be set, which will be placed if no value is passed:

`def fav_TVShow(show = "Lucifer")

my_function("American horror story")
my_function("Money heist")
my_function()
my_function("Brooklyn Nine-Nine")`{{execute}}

## Lists
You can pass any data type to the function (string, number, list, dictionary etc.), and will be treated as the same data type by the function.

For example, if you pass a list to the function, it will be treated as a list by the function:

`def my_function(food):
  for x in food:
    print(x)

fruits = ["apple", "banana", "cherry"]

my_function(fruits)`{{execute}}

## Return
We can use the <mark>return</mark> keyword to return a value:

`def calculator(value)
    return value * 10

print(calculator(3))
print(calculator(5))
print(calculator(9))`{{execute}}

## The Pass statement
You cannot have a blank function, but in the very unlikely event that you do, you can use the pass statement to avoid an error

`def myFunction()
    pass
`{{execute}}

## Recursion!
Python accepts python recursion (a function that calls itself). This is a common mathamatical and programming concept. It has the benefit of meaning you can loop through the data to reach a result.

`def factorial(x):
    """This is a recursive function
    to find the factorial of an integer"""

    if x == 1:
        return 1
    else:
        return (x * factorial(x-1))


num = 3
print("The factorial of", num, "is", factorial(num))`{{execute}}

<marquee style='color: blue;'><b>Yay you've completed part 2!</b></marquee>
