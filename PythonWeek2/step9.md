We mentioned this previously, but lists can also be put as elements of a list, this is called nested lists. You can declare them just like you do with normal lists, however you will have another set of square brackets within your list which contains the list element, as shown in the example below:

`
    allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
    print(allTheNames)`{{execute}}

In the above nested list, there are two elements which are both lists of names. As you can see this can be a little difficult to see where one list ends and another begins, especially as your list elements grow larger and there are more of them within one list. It becomes even harder to tell if you have lists nested within your nested lists. So paying attention to where each square bracket starts and ends can save you a lot of headaches. 

You are probably wondering why you would want to do nested lists if they are difficult to identify, the answer is simple, most of the data you store and work with has multiple values associated with it, such as a shopping list, which has each item and then the price for that item or the quantity of that item you bought. Therefore using nested lists helps show the associated information without having to create multiple seperate lists and maintain that each related element has the same index in each list. Below is an example of how you may use nested lists in a program:

`
    shoppingList = [['Tomatoes', 4, 2.50], ['Cake', 1, 5], ['Potatoes', 3, 1.75]]
    print(shoppingList)`{{execute}}

In the above example you can see each food item is in its own list within the overall shopping list and has its own quantity and price associated with it in the same list. 

So what if we wanted to store the names previous allTheNames list with the associated session those instructors help run? We would then have to use another layer of nesting as shown below:

`
    allTheNames = [['Crash courses', ['Ellie', 'Perry', 'Dan', 'Justin']], ['Challenge centres', ['Domas', 'Alex', 'Raphael', 'Hugo']]]
    print(allTheNames)`{{execute}}

So as you can see, nested listing can complex, but it allows you to store a large amount of associated information in just one large list. 

</br>

## **Retrieving and altering a nested list**

Retrieving an element from a nested list is very similar to how you would do with normal lists, you just need to know the position of the nested list in the overall list and then the position of the element in the nested list, as shown below:

`
    allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
    print(allTheNames[0][1])`{{execute}}

The above code prints the element "Perry" when it is ran. This is because you are asking for the list in the first position of the overall list (at index 0) in the first set of square brackets and then asking for the second element (at index 1) within that smaller list in the second square brackets.

What do you think the following code will print when you run it?

`
    allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
    print(allTheNames[1])`{{execute}}

As you likely saw, it prints the entire second list of names as it is asked to retrieve the second element in the overall list (at index 1).

To alter an element within a nested list you can use the logic used above combined with what you learnt earlier about changing elements within a list, as shown below:

`
    allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
    allTheNames[0][2] = "Max"
    print(allTheNames)`{{execute}}

In the above code "Perry" in the first nested list has been changed to "Max". As you can see from the code, you just have to provide the two indexes for where the element is located in both of the lists and then you can change the variable to whatever you wish.

You can also change an entire nested list if you wish, like so:

`
    allTheNames = [['Ellie', 'Perry', 'Dan', 'Justin'], ['Domas', 'Alex', 'Raphael', 'Hugo']]
    allTheNames[1] = ["Max", "Frankie", "Alisha"]
    print(allTheNames)`{{execute}}

When you run this code you can see that it has replaced the entire second nested list (['Domas', 'Alex', 'Raphael', 'Hugo']) with a new nested list (['Max', 'Frankie', 'Alisha']).

</br>

That is just a brief introduction into nested lists and why they can be very useful, in future sessions we will go into further depth on how you can work with lists and nested lists more easily. 