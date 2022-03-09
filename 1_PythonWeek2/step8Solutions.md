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
