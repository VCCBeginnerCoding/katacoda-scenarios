# Loops
![Variables](./assets/variables.png) // This can be changed

There are two main form of loops in Python. The For loop and the While loop!

`loops.py`{{open}}

## While Loops
While loops execute a set of statements as long as a condition is true

<pre class="file" data-filename="loops.py" data-target="replace">
i = 1
while i < 6:
  print(i)
  i += 1
</pre>

`python loops.py`{{execute}}

## For Loops
A for loop is used to iterate over a sequence:

<pre class="file" data-filename="loops.py" data-target="replace">
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
</pre>

`python loops.py`{{execute}}

You can also use loops to iterate through a string:

<pre class="file" data-filename="loops.py" data-target="replace">
for x in "banana":
  print(x)
</pre>

`python loops.py`{{execute}}

Breaks can be used to stop the loop:

<pre class="file" data-filename="loops.py" data-target="replace">
fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
</pre>

`python loops.py`{{execute}}

Continue statement can be used (breaks the current iteration and moves to the next one)

<pre class="file" data-filename="loops.py" data-target="replace">
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
</pre>

`python loops.py`{{execute}}

  ## Try it yourself!
  - Step 1: Create an array
  - Step 2: Loop through the array
  - Step 3: Print all values in the array
  - Step 4: Create a break statement to break the statement after reading a certain value.


<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
