## Creating Classes
### DIY Task 
<pre class="file" data-filename="solutionEx1.py" data-target="replace">

class Car():
    model = "BMW"
    passengers = 4
    colour = "red"
    speed = 5

    def calculate_acceleration(self):
        speed = self.speed + 2
        print(self.speed)
        print(speed)

C = Car()
C.calculate_acceleration()

</pre>

`python solutionEx1.py`{{execute}}

## Creating objects from a class
### DIY Task - Basic (Car)

<pre class="file" data-filename="solutionEx2.py" data-target="replace">
class Car(object):
    def __init__(self, model, passengers, colour, speed):
        self.car_type = model
        self.max_passengers = passengers
        self.colour = colour
        self.speed = speed

    def get_car_data(self):
        list = [self.car_type, self.max_passengers, self.colour, self.speed]
        return list

    def calculate_acceleration(self):
        self.speed = self.speed + 2
        print (self.speed)

C = Car("BMW", 4, "purple", 50)
print(C.get_car_data())
C.calculate_acceleration()

</pre>

`python solutionEx2.py`{{execute}}

### DIY Task - Advanced (Car)
<pre class="file" data-filename="solutionEx3.py" data-target="replace">
class Car(object):
    def __init__(self, car, ppl, paint, current_speed, max_speed, cost):
        self.car_type = car
        self.max_passengers = ppl
        self.colour = paint
        self.speed = current_speed
        self.top_speed = max_speed
        self.price = cost

    def get_car_data(self):
        list = [self.car_type, self.max_passengers, self.colour, self.speed, self.top_speed]
        print("""Car Model: %s
Maximum Number of Passengers: %s
Colour of Car: %s
Maximum Speed: %s
Price: %s""" % (self.car_type, self.max_passengers, self.colour, self.speed, self.top_speed))
        return list

    def calculate_acceleration(self):
        self.speed = self.speed + 2
        print (self.speed)

C = Car("farrari", 4, "red", 500, 1000, 999.99)
C.get_car_data()
C.calculate_acceleration()

</pre>

`python solutionEx3.py`{{execute}}

### DIY Task - Advanced (Ice Cream)

<pre class="file" data-filename="solutionEx4.py" data-target="replace">
class Customer(object):
  name = ""
  nb_products = 0
  total_cost = 0.00
  special = False
  cost_for_week = 0.00
  list = ["Roxanne", "Jinx", "Jamal", "Litty", "Trixy"]
  
  def create_receipt(self):
    self.cost_for_week += self.total_cost
    if (self.special):
        self.total_cost /= 2
        
    print("Receipt Details: \nName: " + self.name + "\nNumber of Products Bought: " + str(self.nb_products) + "\nTotal Cost: £" + str(self.total_cost))
  
  def isSpecial(self):
    if (self.cost_for_week > 30):
      self.special = True
      list.add(self.name)
      
    if (self.name in self.list):
      self.special = True

C = Customer()
flag = True
while(flag):
    C.name = input("Customer Name: ")
    C.nb_products = int(input("Number of Products: "))
    C.total_cost = C.nb_products * 2
    C.isSpecial()
    C.create_receipt()
    
    finish = input("More Customers? [y/n] ")
    if (finish == "n"):
        flag = False
</pre>

`python solutionEx4.py`{{execute}}


## Pokemon!

### DIY Task Using Our New Skills

<pre class="file" data-filename="solutionEx5.py" data-target="replace">
</pre>

`python solutionEx5.py`{{execute}}


## Learning Inheretence 

### DIY Inheretence Scenario

<pre class="file" data-filename="solutionEx6.py" data-target="replace">
</pre>

`python solutionEx6.py`{{execute}}

### Extension Task: Coding the Eevee Evolutions


<pre class="file" data-filename="solutionEx7.py" data-target="replace">
</pre>

`python solutionEx7.py`{{execute}}



