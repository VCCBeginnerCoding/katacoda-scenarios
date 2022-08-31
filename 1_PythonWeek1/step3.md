# Numbers
Hover over the code snippets below and click *Copy to Editor* to copy the code to a Python file in your editor (top right).

<hr>

Python supports three types of numbers – `int`, `float`, and `complex`. Integers do not have a decimal point, while floats do. Complex is mostly used in geometry and scientific calculations (so ignore them for now). You can also convert numbers into strings, which Python will treat as text (so no more multiplications afterwards).

*Integer and float*
<pre class="file" data-filename="week1.py" data-target="replace">
a = 4
b = 4.0
print(a+b)
</pre>

*Float printed out as an integer*
<pre class="file" data-filename="week1.py" data-target="replace">
a = 4.2
print(a)
print(int(a))
</pre>

*Integer printed out as a float*
<pre class="file" data-filename="week1.py" data-target="replace">
a = 4
print(a)
print(float(a))
</pre>


If you want a user to enter a number that you can then manipulate in Python (for example, multiplying the user's age by 5) you'll want to make sure that Python understands it's a number instead of a string. After all, you can't do maths on text/string.

`input()` will return what Python "thinks" is best, but you can tell Python exactly what variable type you want by doing the following:

<pre class="file" data-filename="week1.py" data-target="replace">
number = int(input("Enter a number"))
print(number)
</pre>

<hr>

# Text
You already know the variable type for text - it's `string`.

<hr>

# Other Data Types
There are many more data types that you'll learn about in future lessons, many of which will take the knowledge from this session and find practical day to day uses for them.

<hr>

# Quick Exercise
- Use `input` to ask a user for their age.
- Subtract 1 from that and print it.
- There's a chance that it results in an error.
- So let's convert the input into an integer before subtracting 1 and printing.

[Click here for solutions.](https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md)

<hr>

# Practical Uses
Floating-point real numbers can't be represented with exact precision due to hardware limitations, so `print(0.1 + 0.2)` gives `0.30000000000000004`, which is obviously not entirely correct. That's where integers or number rounding can come in handy in certain scenarios.
<pre class="file" data-filename="week1.py" data-target="replace">
print(0.1 + 0.2)
print(round(0.1 + 0.2)) # rounds to no decimal place
print(round(0.1 + 0.2, 1)) # rounds to 1 decimal place
</pre>
