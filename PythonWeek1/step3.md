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
Below you can see a series of ```if``` statements, and how it might be used in real life.
`# This is a comment
# Python will not run this
# But it's good to comment your code so you remember what does what

x = 10

if x > 5: # condition one
    print("x is greater than 5")  # Executed if condition one is True.

if x < 10: # condition two
    print("x is less than 10")  # Executed if condition two is True.

if x == 10: # condition three
    print("x is equal to 10")  # Executed if condition three is True.`{{copy}}

You can see that the ```print``` statements are indented, like they are nested under the ```if``` statements. These will only run if the conditions above are met. You can indent by tabbing once, typing 4 spaces or typing 2 spaces. Find something you're comfortable with and stick with it. For this course we'll be using tabs or 4 spaces.

`helloworld.py`{{open}}
Copy and paste the code snippet over to the terminal and play around with it!

# elif
Else if ```elif``` is Python's way of saying if the previous conditions were not true, then try this condition.

```
a = 33
b = 33
if b > a:
    print("b is greater than a")
elif a == b:
    print("a and b are equal")

```

# else
The ```else``` keyword catches anything which isn't caught by the preceding conditions.

```
a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
```