# Practical Python

As your project gets more and more complicated you may soon come across a need to reuse code in different parts of your project. That's where functions come in.

Open new Python file: `functions.py`{{open}}

<pre class="file" data-filename="functions.py" data-target="replace">
def my_function(): # creates a function called my_function()
    print("Hello from a function") # the function itself prints the string "Hello from a function"

my_function() # calls, or runs, the function my_function()
</pre>

`python functions.py`{{execute}}

# Arguments

The function above isn't actually very useful, since it'd be faster to just type ```print("Hello from a function")``` whenever you need that to run. Luckily, we can pass information into functions, called ```arguments```.

<pre class="file" data-filename="functions.py" data-target="replace">
def my_function(fname): # defines a function called my_function() where you pass in an argument called fname
    print(fname + " Refsnes") # as you can see the argument fname is used within the function

my_function("Emil")
my_function("Tobias")
my_function("Linus")
</pre>

`python functions.py`{{execute}}

# Multiple Arguments

<pre class="file" data-filename="functions.py" data-target="replace">
def my_function(fname, lname):
  print(fname + " " + lname)

my_function("Emil", "Refsnes")
</pre>

`python functions.py`{{execute}}

# Others

[Read more](https://www.w3schools.com/python/python_functions.asp) about passing arguments into functions, such as ```*args``` and ```keyword arguments```.