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

When we create an object of a class, we can pass in the unique variables that define that object:

<pre class="file" data-filename="constructors.py" data-target="replace">

class Car():
  def __init__(self, model, year):
    self.model = model
    self.year = year

  def info(self):
    print("The model of the car is " + self.model + " made in " + self.year)

car1 = Car("Volvo", 2010)
car2 = Car("Nissan", 2020)

car1.info()
car2.info()
</pre>

`python constructors.py`{{execute}}


