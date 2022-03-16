Messy Terminal? `clear`{{execute}} it.
<hr>

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

print("The smallest number is: " + str(smallest_number)) 
print("The largest number is: " + str(largest_number))
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

If you run this code you will see that the function printed that the length of the numbers array is 5. You may have thought it would be 4 because of the indexing we explained to you earlier, however the length function does not care about indexes, it only counts how many elements are in a list.

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

As you can see by the print of the above code, the original numbers array is manipulated by the sort, it does not create a copy. When you run the code you should see that by default the sort function sorts by ascending order. You can tell it to sort by descending order by passing in the argument "reverse = True" as shown below:

<pre class="file" data-filename="sort.py" data-target="replace">
names = ["Ellie", "Dan", "Perry", "Justin"]
names.sort(reverse=True)

print(names)
</pre>

Copy the code above over to the editor and then press
`python sort.py`{{execute}}