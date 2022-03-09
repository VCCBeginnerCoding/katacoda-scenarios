Messy Terminal? `clear`{{execute}} it.
<hr>

You were just introduced in the previous step to one of the methods you can use on a list, called index(), which just lets you retrieve the index of a variable within a list. 

Now we're going to explore some more of the functions and methods which can be used on lists that you will find useful, starting with the Sort function. You will learn more about function and methods in next weeks session.

*__Note:__ In the future we will call variables within lists 'elements', as this helps remove any confusion that could occur as to what variable is being referred to.*


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