Now that you have had an introduction to the concept of classes and OOP, we will now walk you through the basics of how to write and use classes.

# Constructors
The first thing you will see in a Python class is what is known as a "constructor". This is a method which is automatically called when an object is created.

This can be seen in the code snippet below:
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

# Methods
You can write methods which belong to a class. We can simplify the example above by writing a method which prints all of the attributes of a given class.

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
