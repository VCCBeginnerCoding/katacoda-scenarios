We mentioned this previously, but lists can also be put as elements of a list, this is called nested lists. You can declare them just like you do with normal lists, however you will have another set of square brackets within your list which contains the list element, as shown in the example below:

<pre class="file" data-filename="nestedlist.py" data-target="replace">
allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
print(allTheNames)
</pre>

Copy the code above over to the editor and then press
`python nestedlist.py`{{execute}}

In the above nested list, there are two elements which are both lists of names. As you can see this can be a little difficult to see where one list ends and another begins, especially as your list elements grow larger and there are more of them within one list. It becomes even harder to tell if you have lists nested within your nested lists. So paying attention to where each square bracket starts and ends can save you a lot of headaches. 

Below is another example of how you may use nested lists in a program:

<pre class="file" data-filename="shoppingList.py" data-target="replace">
shoppingList = [['Tomatoes', 4, 2.50], ['Cake', 1, 5], ['Potatoes', 3, 1.75]]
print(shoppingList)
</pre>

Copy the code above over to the editor and then press
`python shoppingList.py`{{execute}}

</br>

This is just a brief introduction into nested lists, we do not have time to cover them further in our course, but below are some further reading links if you wish to learn more about them: </br>
https://www.javaexercise.com/python/python-list-of-lists </br>
https://www.learnbyexample.org/python-nested-list/ </br>