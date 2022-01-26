# Strings
Hover over the code snippets below and click *Copy to Editor* to copy the code to a Python file in your editor (top right).

Messy Terminal? `clear`{{execute}} it.
<hr>

Strings are text in code. They can be declared in Python like so:

<pre class="file" data-filename="week1.py" data-target="replace">
email = "donotreply@vodafone.com"
print(email)
</pre>

`python week1.py`{{execute}}

The code above declares the variable ```email``` and assigns it the string 'donotreply@vodafone.com', which we then print out in the Terminal.

We can also print out strings directly like so:

<pre class="file" data-filename="week1.py" data-target="replace">
print("I like trains!")
</pre>

`python week1.py`{{execute}}

You can print a new line using ```\n```.

<pre class="file" data-filename="week1.py" data-target="replace">
print("I like \ntrains!")
</pre>

`python week1.py`{{execute}}

Try it yourself using the terminal on the right.

<hr>

# Input
We can obtain user input using a special Python keyword/method called ```input()```. Let's say we want to obtain the user's name, in Python we do the following:

<pre class="file" data-filename="week1.py" data-target="replace">
username = input("What is your name?")
</pre>

`python week1.py`{{execute}}

 When we run this code, the program will wait for the user to enter a name before continuing. Please go to the terminal, type your name, and then press <kbd>ENTER</kbd>. In the above example, the user's name is stored in a variable ```username```. We can print out the user's name like so:

<pre class="file" data-filename="week1.py" data-target="replace">
username = input("What is your name?")
print("Your name is " + username)
</pre>

`python week1.py`{{execute}}

In the above code, we are combining the text *'Your name is '* with the string stored in ```username```. This is known as String Concatenation; joining two strings together.

<div><span style="color:#D1495B">greeting = </span><span style="color:blue">"Good morning!"</span></div>
<div><span style="color:#D1495B">question = </span><span style="color:orange">input(</span><span style="color:#D1495B">greeting</span><span style="color:orange">+</span><span style="color:blue">" What's your name?"</span><span style="color:orange">)</span></div>

```output: Good morning! What's your name?```

<pre class="file" data-filename="week1.py" data-target="replace">
username = input("What is your name?")
print("Hello " + username + ", nice to meet you!")
</pre>

`python week1.py`{{execute}}

<hr>

# Quick Exercise
- Ask the user for their favourite colour.
- Print that variable.
- Optional: Chain it by putting ```input()``` inside of ```print()``` so you only need 1 line of code

[Click here for solutions.](https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md)

<hr>

# Practical Uses
A lot of software require user input of some sort, be it a mouse click, a finger tap, via your keyboard or something else entirely. Instagram can only load your feed if you login and tell Instagram what your username/password is. Minecraft can only move your character if you tell it to, via mouse and keyboard. (Again, there's a few more steps involved in real life, but you get the idea.)