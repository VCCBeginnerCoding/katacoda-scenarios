# Strings

Strings are text in code. They can be declared in Python like so:

```
email = "donotreply@vodafone.com"
print(email)
```{{exec}}

The code above declares the variable `email` and assigns it the string 'donotreply@vodafone.com', which we then print out in the Terminal.

We can also print out strings directly like so:

```
print("I like trains!")
```{{exec}}

You can print a new line using `\n`.

```
print("I like \ntrains!")
```{{exec}}

Try it yourself using the terminal on the right.


# Input
We can obtain user input using a special Python keyword/method called `input()`. Let's say we want to obtain the user's name, in Python we do the following:

```
username = input("What is your name?")
```{{exec}}

 When we run this code, the program will wait for the user to enter a name before continuing. Please go to the terminal, type your name, and then press <kbd>ENTER</kbd>. In the above example, the user's name is stored in a variable `username`. We can print out the user's name like so:

```
username = input("What is your name?")
print("Your name is " + username)
```{{exec}}

In the above code, we are combining the text *'Your name is '* with the string stored in `username`. This is known as String Concatenation; joining two strings together.

```
greeting = "Good morning!"
question = input(greeting + " What's your name?")
```{{exec}}

`output: Good morning! What's your name?`

```
username = input("What is your name?")
print("Hello " + username + ", nice to meet you!")
```{{exec}}


# Practical Uses
A lot of software require user input of some sort, be it a mouse click, a finger tap, via your keyboard or something else entirely. Instagram can only load your feed if you login and tell Instagram what your username/password is. Minecraft can only move your character if you tell it to, via mouse and keyboard. (Again, there's a few more steps involved in real life, but you get the idea.)

# Test your knowledge:
## 1.
Ask the user for a name (eg Tom) and ask user for an emotion (eg happy).  Print out “<name> is feeling <emotion>.”  Eg “Tom is feeling happy.”.
### 1.1 
Extend your program to print out 2 lines – “Pleased to meet you Tom./n Tom is feeling happy today!”

## 2. Extra challenge
* Write a short story (just 1 paragraph) about a character learning how to code. Write it out on paper first.
* Write a program to ask user for a name and ask user what pronouns to use (ie he/him/she/her).  Print your story using the users names and pronouns so that it makes sense.

Ask for help and where to find the example answers when you are done.

[Click here for solutions.](https://github.com/VCCBeginnerCoding/katacoda-scenarios/blob/main/1_PythonWeek1/answers/step2.md)

You have completed part 1!
Kahoot Time!!!