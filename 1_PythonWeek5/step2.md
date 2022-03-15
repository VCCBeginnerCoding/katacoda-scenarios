Now that you have had an introduction to the concept of classes and OOP, we will now walk you through the basics of how to write and use classes.

# Constructors
The first thing you will see in a Python class is what is known as a "constructor". This is a method which is automatically called when an object is created. An example of a constructor can be seen in the code snippet below:

<pre class="file" data-filename="constructor.py" data-target="replace">
class Person:

  # Constructor which initialises the class variables
  def __init__(self, name, age, height):
    self.name = name
    self.age = age
    self.height = height

# Create an object which is an instance of the "Person" class
newPerson = Person("Aymen", 24, 186)

# Print the attributes associated with this object
print(newPerson.name)
print(newPerson.age)
print(newPerson.height)

</pre>

`python constructor.py`{{execute}}

# The "self" parameter
One of the most important elements of classes in Python is the "self" parameter. It is difficult to see its use with a simple code example, but essentially it means that each object that was created from a given class template has its own attributes and methods. The "self" parameter is where the object name is passed into when an object is created. 

It is worth noting that you do not need to use the word "self" (Python will just use the first argurment in the "init" function) but software engineers will typically stick to using "self" as a convention.

https://www.w3schools.com/python/python_classes.asp
https://stackoverflow.com/questions/2709821/what-is-the-purpose-of-the-word-self

# Methods
You can write methods which belongs to a class. We can simplify the example above by writing a method which prints all of the attributes of a given class.

<pre class="file" data-filename="methods.py" data-target="replace">
class Person:

  # Constructor which initialises the class variables
  def __init__(self, name, age, height):
    self.name = name
    self.age = age
    self.height = height
    
  def printDetails(self):
    print(name)
    print(age)
    print(height)

# Create an object which is an instance of the "Person" class
newPerson = Person("Aymen", 24, 186)

# Call the printDetails() method
newPerson.printDetails()

</pre>

`python methods.py`{{execute}}


