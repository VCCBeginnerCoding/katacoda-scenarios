Messy Terminal? `clear`{{execute}} it.
<hr>

Shopping lists:

Tom's Sainsburys shopping list:
- Milk - £0.80
- Fajita kit - £2.00
- Salsa - £2.50

Mike's Asda hopping list:
- Strawberries - £2.00
- Paninis - £0.99
- Coronation chicken spread - £1.40

Lily's Aldi shopping list:
- Eggs - £0.75
- Ice Cream - £1.99
- Cake Mix - £1.25

<mark>Basic tasks:</mark> 

- Create a list that contains all of Lily's items 
- Sort the list of her items (in ascending order)
- Add three food items to Lily's shopping list: Chocolate, Marshmallows and Strawberry jam
- Remove the Ice cream from Lily's shopping list 
- Create the same kind of list for Mike and for Tom

<pre class="file" data-filename="BasicTasks.py" data-target="replace">

# Create a list that contains all of Lily's items
lily=["Eggs","Ice cream","Cake mix"]

# Sort Lily's list in ascending order
lily.sort()
print(lily)

# Add three food items to Lily's shopping list: Chocolate, Marshmallows and Strawberry Jam
lily.append("Chocolate")
lily.append("Marshmallows")
lily.append("Strawberry Jam")
print(lily)

# Remove the Ice cream from Lily's shopping list
lily.remove("Ice cream")
print(lily)

# Create the same kind of list for Mike and for Tom
mike=["Strawberries", "Paninis", "Coronation chicken spread"]
tom=["Milk", "Fajita kit", "Salsa"]
print(mike)
print(tom)

</pre>

`python BasicTasks.py`{{execute}}

<hr>

<mark>Further Work:</mark>

- Make the Shopping lists nested by adding the price of each item next to the item name (i.e. [Salsa, 2.50]). For the items that do not have a price, you can make one up
- Create an overall shoppingLists list with all 3 people's list within it
- Retrieve the cost of Mike's Paninis
- Edit the cost of Tom's Milk to £1 instead
- Delete the Eggs and their cost from Lily's shopping list

<pre class="file" data-filename="FurtherWork.py" data-target="replace">

# Make the shopping lists nested by adding the price next to the item name
lily=[["Eggs", 0.75], ["Ice cream", 1.99], ["Cake Mix", 1.25], ["Chocolate", 1.00], ["Marshmallows", 0.50], ["Strawberry Jam", 1.20]]
mike=[["Strawberries", 2.00], ["Paninis", 0.99], ["Coronation chicken spread", 1.40]]
tom=[["Milk", 0.80], ["Fajita kit", 2.00], ["Salsa", 2.50]]
print(lily)
print(mike)
print(tom)

# Make an overall shopping list with all 3 people's lists within it
shoppingLists = lily + mike + tom
print(shoppingLists)

# Retrieve the cost of Mike's Paninis
# If retrieving from Mike's individual list
cost = mike[1][1]
print("The cost of Mikes Paninis are " + str(cost))
 
# If retrieving Mike's Paninis from shoppingLists
cost = shoppingLists[7][1]
print("The cost of Mikes Paninis are " + str(cost))

# Edit the cost of Tom's Milk to £1
# If manipulating Tom's individual list
tom[0][1] = 1.00
print("The new cost of Tom's Milk is " + str(tom[0][1]))

# If manipulating Tom's Milk in shoppingLists
shoppingLists[9][1] = 1.00
print("The new cost of Tom's Milk is " + str(shoppingLists[9][1]))

# Delete the Eggs and their cost from Lily's shopping list
# If removing from Lily's individual list
lily.remove(["Eggs", 0.75])
print(lily)

# If removing Lily's eggs and cost from shoppingLists
shoppingLists.remove(["Eggs", 0.75])
print(shoppingLists)

</pre>

`python FurtherWork.py`{{execute}}