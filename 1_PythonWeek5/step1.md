
## Intro to Classes

Python is an Objet Oriented Programming langueage (sometimes referred to as OOP). OOPs allow a range of features that are unavailble in other languages (Such as C). One of these features is classes. You can use the 'class' keyword to create a class. Remember that Pyton is case sensitive, so using capital letters are typically associated with class names and lower case is typically associated with variables.

A class is an object constructor, creating a type of object, allowing new instances of the class to be created. You can think of the class as the 'blueprint' and an object as the buildings built using this blueprint. An object can have it's own roperties or methods.

<pre class="file" data-filename="classes.py" data-target="replace">
#let's make the simple class to strat with. This class does nothing
class User:
    pass
</pre>

`python classes.py`{{execute}}

Objects can be used to access different attributes inside a class. For example an attribute of a person class can be 'First Name', 'Surname' or 'Age'. We can access objects using the object name refix. 

<pre class="file" data-filename="objects.py" data-target="replace">
user1 = User()
user1.firstname = 'Aymen'
user2.firstname = 'Daria' 
print(user1.firstname)
print(user2.firstname)
</pre>

`python objects.py`{{execute}}