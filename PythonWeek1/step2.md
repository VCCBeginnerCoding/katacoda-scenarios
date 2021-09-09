# Input
We can obtain user input using a special Python keyword/method called input(). Let's say we want to obtain the user's name, in Python we do the following:

`username = input('What is your name? ')`{{execute}}

 When we run this code, the program will wait for the user to enter a name before continuing. In the above example, the user's name is stored in a variable 'username'. We can print out the user's name like so:

 `print("Your name is " + username)`{{execute}}

In the above code, we are combining the text 'Your name is ' with the string stored in username. This is known as String Concatenation; joining two strings together.

 `print("Hello " + username + ", nice to meet you!")`{{execute}}

Try it yourself!

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

# More about variables
You can also use ```+```, ```-```, ```*```, ```/```, ```//```, ```%```, ```**``` etc. [More Info](https://www.w3schools.com/python/python_operators.asp)

`print(2+3)`{{execute}}
`print(2-3)`{{execute}}
`print(2*3)`{{execute}}
`print(2/3)`{{execute}}
`print(2//3)`{{execute}}
`print(2%3)`{{execute}}