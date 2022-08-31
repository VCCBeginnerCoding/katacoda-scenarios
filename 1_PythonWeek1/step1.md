# Basics
Hover over the code snippets below and click *Copy to Editor* to copy the code to a Python file in your editor (top right).
<hr>


Variables are containers for storing data values. You can store any value in a variable, then use it or change its value later on in the program. We can also print out the variables using `print()`. As you found out from the last session, printing text in Python looks like this: `print("Hello World")`

You can store different types of data in variables as shown below. Text is stored as strings, numbers can be stored as integers (whole numbers) or floats (decimals). There is also boonleans that act as a true/false and can only store these values. 
![DataTypes](./assets/data-types.png)

<pre class="file" data-filename="week1.py" data-target="replace">
# This is a comment
# Python will not run this
# Use comments so you remember what the code does
myCardPin = 1234
print(myCardPin)

a = 2
print(a)
</pre>

Copy the code above over to the editor and then type 
`python week1.py` into the terminal. You can also type that yourself via the Terminal (bottom right) and then press ENTER to execute it.

Note: Variables in Python are case sensitive, so `myCardPin` and `MyCaRdPiN` are two separate variables.

We can assign a new value to an existing variable.

<pre class="file" data-filename="week1.py" data-target="replace">
myCardPin = 2222
print(myCardPin)

myCardPin = 5555
print(myCardPin)

myCardPin = 1382929292
print(myCardPin)
</pre>

<span style="color:green">✓</span> Valid variable names: `days_to_christmas` `Currency`

<span style="color:red">✗</span> Invalid variable names: `10t` *<span style="color:red">must begin with a letter</span>* `Exchange Rate` *<span style="color:red">must not contain a space</span>* `?` *<span style="color:red">must not be punctuation</span>*

Python also has a list of [reserved words](https://www.w3schools.com/python/python_ref_keywords.asp) that cannot be used as variable names.

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

You can also use `+`, `-`, `*`, `/`, `//`, `%`, `**` etc. [More Info](https://www.w3schools.com/python/python_operators.asp).

<pre class="file" data-filename="week1.py" data-target="replace">
print(2+3)
print(2-3)
print(2*3)
print(2/3)
print(2//3)
print(2%3)
</pre>

# Quick Exercise
- Save your age as a variable
- Save the current year (2022 as of writing) as a second variable
- Subtract the current year by your age (using the variables) and save that as a third variable
- Print out the third variable
- You've found your birth year! (We're assuming you were born on 1st January to keep this task simple.)

[Click here for solutions.](https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md)

# Practical Uses
The calculator app on your phone remembers every number as you type it, as well as your previous calculations, thanks to variables. Microsoft Teams remembers your user settings and stores them as variables. Your phone stores your password as a variable too. (Okay, there's a few more steps involved in real life, but you get the idea.)

<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
