# Loops
![Variables](./assets/variables.png) // This can be changed

There are two main form of loops in Python. The For loop and the While loop!

## While Loops
While loops execute a set of statements as long as a condition is true

`i = 1
while i < 6:
  print(i)
  i += 1`{{execute}}

## For Loops
A for loop is used to iterate over a sequence:

`fruits = ["apple", "banana", "cherry"]
for x in fruits:
 print(x)`{{execute}}

You can also use loops to iterate through a string:

`for x in "banana":
   print(x)`{{execute}}

Breaks can be used to stop the loop:

`fruits = ["apple", "banana", "cherry"]
for x in fruits:
 print(x)
 if x == "banana":
  break`{{execute}}

Continue statement can be used (breaks the current iteration and moves to the next one)

`i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)`{{execute}}

<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
