# Basics
First things first let's initialise Python by clicking on this here: `python`{{execute}}

You can store any value in a variable, then use it or change its value later on in the program. For example:

`myCardPin = 1234`{{execute}}
`a = 2`{{execute}}

Note: Variables are case sensitive.

We can print out the variables.

`print(myCardPin)`{{execute}}
`print(a)`{{execute}}

We can change the variables.

`myCardPin = 2222`{{execute}}
`myCardPin = 5555`{{execute}}
`myCardPin = 1382929292`{{execute}}

`print(myCardPin)`{{execute}}

# Strings
Strings are text in code. They can be declared in Python like so:

`foo = 'this is an example of a string'
email = "donotreply@vodafone.com"
`{{execute}}

The code above declares the variable 'foo' and assigns it the string 'this is an example of a string'. We can print foo out in python like so:

`print(foo)`{{execute}}
`print(email)`{{execute}}

We can also print out strings directly like so:

`print("I like trains!")`{{execute}}

Try it yourself using the terminal on the right.

# Input
We can obtain user input using a special Python keyword/method called input(). Let's say we want to obtain the user's name, in Python we do the following:

`username = input('What is your name? ')`{{execute}}

 When we run this code, the program will wait for the user to enter a name before continuing. In the above example, the user's name is stored in a variable 'username'. We can print out the user's name like so:

 `print("Your name is " + username)`{{execute}}

In the above code, we are combining the text 'Your name is ' with the string stored in username. This is known as String Concatenation; joining two strings together.

 `print("Hello " + username + ", nice to meet you!")`{{execute}}

Try it yourself!

`%%html
<marquee style='width: 30%; color: blue;'><b>Whee!</b></marquee>`{{execute}}
