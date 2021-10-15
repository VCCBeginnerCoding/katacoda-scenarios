# Loops
![Variables](./assets/variables.png) // This can be changed

There are two main form of loops in Python. The For loop and the While loop!

## While Loops
While loops execute a set of statements as long as a condition is true

`i = 1
while i < 6:
  print(i)
  i += 1
# Click me to run the code in the terminal
`{{execute}}

## For Loops
A for loop is used to iterate over a sequence:

`fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
# Click me to run the code in the terminal  
  `{{execute}}

You can also use loops to iterate through a string:

`for x in "banana":
  print(x)
# Click me to run the code in the terminal
`{{execute}}

Breaks can be used to stop the loop:

`fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break
# Click me to run the code in the terminal    
`{{execute}}

Continue statement can be used (breaks the current iteration and moves to the next one)

`i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
 # Click me to run the code in the terminal 
  `{{execute}}

  ## Try it yourself!
  - Step 1: Create an array
  - Step 2: Loop through the array
  - Step 3: Print all values in the array
  - Step 4: Create a break statement to break the statement after reading a certain value.


<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
