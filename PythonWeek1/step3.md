# Comparison
```=``` is an assignment operator. ```a = 2``` assigns ```a``` with the value of ```2```.
```==``` instead asks the question *are the values equal*?

`100 == 100`{{execute}}
`100 == 200`{{execute}}

`a = 100
a == 100`{{execute}}

You can also use the ```!=``` not equal to operator.

`100 != 100`{{execute}}
`100 != 200`{{execute}}

Other operators include ```>``` greater than, ```>=``` greater than or equal to, ```<``` less than, and ```<=``` less than or equal to.

`100 > 100`{{execute}}
`100 >= 100`{{execute}}
`100 < 100`{{execute}}
`100 <= 100`{{execute}}

# if statements
We added code to automatically initialise Python within the terminal. You don't want to write actual code there since it gets messy very quickly. So let's quit Python. `exit()`{{execute}}

`ifstatements.py`{{open}}

Click on the above to create a new Python file in the editor (top right), and then copy the code below over to the new file.

<pre class="file" data-filename="ifstatements.py" data-target="replace"># This is a comment
# Python will not run this
# But it's good to comment your code so you remember what does what

x = 10

if x > 5: # condition one
    print("x is greater than 5")  # Executed if condition one is True.

if x < 10: # condition two
    print("x is less than 10")  # Executed if condition two is True.

if x == 10: # condition three
    print("x is equal to 10")  # Executed if condition three is True. </pre>

You can see that the ```print``` statements are indented, like they are nested under the ```if``` statements. These will only run if the conditions above are met. You can indent by pressing <kbd>TAB</kbd> once, <kbd>SPACE</kbd> four times or <kbd>SPACE</kbd> two times. Find something you're comfortable with and stick with it. For this course we'll be using tabs or 4 spaces.

To run the Python file, go to the terminal and execute this. `python ifstatements.py`{{execute}}

# elif
Else if ```elif``` is Python's way of saying if the previous conditions were not true, then try this condition.

<pre class="file" data-filename="ifstatements.py" data-target="replace">
a = 33
b = 33
if b > a:
    print("b is greater than a")
elif a == b:
    print("a and b are equal")
</pre>

`python ifstatements.py`{{execute}}

# else
The ```else``` keyword catches anything which isn't caught by the preceding conditions.

<pre class="file" data-filename="ifstatements.py" data-target="replace">
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
</pre>

`python ifstatements.py`{{execute}}