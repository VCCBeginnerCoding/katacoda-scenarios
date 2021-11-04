You were just introduced in the previous step to one of the methods you can use on a list, called index(), which just lets you retrieve the index of a variable within a list. 

Now we're going to explore some more of the functions and methods which can be used on lists that you will find useful. You will learn more about function and methods in next weeks session.

*__Note:__ In the future we will call variables within lists 'elements', as this helps remove any confusion that could occur as to what variable is being referred to.*


</br>

## **Max and Min**

Two such functions will likely seem familiar, max() and min(). As you can probably guess, max() finds the largest number in an list and min() finds the smallest, as shown below:

<pre class="file" data-filename="minmax.py" data-target="replace">
    numbers = [10, 90, 23, 46, -20]

    smallest_number = min(numbers)
    largest_number = max(numbers)

    print(smallest_number) 
    print(largest_number)
</pre>

Copy the code above over to the editor and then press
`python minmax.py`{{execute}}

</br>

## **Len**

Another function which you will likely use quite regularly is the len() function. This function takes the list's name as an argument, and returns the number of elements currently stored inside the list (i.e. the length of the list). Below is an example of using the len() method:

<pre class="file" data-filename="len.py" data-target="replace">
    numbers = [10, 90, 23, 46, -20]
    length = len(numbers)

    print(length)
</pre>

Copy the code above over to the editor and then press
`python len.py`{{execute}}

If you run this code you will see the number 5 is printed. You may have thought it would be 4 because of the indexing we explained to you earlier, however the length function does not care about indexes, it only counts how many elements are in a list.

</br>

## **Sort**

Another method you should know about is the sort() method. This method sorts a list into either ascending or descending order. Below is an example of the sort function being used on a list of numbers:

<pre class="file" data-filename="sort.py" data-target="replace">
    numbers = [10, 90, 23, 46, -20]
    numbers.sort()
    print(numbers)
</pre>

Copy the code above over to the editor and then press
`python sort.py`{{execute}}

As you can see in the above code, the original numbers array is manipulated by the sort, it does not create a copy. When you run the code you should see that by default the sort function sorts by ascending order. You can tell it to sort by descending order by passing in the argument "reverse = True" as shown below:

<pre class="file" data-filename="sort.py" data-target="replace">
    names = ["Ellie", "Dan", "Perry", "Justin"]
    sorted_names = names.sort(reverse=True)

    print(sorted_names)
</pre>

Copy the code above over to the editor and then press
`python sort.py`{{execute}}

</br>

## **Copy**

For lists there is a copy() method which lets you make a new version of a list and change that version without altering the original version. Below is an example of it being used:

<pre class="file" data-filename="copy.py" data-target="replace">
    numbers = [10, 90, 23, 46, -20]
    numbers_copy = numbers.copy()
    numbers_copy[1] = "Changing"
    print(numbers)
    print(numbers_copy)
</pre>

Copy the code above over to the editor and then press
`python copy.py`{{execute}}

When you run the code you can see that the original numbers list has not been altered, however the numbers_copy list has the value "Changing" as the second element instead of 90. This is how we approach copying and manipulating versions of strings without altering the original if you do not wish to.