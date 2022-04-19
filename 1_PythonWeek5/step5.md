# What is Inheritance?
Inheritance refers to defining a new class with little or no modification to an existing class. The descendant class is a child class which inherits the attributes/methods from the base and/or parent class. See pre-reading for more details.


## How to Code Inheritance
<pre class="file" data-filename="inheritEx1.py" data-target="replace">
class Parent(object):       # Parent/Super class
  type = "vehical"
  
  def __init__(self, seats, colouring):
    self.nb_of_seats = seats
    self.colour = colouring
      
  def specs(self):
    print("I am a " + self.type + ". I have " + str(self.nb_of_seats) + " seats and I am " + self.colour)

class Child (Parent):       # Child/Sub class to Parent
    type = "car"
    def description(self):
        print("This description is only for cars")
        
    
vehical = Parent(4, "red")
car = Child(2, "blue")
vehical.specs()
car.description()
car.specs()

</pre>

`python inheritEx1.py`{{execute}}

## Inheritance Scenario
