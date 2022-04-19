# What is Inheritance?
Inheritance refers to defining a new class with little or no modification to an existing class. The descendant class is a child class which inherits the attributes/methods from the base and/or parent class. It's used in order to reduce repitition of code. See pre-reading for more details.

<pre class="file" data-filename="inheritExample.py" data-target="replace">
class Parent(object):
  pass
  
class Child(Parent):
  pass
</pre>

`python inheritExample.py`{{execute}}

## How to Code Inheritance

<br></br>
<p align="center">
  <img width="500"  alt="image" src="https://www.learnbyexample.org/wp-content/uploads/python/Python-Inheritance-Illustration.png">
</p>
<br></br>

<pre class="file" data-filename="inheritEx1.py" data-target="replace">
class Vehical(object):       # Parent/Super class
  type = "vehical"
  
  def __init__(self, seats, colouring):
    self.nb_of_seats = seats
    self.colour = colouring
      
  def specs(self):
    print("I am a " + self.type + ". I have " + str(self.nb_of_seats) + " seats and I am " + self.colour)

class Car(Vehical):       # Child/Sub class to Parent
    type = "car"
    def description(self):
        print("This description is only for cars")
        
    
vehical = Vehical(4, "red")
car = Car(2, "blue")
vehical.specs()
car.description()
car.specs()

</pre>

`python inheritEx1.py`{{execute}}

<br></br>

## DIY Inheritance Scenario
<img width="308"  align="right" alt="image" src="https://ds055uzetaobb.cloudfront.net/brioche/uploads/7vXgCqKOYV-lotr.png?width=2400">
To the right is a class heirarchy diagram for you to practice from.<br></br>Note that dragons and orcs both have a colour, size and an enemies list.<br></br>However, they don't share all of the same characteristics. For instance, Orcs can carry a weapon(s).<br></br>The rest of the features are up to you. Also note that you do not have to include the suggestions above, they are to help you get an idea of what to do.
<br></br>

**Terminology**
<ul>
  <li>Character = Base Class (this is also a parent class)</li>
  <li>Monster = Child class to 'Character'. Parent class to 'Dragon' and 'Orc'</li>
  <li>Hero = Child class to 'Character'</li>
  <li>Dragon = Child class to 'Monster'</li>
  <li>Orc = Child class to 'Monster'</li>
</ul>


