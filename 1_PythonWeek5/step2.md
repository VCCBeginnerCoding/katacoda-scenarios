Messy Terminal? `clear`{{execute}} it.
<hr>

## Basic Structure

Classes in Python are created using the `class` keyword:

<pre class="file" data-filename="snippet.py" data-target="replace">

class exampleOne():
  number = 5
</pre>

Note that the `number` value is an <b>attribute</b> of `example()`
<br>

## Objects

In order to use the classes we create, we must create objects of them. These use the class as a blueprint to their creation - for example:

<pre class="file" data-filename="objectCreation.py" data-target="replace">

class exampleTwo():
  number = 5
  
val = exampleTwo()
print(val)
</pre>

`python objectCreation.py`{{execute}}

## Self

In order to give classes methods that will define an object's functions, we must first look at the `self` keyword in Python.

The `self` parameter is used as a reference to the current instance of the class, and is used to access variables that belong to a particular object that you create. This means that you can create multiple instances of a class, and access each of their attributes independantly. 

You will see this keyword used in examples below.

## Methods and Constructors

Classes have their own methods inside them, which give an object its functions. Once an object has been created, it can then directly call these methods. 

To access the attributes within a class, it is necessary to have a constructor defining these variables. This is a special method defined by the keyword `__init__`.

When we create an object of a class, we have to ensure that we pass in the attributes required in that class's constructor. 

<b>Note for object creation:</b> You don't have to pass in `self` when creating the object, you only need to pass in the variables stated in `__init__`. 
<b>Note for class methods:</b> You only have to pass in `self` into the method to ensure that it can access the `self.variable` within the class.

<pre class="file" data-filename="constructors.py" data-target="replace">

class Car():
  def __init__(self, make, year):
    self.make = make
    self.year = year

  def info(self):
    print("The make of the car is " + self.make + " made in " + self.year)

car1 = Car("Volvo", 2010)
car2 = Car("Nissan", 2020)

car1.info()
car2.info()
</pre>

`python constructors.py`{{execute}}


