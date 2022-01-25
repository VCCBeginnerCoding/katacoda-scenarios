# Basics
Hover over the code snippets below and click *Copy to Editor* to copy the code to a Python file in your editor (top right).

Messy Terminal? `clear`{{execute}} it.
<hr>

![Variables](./assets/variables.png)

You can store any value in a variable, then use it or change its value later on in the program. We can also print out the variables using ```print()```. <span style="color:green">print(</span><span style="color:blue">"Hello World!"</span><span style="color:green">)</span> <span style="color:green">print(</span><span style="color:blue">variable</span><span style="color:green">)</span>

Click here to create new Python file: `week1.py`{{open}}

<pre class="file" data-filename="week1.py" data-target="replace">
# This is a comment
# Python will not run this
# Use comments so you remember what the code does
myCardPin = 1234
print(myCardPin)

a = 2
print(a)
</pre>

Copy the code above over to the editor and then press
`python week1.py`{{execute}}. You can also type that yourself via the Terminal (bottom right) and then press <kbd>ENTER</kbd> to execute it.

Note: Variables are case sensitive, so ```myCardPin``` and ```MyCaRdPiN``` are two separate variables.

<hr>

We can assign a new value to an existing variable.

<pre class="file" data-filename="week1.py" data-target="replace">
myCardPin = 2222
print(myCardPin)

myCardPin = 5555
print(myCardPin)

myCardPin = 1382929292
print(myCardPin)
</pre>

`python week1.py`{{execute}}

<hr>

<span style="color:green">✓</span> Valid variable names: ```_``` ```days_to_christmas``` ```Adiós_Señora```

<span style="color:red">✗</span> Invalid variable names: ```10t``` *<span style="color:red">must begin with a letter</span>* ```Exchange Rate``` *<span style="color:red">must not contain a space</span>* ```?``` *<span style="color:red">must not be punctuation</span>*

Python also has a list of [reserved words](https://www.w3schools.com/python/python_ref_keywords.asp) that cannot be used as variable names.

<hr>

# More about variables
Try these commands.

<pre class="file" data-filename="week1.py" data-target="replace">
b = 4
print(b)

b = b+2
print(b)

b += 2
print(b)
</pre>

`python week1.py`{{execute}}

You can also use ```+```, ```-```, ```*```, ```/```, ```//```, ```%```, ```**``` etc. [More Info](https://www.w3schools.com/python/python_operators.asp).

<pre class="file" data-filename="week1.py" data-target="replace">
print(2+3)
print(2-3)
print(2*3)
print(2/3)
print(2//3)
print(2%3)
</pre>

`python week1.py`{{execute}}

<hr>

# Quick Exercise
- Save your age as a variable
- Save the current year (2022 as of writing) as a second variable
- Subtract the current year by your age (using the variables) and save that as a third variable
- Print out the third variable
- You've found your age! (We're assuming you were born on 1st January to keep this task simple.)

[Click here for solutions.](https://www.youtube.com/watch?v=dQw4w9WgXcQ)

<hr>

# Practical Uses
The calculator app on your phone remembers every number as you type it, as well as your previous calculations, thanks to variables. Microsoft Teams remembers your user settings and stores them as variables. Your phone stores your password as a variable too. (Okay, there's a few more steps involved in real life, but you get the idea.)

<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
