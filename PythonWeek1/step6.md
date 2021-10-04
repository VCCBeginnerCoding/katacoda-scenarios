# Lots of Variables

Remember to clear your terminal with `clear`{{execute}} if it's too messy!

Imagine you want to store 100 values. Do you do this?

```
var1 = int(input())
var2 = int(input())
var3 = int(input())
var4 = int(input())
var5 = int(input())
var6 = int(input())
:
:
```

Of course not! There's where lists come in.

Open new Python file: `lists.py`{{open}}

<pre class="file" data-filename="lists.py" data-target="replace">
myNumbers = [10, 5, 7, 2, 1]
print(myNumbers)
</pre>

`python lists.py`{{execute}}

# Counting from Zero

That's right, we count from zero! If we want to change the first value ```10``` within ```myNumbers``` we do this:

<pre class="file" data-filename="lists.py" data-target="replace">
myNumbers = [10, 5, 7, 2, 1]
print("Original list content:", myNumbers)

# Change item 0 on the list from the value 10 to the new value 9999
myNumbers[0] = 9999
print("New list content: ", myNumbers)
</pre>

`python lists.py`{{execute}}

# List Mayhem

Lists can contain a mix of data types.

```my_list = [1, None, True, "I am a string", 256, 0]```

Lists can also be nested inside of lists.


```my_list = [1, 'a', ["list", 64, [0, 1], False]]```

# len

Want to know the length of this list? Use ```len```.

<pre class="file" data-filename="lists.py" data-target="replace">
myNumbers = [10, 5, 7, 2, 1]
print("List length:", len(myNumbers))
</pre>

`python lists.py`{{execute}}

# del

For deleting your mistakes.

<pre class="file" data-filename="lists.py" data-target="replace">
myNumbers = [10, 5, 7, 2, 1]
print("List length:", len(myNumbers))
print(myNumbers)

del myNumbers[1]
print("List length:", len(myNumbers))
print(myNumbers)
</pre>

`python lists.py`{{execute}}

# -1

<pre class="file" data-filename="lists.py" data-target="replace">
myNumbers = [10, 5, 7, 2, 1]
print(myNumbers[-1]) # last number
print(myNumbers[-2]) # second to last
</pre>

`python lists.py`{{execute}}

# append

Add an element to the list.

<pre class="file" data-filename="lists.py" data-target="replace">
fruits = ['apple', 'banana', 'cherry']
print(fruits)
fruits.append("orange")
print(fruits)
</pre>

`python lists.py`{{execute}}

# insert

Insert new value as the second element of the list.

<pre class="file" data-filename="lists.py" data-target="replace">
fruits = ['apple', 'banana', 'cherry']
print(fruits)

fruits.insert(1, "orange")
print(fruits)
</pre>

`python lists.py`{{execute}}

# pop

Remove the second element of the list.

<pre class="file" data-filename="lists.py" data-target="replace">
fruits = ['apple', 'banana', 'cherry']
print(fruits)

fruits.pop(1)
print(fruits)
</pre>

`python lists.py`{{execute}}

# remove

Remove a specific element of the list.

<pre class="file" data-filename="lists.py" data-target="replace">
fruits = ['apple', 'banana', 'cherry']
print(fruits)

fruits.remove("banana")
print(fruits)
</pre>

`python lists.py`{{execute}}

# Tuples

You don't have to worry about tuples for now, but just know that tuples are fixed size in nature whereas lists are dynamic.

* You can't add elements to a tuple. Tuples have no append or extend method.
* You can't remove elements from a tuple. Tuples have no remove or pop method.
* You can find elements in a tuple, since this doesn’t change the tuple.
* You can also use the in operator to check if an element exists in the tuple.

Tuples are faster than lists, and it makes your code safer if you “write-protect” data that does not need to be changed.

# Others
[Read more](https://www.w3schools.com/python/python_ref_list.asp) about the list methods, including ```sort```, ```clear```, ```reverse``` and ```copy```. Also, [read more](https://www.w3schools.com/python/python_strings_slicing.asp) on ```slicing``` and try to use it for lists!