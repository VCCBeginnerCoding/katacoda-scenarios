Now let's move onto something new, Lists. Lists are a new type of Data Type which you haven't met yet, they are a structure which allows us to store multiple variables within them. 

**Why do we need to store multiple variables?** In some programs there are many variables that the program has to work with, sometimes up to the hundreds or thousands, having a list to store these in and handle them saves a lot of time and makes the code a lot more efficient.

</br>

## Initialising Lists

Lists are multi-value variables which can have variables within them all of the same type or of different types. Some of them may be integers, strings, booleans or even other lists (this is called nested listing, we will come back to this). Below is an example of how to declare a list, in this instance we are declaring a list of strings and a list of strings and numbers:

`
    names = ["Ellie", "Dan", "Perry", "Justin"]
food = ["Apple", 3, "Chocolate", 3, "Sandwhich", 4, "Cake", 1]print(names)
print(food)`{{execute}}

As you can see, there are some similarities to how you declare a variable, you need to:
- Give a name for the list
- Have an equals sign which declares it is a variable and sets it to the values you put on the right side of the equals sign

But you also need to seperate each invidivual variable with a comma within the square brackets.

You can also declare a list using pre-existing variables as shown below:

`
    name1 = "Ellie"
name2 = "Dan"
names = [name1, name2]
print(names)`{{execute}}

*It is important to remember for the future that elements in a list are always **numbered starting from zero**, so in our first 'names' example "Ellie" is the first element and is in position 0 of the list. The final element is "Justin" and is in position 3 of the list.*