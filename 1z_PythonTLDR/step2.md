# Strings
Strings are text in code. They can be declared in Python like so:

```
foo = 'this is an example of a string'
email = "donotreply@vodafone.com"
```{{exec}}

The code above declares the variable `foo`{{}} and assigns it the string 'this is an example of a string'. We can print foo out in Python like so:

* `print(foo)`{{exec}}
* `print(email)`{{exec}}

We can also print out strings directly like so:

* `print("I like trains!")`{{exec}}

You can print a new line using `\n`{{}}.

* `print("I like\ntrains!")`{{exec}}

Try it yourself using the terminal on the right.

# Input
We can obtain user input using a special Python keyword/method called input(). Let's say we want to obtain the user's name, in Python we do the following:

`username = input('What is your name? ')`{{exec}}

 When we run this code, the program will wait for the user to enter a name before continuing. Please go to the terminal, type your name, and then press <kbd>ENTER</kbd>. In the above example, the user's name is stored in a variable `username`{{}}. We can print out the user's name like so:

 * `print("Your name is " + username)`{{exec}}

In the above code, we are combining the text *'Your name is '* with the string stored in `username`{{}}. This is known as String Concatenation; joining two strings together.

* `print("Hello " + username + ", nice to meet you!")`{{exec}}

Try it yourself!

Remember int and float from the last section? If you want a user to enter a number that you can then manipulate in Python (for example, multiplying the user's age by 5) you'll want to make sure that Python understands it's a number instead of a string.

`input()`{{}} will return what Python "thinks" is best, but you can tell Python exactly what you want by doing the following:

```
number = int(input("Enter a number"))
```{{exec}}}