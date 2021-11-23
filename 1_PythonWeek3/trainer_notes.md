# Trainer Notes For Week 3

This document is to provide trainer details for the Week 3 content of the Crash Course. The topics covered are: Loops, Functions, Classes and recusion. There are multiple interactive elements in this course.

## Step 1: Loops
This section covers two loops: The while loop and the For loop. It demonstrates how a for loop works, how it can iterate over a sequence, over a string, how breaks work and how continue statements work.

The student is asked to try it for themselves. The task is to create through an array and loop through it. They are then asked to create a break statement when for a certain value. 

For example:

fruits = ["apple", "banana", "cherry"]
for x in fruits:
  print(x)
  if x == "banana":
    break

## Step 2: Functions
This section gives a brief overview of what a function is, then explains how to define it, how to call it, how to pass data to it, what happens when only one argument is passed when more is expected, how tuples work, what keyword arguments are, how default values work, how to pass a list to a function, how the return statement works, how the pass statement works and the basics of recursion.

## Step 3: Have a go section.
Here the user is presented with two tasks to work through.

1. Fizz Buzz: The user is asked to provide a maxium value, and then loop through all numbers between 0 and the maximum value checking against the following:

If the current number is divisible by 3, it should print “Fizz”.
If it is divisible by 5, it should print “Buzz”.
If it is divisible by both 3 and 5, it should print “FizzBuzz”.
Otherwise, it should print the same number.

Example code:

def fizzBuzzFunc(maxValue):
    fizzbuzz = 0
    while fizzbuzz < maxValue:
        if fizzbuzz % 3 == 0 and fizzbuzz % 5 == 0:
            print("fizzbuzz")
            continue
        elif fizzbuzz % 3 == 0:
            print("fizz")
            continue
        elif fizzbuzz % 5 == 0:
            print("buzz")
            continue
        print(fizzbuzz)

maximumValue = input("please enter max value")
fizzBuzzFunc(maximumValue)

The additional tasks are as follows:
Using default value: def fizzBuzzFunc(maxValue = 100):
Adding lower parameter: def fizzBuzzFunc(maxValue = 100, lowerValue = 0):
Using keyword value: fizzBuzzFunc(maxValue = 50, lowerValue = 20)

2. The second task is to use a tuple to create a list of car manufactures and loop through them 

Example code:

carManufactures = ("BMW", "Ford", "Skoda", "Citroen")
for x in carManufactures
    print(carManufactures)

The extra tasks if they can use a nested tuple to also include car models. For example: 
my_tuple = ("Skoda, Fabia, Kodiaq", ("Peugeot, 208, 308"))

## Step 4 - Classes
This section defines briefly what a class is, how to create objects, the init() function, how functions work inside classes, the self parameter, how to modify object properties, how to delete properties and the pass statement.

## step 5: Classes Task

This task asks the student to create a class called pet, and then create a class called Dog that inherits from pet. 

For example:

class Pet:
    def __init__(self,name,age,fav_food):
        self.petName = name
        self.petAge = age
        self.favouriteFood = fav_food
        
class Dog(Pet):
    def __init__(self, name, age, fav_food, fav_toy):
        super().__init__(name, age, fav_food)
        self.favoriteToy = fav_toy
        
    def printdetails(self):
        print("The dog is called " + self.petName + " who is " + self.petAge + " years old")
    
x = Dog("Fido", "5" , "Dry food", "Ball")
x.printdetails()




