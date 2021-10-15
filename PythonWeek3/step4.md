# Classes!

## What is a class?

Python is a "Object-orientated programming language". This means that each program is made up of mini "objects" which contains different properties and methods. A class is like a blueprint for creating these objects.

For example:

`classes.py`{{open}}

<pre class="file" data-filename="classes.py" data-target="replace">
class LinkedIn:
userName = "Bob Cratchit"
totalLikes = 622
lastPostDate = "14-10-2021"

print(LinkedIn)
</pre>

`python classes.py`{{execute}}

## Creating objects

We can now use the class "blueprint" to create an object

<pre class="file" data-filename="classes.py" data-target="replace">
class LinkedIn:
userName = "Bob Cratchit"
totalLikes = 622
lastPostDate = "14-10-2021"

myClass = LinkedIn()
print(myClass.totalLikes)
</pre>

`python classes.py`{{execute}}

## The **init**() function

All classes have a function called **init**(), which is always executed when the class is being initiated.

You can use the **init**() function to assign values to object properties, or other operations that are neccesary to do when the object is being created.

<pre class="file" data-filename="classes.py" data-target="replace">
class Car:
def **init**(model,make,age):
self.model = model
self.make = make
self.age = age

myCar = Car("Audi", "A1", 3)
print(myCar.model)
print(myCar.make)
</pre>

`python classes.py`{{execute}}

## Functions

Objects can also contain functions that belong to that class

<pre class="file" data-filename="classes.py" data-target="replace">
def **init**(model,make,age):
self.model = model
self.make = make
self.age = age

    def printCarFunction(self)
        print("The car is an " + self.make + self.model + " which is " + self.age + " years old")

myCar = Car("Audi", "A1", 3)
myCar.printCarFunction()
</pre>

`python classes.py`{{execute}}

## Self!

The <mark>self</mark> parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.

It does not have to be named <mark>self</mark>, you can call it whatever you like but it has to be the first parameter of any function in a class

<pre class="file" data-filename="classes.py" data-target="replace">
class NamePrinter:
def**init**(steve, age)
steve.age = age

    def namePrinter(lol):
        print("The age of this person is " + lol.age)

myInstance = NamePrinter(25)
myInstance.namePrinter()
</pre>

`python classes.py`{{execute}}

## Modifying object properties

You can modify properties on objects like this:

<pre class="file" data-filename="classes.py" data-target="replace">
class NamePrinter:
def**init**(steve, age)
steve.age = age

    def namePrinter(lol):
        print("The age of this person is " + lol.age)

myInstance = NamePrinter(25)
myInstance.namePrinter()

myInstance.age = 32
myInstance.namePrinter()
</pre>

`python classes.py`{{execute}}

## Deleting properties

You can use <mark>del</mark> keyword to delete the properties on objects

<pre class="file" data-filename="classes.py" data-target="replace">
class NamePrinter:
def**init**(steve, age)
steve.age = age

    def namePrinter(lol):
        print("The age of this person is " + lol.age)

myInstance = NamePrinter(25)
myInstance.namePrinter()

myInstance.age = 32
myInstance.namePrinter()

del myInstance.age  
myInstance.namePrinter()
</pre>

`python classes.py`{{execute}}

You can also use this to delete objects

<pre class="file" data-filename="classes.py" data-target="replace">
class NamePrinter:
def**init**(steve, age)
steve.age = age

    def namePrinter(lol):
        print("The age of this person is " + lol.age)

myInstance = NamePrinter(25)
myInstance.namePrinter()

myInstance.age = 32
myInstance.namePrinter()

del myInstance
myInstance.namePrinter()
</pre>

`python classes.py`{{execute}}

## The pass statment

<mark>Class</mark> definitions cannot be empty, but if you for some reason have a <mark>class</mark> definition with no content, put in the <mark>pass</mark> statement to avoid getting an error.

```Class Orange pass ```
