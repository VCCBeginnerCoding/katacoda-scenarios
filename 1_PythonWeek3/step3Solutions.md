


<mark>Task:</mark> create a tuple that contains the first names of some friends, and, by calling a function, loop through and print them off

<pre class="file" data-filename="TaskSolution.py" data-target="replace">

# Creating a function called my_function()
def print_tuple(*friends): 
  # The function will then print each name
  for friend in friends:
    print(friend)

# setting up the tuple
friends = ("Aymen", "Emma", "Sandra", "Yasmin")
# calling the function
print_tuple(friends) 
</pre>

`python TaskSolution.py`{{execute}}

<mark>Extra Task 1:</mark> use key-value pairs of first names and last names, and print off the last name of one of your friends using the key

<pre class="file" data-filename="ET1.py" data-target="replace">
def print_last_name(**friends):
  print(Aymen's last name is + " " + friends["Aymen"])
  
friends = (Aymen = "Benylles", Emma = "Eady", Sandra = "Neeliyara", Yasmin = "Cooper")
print_last_name(friends)

</pre>

`python ET1.py`{{execute}}

<mark>Extra Task 2:</mark> repeat the original task, but instead of using a loop try to complete it using a recursive function

<pre class="file" data-filename="ET2.py" data-target="replace">
def recursive_task(friends, count):
  if count == 4:
    return
   else:
    print(friends[count])
    return recursive_task(friends, count+1)

friends = ("Aymen", "Emma", "Sandra", "Yasmin")
recursive_task(friends, 0)

</pre> 

`python ET2.py`{{execute}}
