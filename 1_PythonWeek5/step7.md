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
class Pokemon(object):
    partner = ""
    previous_partners = []
    released = 0
    
    def choosePartner(self):
        empty = False
        if (self.partner == ""):
            empty = True
            print("Your current partner is " + self.partner)
        
        chosen = int(input("""Select A Partner:
    1. Pikachu
    2. Lucario
    3. Bulbasaur
    4. Charmander
    5. Eevee
    """))
        
        if (chosen == 1):
            if not (empty):
                self.previous_partners.append(self.partner)
                self.released += 1
            self.partner = "Pikachu"
        elif (chosen == 2):
            if not (empty):
                self.previous_partners.append(self.partner)
                self.released += 1
            self.partner = "Lucario"
        elif (chosen == 3):
            if not (empty):
                self.previous_partners.append(self.partner)
                self.released += 1
            self.partner = "Bulbasaur"
        elif (chosen == 4):
            if not (empty):
                self.previous_partners.append(self.partner)
                self.released += 1
            self.partner = "Charmander"
        elif (chosen == 5):
            if not (empty):
                self.previous_partners.append(self.partner)
                self.released += 1
            self.partner = "Eevee"
        else:
            print("Not an option. Pick again...")
            self.choosePartner()
    
    def details(self):
        if (self.partner == "Pikachu"):
            print("Pikachu is yellow with red cheeks")
        elif (self.partner == "Lucario"):
            print("Lucario is a blue fighter - bestie")
        elif (self.partner == "Bulbasaur"):
            print("Bulbasaur is a leafy starter")
        elif (self.partner == "Charmander"):
            print("Charmande is fire king")
        elif (self.partner == "Eevee"):
            print("Eevee has hidden power")
        else:
            print("No Partner")
            
    def getPartner(self):
        if (self.partner != ""):
            print(self.partner)
        else:
            print("No Partner")

    def getPrevious(self):
        print(self.previous_partners)
        print("You have release: ",self.released," pokemon")

flag = True
P = Pokemon()
while (flag):
    action = input("""Choose Option:
    1. View Partner
    2. Choose Partner
    3. View Previous Partners
    4. Exit
    """)

    if (action == "1"):
        P.getPartner()
    elif (action == "2"):
        P.choosePartner()
        P.details()
    elif (action == "3"):
        P.getPrevious()
    elif (action == "4"):
        flag = False
    else:
        print("Not an option")
</pre>

`python solutionEx5.py`{{execute}}


## Learning Inheretence 

### DIY Inheretence Scenario

<pre class="file" data-filename="solutionEx6.py" data-target="replace">
import random

class Character(object):
    name = ""
    age = ""
    weapon = False
    level = 0
    
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def description(self):
        print("Character Features: Name, Age, Weapon, level")

class Hero(Character):
    weapon = True
    weapon_vault = ["sword", "shield"]
    monsters_killed = 0
    dragons_killed = 0
    monster_encountered_list = {"Dragon":0, "Orc":0}
    defeats = 0
    exp = 0

    def description(self):
        self.calc_level()
        print("\n" + self.name + "'s Characteristics: I am " + str(self.age) +" years old and I am at level", self.level)
        print("Weapons: " + str(self.weapon_vault))
        print("Kills: " + str(self.monsters_killed))
        print("Dragons Killed: " + str(self.dragons_killed))
        print("History: " + str(self.monster_encountered_list))
        print("Defeats: " + str(self.defeats))
        print("Experience: " + str(self.exp) + "\n")


    def attack(self):
        options = ["Dragon", "Orc"]
        opponent = random.choice(options)

        if (opponent == "Dragon"):
            D = Dragon("","")
            D.description()
            if (self.level < 6):
                print("you have been defeated by a Dragon")
                self.monster_encountered_list["Dragon"] += 1 
                self.defeats += 1
            else:
                print("you won!")
                self.dragons_killed += 1
                self.monsters_killed += 1
                self.monster_encountered_list["Dragon"] += 1 
                self.exp += 30
                if (self.exp >= 100):
                    self.level += 1
                    self.exp -= 100

        else:
            O = Orc("","")
            O.description()
            list = ["won", "fail", "fail"]
            result = random.choice(list)
            if (result == "fail"):
                print("you have been defeated by an Orc ")
                self.monster_encountered_list["Orc"] += 1 
                self.defeats += 1
            else:
                print("you won!")
                self.monsters_killed += 1
                self.monster_encountered_list["Orc"] += 1 
                self.exp += 10
                if (self.exp >= 100):
                    self.level += 1
                    self.exp -= 100

    def calc_level(self):
        if (self.dragons_killed != 0):
            if (self.monster_encountered_list["Dragon"] != 0):
                if (self.dragons_killed % 5 == 0):
                    if (self.level > 1):
                        print(self.dragons_killed)
                        self.level *= self.dragons_killed/5
                        print("Killing Dragons Have Increased Your Level!")

class Monster(Character):
    colour = "red"
    size = 200
    enemies = ["Hero"]
    level = 5

class Dragon(Monster):
    element = ["Fire", "Water", "Air", "Earth"]
    friendly = [True, False]

    def description(self):
        f = random.choice(self.friendly)
        if (f):
            print("I'm friendly, I swear! Please don't kill me :(")
        else:
            print("ROOOOAR!")

class Orc(Monster):
    weapon = "Dagger"

    def description(self):
        print("DIE DIE DIE")


print("""
Menu:
 1. Create A Hero
 2. View Hero Details
 3. Attack A Monster
 4. Exit
 """)
H = ""
loop = True
while (loop):
    try:
        action = int(input("Select Menu Item: "))
    except ValueError:
        continue
    
    if (action == 1):
        name = input("What is your character's name? ")
        age = int(input("How old is your character? "))
        H = Hero(name, age)
        print()
        
    elif (action == 2):
        if (H != ""):
            H.description()
        else:
            print("You need to create a character first\n")
            
    elif (action == 3):
        H.attack()

    elif (action == 4):
        print("Goodbye")
        loop = False
    
    else:
        print("That is not a menu option. Please pick 1, 2, 3 or 4.")
</pre>

`python solutionEx6.py`{{execute}}

### Extension Task: Coding the Eevee Evolutions


<pre class="file" data-filename="solutionEx7.py" data-target="replace">
</pre>

`python solutionEx7.py`{{execute}}



