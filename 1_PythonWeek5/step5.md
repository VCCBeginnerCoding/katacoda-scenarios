# What is Inheritance?
Inheritance refers to defining a new class with little or no modification to an existing class. The descendant class is a child class which inherits the attributes/methods from the base and/or parent class. See pre-reading for more details.

<br></br>
<p align="center">
  <img width="500"  alt="image" src="https://www.learnbyexample.org/wp-content/uploads/python/Python-Inheritance-Illustration.png">
</p>
<br></br>

## How to Code Inheritance

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
##############################################<br></br>###############################################################<br></br>##################################### 
<br></br>


