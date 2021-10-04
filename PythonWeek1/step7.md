# A list, but different

Remember to clear your terminal with `clear`{{execute}} if it's too messy!

Tuples are fixed size in nature whereas lists are dynamic.

* You can't add elements to a tuple. Tuples have no append or extend method.
* You can't remove elements from a tuple. Tuples have no remove or pop method.
* You can find elements in a tuple, since this doesn’t change the tuple.
* You can also use the in operator to check if an element exists in the tuple.

Tuples are faster than lists, and it makes your code safer if you “write-protect” data that does not need to be changed. [Read more](https://www.w3schools.com/python/python_tuples.asp).

```
tuple1 = ("apple", "banana", "cherry")
tuple2 = (1, 5, 7, 9, 3)
tuple3 = (True, False, False)
```

# Dictionaries

Dictionaries are used to store data values in key:value pairs.

A dictionary is a collection which is ordered, changeable and does not allow duplicates.

Open new Python file: `dictionaries.py`{{open}}

<pre class="file" data-filename="dictionaries.py" data-target="replace">
thisdict = {
    "brand": "Ford",
    "model": "Mustang",
    "year": 1964
}
print(thisdict)
</pre>

`python dictionaries.py`{{execute}}

<pre class="file" data-filename="dictionaries.py" data-target="replace">
thisdict = {
    "brand": "Ford",
    "model": "Mustang",
    "year": 1964
}
print(thisdict["brand"])
</pre>

`python dictionaries.py`{{execute}}

As you can see below a dictionary can hold any data type.

```
thisdict = {
  "brand": "Ford",
  "electric": False,
  "year": 1964,
  "colors": ["red", "white", "blue"]
}
```