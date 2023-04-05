<p align="center">
    <img src="./assets/ifelse.png" alt="If-else Statement" width="250" class="center"/>
</p>

Conditional statements check if a specified condition is met before carrying out an action.  

An if/else statement is an example of a conditional statement in Python.

You can see an example of the if/else statement below which checks if a statement is True or False: 

Create and open new Python file in the editor: `ifelseexample.py`

<pre class="file" data-filename="ifelseexample.py" data-target="replace">
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
`python ifelseexample.py`{{execute}}

*__Note:__ Sometimes for the code blocks to execute you may have to press this button more than once*

This code checks if the **colour variable** is set to the string Green. If the statement is True then the code prints "The Colour is Green!". Otherwise the code executes the else statement printing "The colour is not Green" 

In the future if the terminal gets messy clear it with `clear`{{execute}}.

</br>

There are also **Else If** statements to check for secondary conditions. In Python Else If statements are abbreviated to 'elif'. Multiple Elif statements after each other are sometimes called a **cascade**. 

An example of this is checking if the colour is yellow after you have checked if it is green, as shown below:

Replace the old code in the ifelseexample.py file with this code

<pre class="file" data-filename="ifelseexample.py" data-target="replace">
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

`python ifelseexample.py`{{execute}}

This code checks to see if the **colour variable** is set to the string Green, then it moves to the `elif colour == "Yellow"` line, which checks if the colour is yellow instead. If it is then it executes the print statement "The Colour is Yellow!". Again, if the colour is not green or yellow, it will move to the else statement and print "The Colour is not Green or Yellow!".

