Messy Terminal? `clear`{{execute}} it.
<hr>

Now we're going to create some lists and work with them as practice.
Tom, Mike and Lily all go shopping at different supermarkets and want to compare their weekly shop. Below is each of their shopping lists:

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

Now do the following steps using the shopping list data provided and the knowledge you have gained about nested lists:

- Create a list that contains all of Lily's items 
- Sort the list of her items (in ascending order)
- Add three food items to Lily's shopping list: Chocolate, Marshmallows and Strawberry jam
- Remove the Ice cream from Lily's shopping list 
- Create the same kind of list for Mike and for Tom

To write your own code simply create a new Python file: `listsexercise.py`{{open}}

Write your code in the editor that has now opened and when you are ready, execute it with
`python listsexercise.py`{{execute}}

<hr>
Hints:
- print statements can be helpful to understand what's going on inside your lists and if you're getting expected outputs. To print a list the syntax is print(list_name)
- the format for a list is list = ['a', 2, 2.5]
- .sort() sorts the list 
- .append() saves to list 
- .remove() removes from list 
- index of a list starts at 0 
<hr>

As further work you can do the following steps to explore nested lists:
- Make the Shopping lists nested by adding the price of each item next to the item name (i.e. [Salsa, 2.50]). For the items that do not have a price, you can make one up
- Create an overall shoppingLists list with all 3 people's list within it
- Retrieve the cost of Mike's Paninis
- Edit the cost of Tom's Milk to £1 instead
- Delete the Eggs and their cost from Lily's shopping list
