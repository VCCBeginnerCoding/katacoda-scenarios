# Basics
![Variables](./assets/variables.png)

You can store any value in a variable, then use it or change its value later on in the program. Click on the code snippets below and they will run automatically in the terminal (bottom right). You can also type it yourself and then press <kbd>ENTER</kbd> to execute it.

`myCardPin = 1234`{{exec}}
`a = 2`{{exec}}

Note: Variables are case sensitive, so `myCardPin`{{}} and `MyCaRdPiN`{{}} are two separate variables.

We can print out the variables.

`print(myCardPin)`{{exec}}
`print(a)`{{exec}}

We can assign a new value to an existing variable.

`myCardPin = 2222`{{exec}}
`myCardPin = 5555`{{exec}}
`myCardPin = 1382929292`{{exec}}

`print(myCardPin)`{{exec}}

✓ Valid variable names:
`_`{{}}
`days_to_christmas`{{}}
`Adiós_Señora`{{}}

✗ Invalid variable names:
`10t`{{}} * must begin with a letter
`Exchange Rate`{{}} * must not contain a space

Python also has a list of [reserved words](https://www.w3schools.com/python/python_ref_keywords.asp) that cannot be used as variable names.

# More about variables
Try these commands.

```
b = 4
print(b)
```{{exec}}

```
b = b+2
print(b)
```{{exec}}

```
b += 2
print(b)
```{{exec}}

You can also use `+`{{}}, `-`{{}}, `*`{{}}, `/`{{}}, `//`{{}}, `%`{{}}, `**`{{}} etc. [More Info](https://www.w3schools.com/python/python_operators.asp).

* `print(2+3)`{{exec}}
* `print(2-3)`{{exec}}
* `print(2*3)`{{exec}}
* `print(2/3)`{{exec}}
* `print(2//3)`{{exec}}
* `print(2%3)`{{exec}}

Python supports three types of numbers – int, float, and complex. Integers do not have a decimal point, while floats do. Complex is mostly used in geometry and scientific calculations. You can also convert numbers into strings, which Python will treat as text (so no more multiplications afterwards).

```
a = 4
b = 4.0
print(a+b)
```{{execute}}

```
a = 4.2
print(a)
print(int(a))
```{{execute}}

```
a = 4
print(a)
print(float(a))
```{{execute}}

<b>Yay you've completed part 1!</b>
