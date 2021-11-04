We mentioned this previously, but lists can also be put as elements of a list, this is called nested lists. You can declare them just like you do with normal lists, however you will have another set of square brackets within your list which contains the list element, as shown in the example below:

<pre class="file" data-filename="nestedlist.py" data-target="replace">
allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
print(allTheNames)
</pre>

Copy the code above over to the editor and then press
`python nestedlist.py`{{execute}}

In the above nested list, there are two elements which are both lists of names. As you can see this can be a little difficult to see where one list ends and another begins, especially as your list elements grow larger and there are more of them within one list. It becomes even harder to tell if you have lists nested within your nested lists. So paying attention to where each square bracket starts and ends can save you a lot of headaches. 

You are probably wondering why you would want to do nested lists if they are difficult to identify, the answer is simple, most of the data you store and work with has multiple values associated with it, such as a shopping list, which has each item and then the price for that item or the quantity of that item you bought. Therefore using nested lists helps show the associated information without having to create multiple seperate lists and maintain that each related element has the same index in each list. Below is an example of how you may use nested lists in a program:

<pre class="file" data-filename="shoppingList.py" data-target="replace">
shoppingList = [['Tomatoes', 4, 2.50], ['Cake', 1, 5], ['Potatoes', 3, 1.75]]
print(shoppingList)
</pre>

Copy the code above over to the editor and then press
`python shoppingList.py`{{execute}}

In the above example you can see each food item is in its own list within the overall shopping list and has its own quantity and price associated with it in the same list. 

So what if we wanted to store the names previous allTheNames list with the associated session those instructors help run? We would then have to use another layer of nesting as shown below:

<pre class="file" data-filename="names.py" data-target="replace">
allTheNames = [['Crash courses', ['Ellie', 'Perry', 'Dan', 'Justin']], ['Challenge centres', ['Domas', 'Alex', 'Raphael', 'Hugo']]]
print(allTheNames)
</pre>

Copy the code above over to the editor and then press
`python names.py`{{execute}}

So as you can see, nested listing can be complex, but they allow you to store a large amount of associated information in just one large list. 

</br>

You can change the value of elements and full lists in nested lists in the same way that you do with normal lists, like in the code below:

<pre class="file" data-filename="names.py" data-target="replace">
allTheNames = [['Crash courses', ['Ellie', 'Perry', 'Dan', 'Justin']], ['Challenge centres', ['Domas', 'Alex', 'Raphael', 'Hugo']]]
allTheNames[0][1] = ['Max', 'Dan']
print(allTheNames)
</pre>

Copy the code above over to the editor and then press
`python names.py`{{execute}}

</br>

That is just a brief introduction into nested lists and why they can be very useful, in future sessions we will go into further depth on how you can work with lists and nested lists more easily. 