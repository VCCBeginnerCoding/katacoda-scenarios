Messy Terminal? `clear`{{execute}} it.
<hr>

Elements can also be removed from a list at any point in time, we will explore some of the apporaches you can use to remove elements from a list below.

</br>

## **Remove**
The remove method allows you to specify the value you want to remove from the list rather than using the index of the variable. Below is an exmample of us removing a number from the same list using the remove() method:

<pre class="file" data-filename="remove.py" data-target="replace">
numbers = [10, 90, 23, 46, -20]
numbers.remove(90)
print(numbers)
print(len(numbers))
</pre>

Copy the code above over to the editor and then press
`python remove.py`{{execute}}

As you can see it removes the element 90 from the list and reduces the length of the list by one. An issue with this method is if there are multiple instances of 90, what will happen? Try and run some code with two 90s in the list and see. 

</br>

As you  may have noticed when removing any element from a list, all the other elements that come after that element in the list change position, therefore have different indexes. This is important as it means you could accidentally delete the wrong element if you try and delete elements concurrently (one after the other), or you may end up retrieving the wrong element as its index may have changed. This is something that you should always keep in mind and adjust your code to. The same issue can occur when you add elements to a list via insertion, since all the elements after the inserted element will have a different index. 