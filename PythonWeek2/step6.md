You were just introduced in the previous step to one of the methods you can use on a list, called index(), which just lets you retrieve the index of a variable within a list. 

Now we're going to explore some more of the functions and methods which can be used on lists that you will find useful. Functions get data, manipulate data and generally return a result. Methods do all of these things and are a specific kind of function, as they belong to the data that they are being called on. A method is owned by the data it works for, while a function is owned by the whole code. This is why with the index method we call it by typing the lists name and then call the function on that list by putting a period. Whereas with other functions below such as the min and max functions, you call the function by passing the list in to the function via the brackets. 

***Note:** In the future we will call variables within lists elements, as this helps remove any confusion that could occur as to what variable is being referred to.*


</br>

## **Max and Min**

Two such functions will likely seem familiar, max() and min(). These functions do basically the same as the code you wrote earlier to find the smallest and largest number in an list, but can do it on a much larger scale so are more efficient to use on bigger lists than writing your own code. As you can probably guess, max() finds the largest number in an list and min() finds the smallest, as shown below:

`
    numbers = [10, 90, 23, 46, -20]

    smallest_number = min(numbers)
    largest_number = max(numbers)

    print(smallest_number) 
    print(largest_number)`{{execute}}

As you can see these functions are called differently and instead have the list of numbers passed into them as an argument. This is because the function can be called on more structures than just a list, you will learn about these other structures as you explore Python further. Over time you will get used to which functions are called in which way as you use them more often in your code. 

</br>

## **Len**

Another function which you will likely use quite regularly is the len() function. This function takes the list's name as an argument, and returns the number of elements currently stored inside the list (i.e. the length of the list). This function is quite useful when you have large lists and you want to know the total size of the list so you can go through each element using something called iteration, which we will cover next week. Below is an example of using the len() method:

`
    numbers = [10, 90, 23, 46, -20]
    length = len(numbers)

    print(length)`{{execute}}

If you run this code you will see the number 5 be printed. You may have thought it would be 4 because of the indexing we explained to you earlier, however the length function does not care about indexes, it only counts how many elements are in a list.

</br>

## **Sort**

Another method you should know about is the sort() method. This method sorts a list into either ascending or descending order, no matter if the list contains strings or integers, though it can only contain elements of the same type. Below is an example of the sort function being used on a list of numbers:

`
    numbers = [10, 90, 23, 46, -20]
    numbers.sort()
    print(numbers)`{{execute}}

As you can see in the above code, the original numbers array is manipulated by the sort, rather than creating a new sorted array. This is similar to what we discussed earlier and should be kept in mind if you ever want to keep the original order of a list.

When you run the code you should see that by default the sort function sorts by ascending order. You can tell it to sort by descending order by passing in the argument "reverse = True" as shown below:

`
    names = ["Ellie", "Dan", "Perry", "Justin"]
    sorted_names = names.sort(reverse=True)

    print(sorted_names)`{{execute}}

Now try and sort a list of different variable types (i.e. integers, strings and booleans) and see what happens.

*That's right, you cannot sort a list which contains different types of variables, it throws an error.*

In this code we passed the argument "reverse = True". Arguments are what are passed into a function to give it the information it needs to perform in the way you want, for example when we called the index method earlier we passed the argument "Perry" into the method so it would search for "Perry" in the list and return the index for that element. 

</br>

## **Copy**

We explored earlier how you can copy a list, however we found that the method was passing by reference, i.e. if you changed the copy you changed the original. To resolve this issue there is a copy() method for lists which passes by value instead, i.e. lets you change the new list without it affecting the original version. Below is an example of it being used:

`
    numbers = [10, 90, 23, 46, -20]
    numbers_copy = numbers.copy()
    numbers_copy[1] = "Changing"
    print(numbers)
    print(numbers_copy)`{{execute}}

When you run the code you can see that the original numbers list has not been altered, however the numbers_copy list has the value "Changing" as the second element instead of 90. This is how we approach copying and manipulating versions of strings without altering the original if you do not wish to.
