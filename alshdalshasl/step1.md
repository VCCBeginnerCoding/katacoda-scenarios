# Basics
![Variables](./assets/variables.png)

You can store any value in a variable, then use it or change its value later on in the program. Click on the code snippets below and they will run automatically in the terminal (bottom right).

`myCardPin = 1234`{{execute}}
`a = 2`{{execute}}

Note: Variables are case sensitive, so *myCardPin* and *MyCaRdPiN* are two separate variables.

We can print out the variables.

`print(myCardPin)`{{execute}}
`print(a)`{{execute}}

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

You can also use ```+```, ```-```, ```*```, ```/```, ```//```, ```%```, ```**``` etc. [More Info](https://www.w3schools.com/python/python_operators.asp)

`print(2+3)`{{execute}}
`print(2-3)`{{execute}}
`print(2*3)`{{execute}}
`print(2/3)`{{execute}}
`print(2//3)`{{execute}}
`print(2%3)`{{execute}}

Python supports three types of numbers – int, float, and complex. Integers do not have a decimal point, while floats do. Complex is mostly used in geometry and scientific calculations. You can also convert numbers into strings, which Python will treat as text (so no more multiplications afterwards).

`a = 4
b = 4.0
print(a+b)`{{execute}}

`a = 4.2
print(a)
print(int(a))`{{execute}}

`a = 4
print(a)
print(float(a))`{{execute}}

<marquee style='color: blue;'><b>Yay you've completed part 1!</b></marquee>
