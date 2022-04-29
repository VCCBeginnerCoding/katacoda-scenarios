## Pokemon! Gotta Catch Em All!
Who here is a pokemon fan???

<img width="209" align = "right" alt="image" src="https://user-images.githubusercontent.com/60058170/158644283-b76d6cbf-fd34-4768-b1ef-c6753355936b.png">

**If you are:** you're awesome. <br>
**If you aren't:** tough because I am.

<img width="210" align = "right" alt="image" src="https://user-images.githubusercontent.com/60058170/158645120-488f50c3-3d06-477c-a1e5-a30b9e2aaf50.png">
<img width="210" align = "right" alt="image" src="https://user-images.githubusercontent.com/60058170/158645318-0e381115-ac28-4ebb-a433-1b5cbd7480fc.png">

<br>

**Pokemon:**
<ul>
  <li>Pikachu</li>
  <li>Lucario</li>
  <li>Bulbasaur</li>
  <li>Charmander</li>
  <li>Eevee</li>
</ul>

<img width="200" align = "right" alt="image" src="https://user-images.githubusercontent.com/60058170/158645552-288a5ca1-8339-40f2-aef9-4e66cb812903.png">

<br>

_Feel free to add more. These are just to start you off._

<img width="180" align = "right" alt="image" src="https://user-images.githubusercontent.com/60058170/158644727-08e26840-b106-4238-9ca2-de1d643876be.png">

<br>

You are going to create classes for a pokedex. Once your code is finished the user should be able to view details of a pokemon that they choose. They should also be able to pick a pokemon to be their partner (they are only allowed one). At any point they can also view who their partner is, any previous partners that they have had and the number of times they've released a pokemon.

**Note:** Every the user picks a new partner. If they already have one, that partner is released.

Are you up for the challenge?

<pre class="file" data-filename="pokemon.py" data-target="replace">
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

`python pokemon.py`{{execute}}

