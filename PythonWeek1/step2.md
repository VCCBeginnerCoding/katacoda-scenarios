# Strings
Strings are text in code. They can be declared in Python like so:

`email = "donotreply@vodafone.com"
`{{execute}}

The code above declares the variable ```email``` and assigns it the string 'donotreply@vodafone.com'. We can print it out in Python like so:

`print(email)`{{execute}}

We can also print out strings directly like so:

`print("I like trains!")`{{execute}}

You can print a new line using ```\n```.

`print("I like\ntrains!")`{{execute}}

Try it yourself using the terminal on the right.

# Input
We can obtain user input using a special Python keyword/method called ```input()```. Let's say we want to obtain the user's name, in Python we do the following:

`username = input("What is your name?")`{{execute}}

 When we run this code, the program will wait for the user to enter a name before continuing. Please go to the terminal, type your name, and then press <kbd>ENTER</kbd>. In the above example, the user's name is stored in a variable ```username```. We can print out the user's name like so:

 `print("Your name is " + username)`{{execute}}

In the above code, we are combining the text *'Your name is '* with the string stored in ```username```. This is known as String Concatenation; joining two strings together.

 `print("Hello " + username + ", nice to meet you!")`{{execute}}

Try it yourself by typing in the Terminal!