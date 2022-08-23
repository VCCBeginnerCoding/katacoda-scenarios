# Using Comparisions

![Variables](./assets/ifelse.png)<br>

You don't have to understand ```if``` statements right now - we'll cover those next week. But here's why comparisions can come in handy, and why Python can be a versatile language.

<pre class="file" data-filename="week1.py" data-target="replace">
age = 17

if age < 18: 
    print("You're too young to buy scissors.")

if age < 0: 
    print("You haven't been born yet.")
</pre>

<hr>

# Indentation

See how the ```print``` statement above is indented? It means it sits under the ```if``` statement, and will only run if the conditions of that ```if``` statement is true.

To indent a line, you have a few options. Choose one and then start a fight with the others over which one is superior:

- press <kbd>SPACE</kbd> 4 times
- press <kbd>SPACE</kbd> 2 times
- press <kbd>TAB</kbd> once

Indentation is very important. While other programming languages allow you to write horrifyingly unindented code and wrap them in ```{}``` brackets, Python relies on your indentation to know when to run what code. Remember this!
