Messy Terminal? `clear`{{execute}} it.
<hr>

Lists can grow to any length you wish them to be (have as many elements as you want), can be added to at any point and any element can be changed at any point in time, as you saw earlier in this session. Methods for adding elements to a list are important to know as you will be using them regulalry. Below we will explore some different methods you can use to do so.

</br>

## **Append**
The append method is the default method most people use when adding an element to a list. It is simple and easy to understand and quite efficient, as it just adds the element to the end of the list and increases the lists length by one, as shown below:

<pre class="file" data-filename="append.py" data-target="replace">
names = ["Ellie", "Dan", "Perry", "Justin"]
names.append("Max")
print(names)
print(len(names))
</pre>

Copy the code above over to the editor and then press
`python append.py`{{execute}}

When you run the code you should see that the variable "Max" has now been added to the end of the list and the list length is now 5.

</br>
