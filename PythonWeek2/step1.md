<p align="center">
    <img src="./assets/ifelse.png" alt="If-else Statement" width="250" class="center"/>
</p>

One of the fundamental parts of programming are conditional statements, which is when a set of actions are taken if a condition is met. As an example of this in real life, if two people are playing catch, the first person will check that the second is paying attention to them (the condition) before they throw them the ball (set of actions). 

An If/Else statement is one of the simpler conditional statements in Python, which we will be exploring today. You are most likely to use If/Else statements in Python when you wish for code to execute only if something else is True or False, such as the example below:

Open new Python file: `colour.py`{{open}}

<pre class="file" data-filename="colour.py" data-target="replace">
colour = "Green"

if colour == "Green":
    print("The Colour is Green!")
else:
    print("The Colour is not Green!")


colour = "Yellow"

if colour == "Green":
    print("The Colour is Green!")
else:
    print("The Colour is not Green!")
</pre>

Copy the code above over to the editor and then press
`python colour.py`{{execute}}

If the terminal gets messy clear it with `clear`{{execute}}.

In the above example, the code checks if the **colour variable** is set to the string Green or not  by using the 'if colour == "Green"' line. If it is "Green" then the print statement stating "The Colour is Green!" is executed, otherwise the 'else' line is executed meaning the print statement stating "The Colour is not Green" is executed. This is just a simple example of what an If/Else statement can do.

</br>

There are also **Else If** statements to check for secondary conditions after you have checked for the first condition, for example, checking if the colour is yellow after you have checked if it is green, as shown below:

Replace the old code in the colour.py file with this code

<pre class="file" data-filename="colour.py" data-target="replace">
colour = "Yellow"

if colour == "Green":
    print("The Colour is Green!")
elif colour == "Yellow":
    print("The Colour is Yellow!")
else:
    print("The Colour is not Green or Yellow!")


colour = "Blue"

if colour == "Green":
    print("The Colour is Green!")
elif colour == "Yellow":
    print("The Colour is Yellow!")
else:
    print("The Colour is not Green or Yellow!")
</pre>

`python colour.py`{{execute}}

In the above example, the code checks to see if the **colour variable** is set to the string Green or not as usual, then it moves to the 'elif colour == "Yellow"' line, which checks if the colour is yellow instead, if it is then it executes the print statement "The Colour is Yellow!". In Python Else If statements are abbreviated to 'elif'. Again, if the colour is not green or yellow, it will move to the else statement and print "The Colour is not Green or Yellow!". As you have probably already gathered, the 'else' statement just means, if none of the other conditionals are met (i.e. it's not green or yellow) then execute these steps. **Elif** is used to check more than just one condition, and to stop when the first statement which is true is found. Multiple Elif statements after each other are sometimes called a **cascade**.

Note: else is always the last branch of a cascade, regardless of whether you've used elif or not. Else is optional and may be omitted, but as stated, must always be at the end of the cascade if it is included.