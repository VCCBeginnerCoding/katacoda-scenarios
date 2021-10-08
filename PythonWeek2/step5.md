# Indexing lists and Changing Values

To change the value of an item in a list, you need to first know it's position in the list (known as its index in the list). For instance, if we wanted to change the name of "Jusin" in the below list to "Justin" we would need to know that their name is in position 3 of the list as we previously stated. Knowing this we can assign the value of "Justin" to that position in the list (index), overwriting the variable already in that position, as shown below:

`
    names = ["Ellie", "Dan", "Perry", "Jusin"]
    names[3] = "Justin"
    print(names)`{{execute}}

This code replaces the variable "Jusin" in the list with "Justin" because we are saying to the program, replace the variable at position 3 in the list with this variable after the equals sign. The format of changing values is shown below:

`listname[index of variable to change] = new value of variable`{{execute}}

We can use the same function to copy one variable of the list into another spot in the variable, such as replacing "Dan" with "Justin" so there are two "Justin"s in the list, as shown below:

`
    names[1] = names[3]
    print(names)`{{execute}}

We know that the position of the "Dan" variable is 1 so we can replace that variable using the same function we did in the previous example, but this time replacing the "Dan" variable with the value of the variable in position 3 of the list (i.e. "Justin").

This function can also be used to copy full lists into new varaibles:

`
    names_copy = names`{{execute}}

Just be aware that in python this function is called **passing by reference** and any changes you make to the new list will also be applied to the original version. As shown below:

`
    names = ["Ellie", "Dan", "Perry", "Justin"]

    names_copy = names
    names_copy[0] = "Not Ellie"

    print(names_copy)
    print(names)`{{execute}}


There are ways that you can copy over just certain variables into the new list and ways you can copy a list and alter it without changing the original, this is called **passing by value**. We will discuss this later on in this weeks session. 

</br>

## Methods:
You are probably wondering at this point how you get the position (index) of a variable in a list when you don't know where it is. In Python there are things called methods on each of the Data types which help you do simple tasks easily without having to write the code yourself. One instance of these methods on the list class is index(). This method is useful for cases like the one we just mentioned as it finds the position (index) of a variable in a list for you. Once you have got this position, you can then edit the variable as normal. This method is particularly useful when you have quite large lists that you need to find variable indexes in. Below is an example of getting the index of the variable "Perry" from the names list:

`
    names = ["Ellie", "Dan", "Perry", "Justin"]

    index_of_perry = names.index("Perry")`{{execute}}

As you can see, you call the method (which means you run it) by first writing the list name you want to call it on, followed by a period and then in brackets the variable you wish for it to search for and get the index of in the list.

Something which you may find helpful is that when you try and retrieve a variable from the list by putting the index -1, you will retrieve the last variable in the list. This is very useful when working with large lists. Try running the piece of code below and see what variable is retrieved:

`
    food = ["Apple", 3, "Chocolate", 3, "Sandwhich", 4, "Cake", 1]
    print(food[-1])`{{execute}}

Now try and run the above code with -2 instead. What variable is it retrieveing now?
