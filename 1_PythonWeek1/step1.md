# Basics
![Variables](./assets/variables.png)

You can store any value in a variable, then use it or change its value later on in the program. Click on the code snippets below and they will run automatically in the terminal (bottom right). You can also type it yourself and then press <kbd>ENTER</kbd> to execute it.

`myCardPin = 1234`{{execute}}
`a = 2`{{execute}}

Note: Variables are case sensitive, so ```myCardPin``` and ```MyCaRdPiN``` are two separate variables.

We can print out the variables.

`print(myCardPin)`{{execute}}
`print(a)`{{execute}}

![Variables](./assets/components1.png)

We can assign a new value to an existing variable.

`myCardPin = 2222`{{execute}}
`myCardPin = 5555`{{execute}}
`myCardPin = 1382929292`{{execute}}

`print(myCardPin)`{{execute}}

<span style="color:green">✓</span> Valid variable names: ```_``` ```days_to_christmas``` ```Adiós_Señora```

<span style="color:red">✗</span> Invalid variable names: ```10t``` *<span style="color:red">must begin with a letter</span>* ```Exchange Rate``` *<span style="color:red">must not contain a space</span>*

Python also has a list of [reserved words](https://www.w3schools.com/python/python_ref_keywords.asp) that cannot be used as variable names.

# More about variables
Try these commands.

`b = 4
print(b)`{{execute}}
`b = b+2
print(b)`{{execute}}
`b += 2
print(b)`{{execute}}

You can also use ```+```, ```-```, ```*```, ```/```, ```//```, ```%```, ```**``` etc. [More Info](https://www.w3schools.com/python/python_operators.asp).

`print(2+3)`{{execute}}
`print(2-3)`{{execute}}
`print(2*3)`{{execute}}
`print(2/3)`{{execute}}
`print(2//3)`{{execute}}
`print(2%3)`{{execute}}

# Quick Exercise
- Type your code line by line into the Terminal (don't forget to press <kbd>ENTER</kbd>)
- Save your age as a variable
- Save the current year (2021 as of writing) as a second variable
- Use maths to figure out your birth year (assume you're born on 1st Jan to make the maths simpler)
- Save the answer as a third variable and print it

# Practical Uses
The calculator app on your phone remembers every number as you type it, as well as your previous calculations, thanks to variables. Microsoft Teams remembers your user settings and stores them as variables. Your phone stores your password as a variable too. (Okay, there's a few more steps involved in real life, but you get the idea.)

<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
