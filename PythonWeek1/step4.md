# while
```
while there is something to do
    do it
```

As you can see, ```while``` and ```if``` work similarly.

Open new Python file: `loops.py`{{open}}

<pre class="file" data-filename="loops.py" data-target="replace">
# Store the current largest number here.
largest_number = -999999999

# Input the first value.
number = int(input("Enter a number or type -1 to stop: "))

# If the number is not equal to -1, continue.
while number != -1:
    # Is number larger than largest_number?
    if number > largest_number:
        # Yes, update largest_number.
        largest_number = number
    # Input the next number.
    number = int(input("Enter a number or type -1 to stop: "))

# Print the largest number.
print("The largest number is:", largest_number)

# Click here and then press enter on the terminal to run this code.
</pre>

`python loops.py`{{execute}}

If you're stuck in an infinite loop and want it to stop you can press <kbd>CONTROL</kbd><kbd>C</kbd>, <kbd>CONTROL</kbd><kbd>BREAK</kbd> or <kbd>COMMAND</kbd><kbd>C</kbd> depending on your computer.

# for

Try to guess what this does before running it.

<pre class="file" data-filename="loops.py" data-target="replace">
for i in range(10):
    print("The value of i is currently", i)
</pre>

`python loops.py`{{execute}}

<pre class="file" data-filename="loops.py" data-target="replace">
for i in range(2, 8): # start at 2, stop BEFORE 8
    print("The value of i is currently", i)
</pre>

`python loops.py`{{execute}}

# break

# continue

