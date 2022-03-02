


## Defining and calling a function

A function is a named section of a code that performs a specific task. 
This typically involves taking some input, manipulating the input and returning an output.

To call a function, use the name of the function and add parenthesis () at the end.

You will see how there are indentations (tabs or spaces - up to the programmer!) underneath any colons (functions, loops, if statements...).
This tells Python that the code underneath is part of the same block, and without the correct indents Python will not work.

In calling a function at the bottom, there are no indents as this is considered the 'main' function, where the code runs outside of a function 
and executes the rest of our script.

<pre class="file" data-filename="functionCall.py" data-target="replace">
# Creating a function called my_function()
def my_function(): 
  # The function will then print this string
  print("Hello from a function") 

# calling my_function()
my_function() 
</pre>

`python functionCall.py`{{execute}}

## Passing data to the function

We can also pass data to the function, by adding it inside the parentheses as <mark>arguments</mark>:

<pre class="file" data-filename="passingData.py" data-target="replace">
def print_name(name):
  print("My name is " + name)

print_name("Aymen")
print_name("Emma")
print_name("Sandra")
print_name("Yasmin")
</pre>

`python passingData.py`{{execute}}

Functions can take more than one argument, and when you call them you must pass in the amount specified:

<pre class="file" data-filename="moreArugments.py" data-target="replace">
def print_car_details(make, model):
  print("The car is " + make + " " + model)

print_car_details("ford", "fiesta")
print_car_details("Skoda", "Octavia")
print_car_details("Citroen", "C1")
</pre>

`python moreArugments.py`{{execute}}

## Tuples
In python, tuples are used to store multiple items in a single variable. 

For example:

<pre class="file" data-filename="tuples.py" data-target="replace">
thistuple = ("apple", "banana", "cherry")
print(thistuple)
</pre>

`python tuples.py`{{execute}}

If you have varying lengths of variables to pass, you can use the <mark>*args</mark> annotation to pass in your arguments.

This denotes a tuple.

<pre class="file" data-filename="tupleAnnotation.py" data-target="replace">
def my_dog_tuple(*dogs):
  print("The youngest dog is " + dogs[2])

my_dog_tuple("Toby", "Max", "Bob")
</pre>

`python tupleAnnotation.py`{{execute}}

## Keyword arguments

Arguments can also be sent with the <mark>key = value syntax</mark>. The order it is passed in does not matter in this case.

<pre class="file" data-filename="keywordArguments.py" data-target="replace">
def my_cat_values(cat3, cat1, cat2):
  print("The smallest cat is " + cat3)

# Note that the order of the variables is different to the arguments in the function
my_cat_values(cat1="fido", cat2="sophie", cat3="felix")
</pre>

`python keywordArguments.py`{{execute}}

If the argument passed in has <mark>**args</mark> these are known as 'kwargs' (keyword arguments), and allow us to pass in varying lengths of key-value pairs.
We can then access each argument based on its key.

<pre class="file" data-filename="keywordAnnotation.py" data-target="replace">
def kwargs(**kid):
  print("His last name is " + kid["lname"])

kwargs(fname = "Tobias", lname = "Refsnes")
</pre>

`python keywordAnnotation.py`{{execute}}

## Default values
A default value can be set, which will be used if no value is passed:

<pre class="file" data-filename="defaultValues.py" data-target="replace">
def favourite_show(show = "Lucifer"):
  print(show)

favourite_show("American horror story")
favourite_show()
</pre>

`python defaultValues.py`{{execute}}

## Passing in different data types
Python allows for different data types (Strings, Lists, Tuples...) to be passed in and treated as that data type.

This means a function could accept different data types:

<pre class="file" data-filename="passingDifferentData.py" data-target="replace">
def print_argument(data):
  for x in data:
    print(x)

fruits = ["apple", "banana", "cherry"]
sentance = "Hello world"

print_argument(fruits)
print_argument(sentance)
</pre>

`python passingDifferentData.py`{{execute}}

## Return
We can use the <mark>return</mark> keyword to return a value:

<pre class="file" data-filename="return.py" data-target="replace">
def calculator(value):
  return value * 10

print(calculator(3))
print(calculator(5))
print(calculator(9))
</pre>

`python return.py`{{execute}}

## The Pass statement
You cannot have a blank function, but if you need to have a function as a placeholder (eg. for future code), you can use the <mark>pass</mark> keyword

<pre class="file" data-filename="pass.py" data-target="replace">
def placeholder():
  pass
    
placeholder()
</pre>

`python pass.py`{{execute}}

## Recursion!
Recursion is a mathematical and computing concept that allows us to loop through data without using for or while. This has the benefit of making the code more efficient, and works by having a function return a call to itself. 
For example, we can pass in a counter to a recursive function and increment it until it reaches a desired value, then simply return the end amount:

<pre class="file" data-filename="recursiveCall.py" data-target="replace">
# This is a recursive functuon that returns the addition
# of 5 decreasing numbers
def recursive(number, count, answer):
  
  if count == 5:
    return answer
  else:
    # decreasing the value added using number-1
    # increasing the count of numbers used using count+1
    # calculating the addition of the next number using answer+number
    return recursive(number-1, count+1, answer+number)

# For reference, this is what the recursive call would look like in a while loop:

def loop(number, count, answer):

  while count < 5:
    answer += number
    number -= 1
    count += 1
  
  return answer

# We need (start val, number of values already added, total addition) to pass into the functions
# in this case, the last two numbers are 0 as we are at the start of the loop

print("RECURSIVE")
print(recursive(10,0,0))
print ("LOOP")
print(loop(10,0,0))
</pre>

`python recursiveCall.py`{{execute}}

<marquee style='color: blue;'><b>Yay you've completed part 2!</b></marquee>
