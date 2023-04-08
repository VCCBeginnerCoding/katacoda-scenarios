Messy Terminal? `clear`{{execute}} it.
<hr>

<mark>Task:</mark> create a tuple that contains the first names of some friends, and, by calling a function, loop through and print them off

```python
# Creating a function called my_function()
def print_tuple(*friends): 
  # The function will then print each name
  for friend in friends:
    print(friend)

# setting up the tuple
friends = ("Aymen", "Emma", "Sandra", "Yasmin")
# calling the function
print_tuple(friends) 
```

<mark>Extra Task:</mark> use key-value pairs of first names and last names, and print off the last name of one of your friends using the key

```python
def print_last_name(**friends):
  print("Aymen's last name is " +  " "  + friends["Aymen"])
  
print_last_name(Aymen = "Benylles", Emma = "Eady", Sandra = "Neeliyara", Yasmin = "Cooper")
```

<mark>A different method:</mark> repeating the original task, but instead of using a loop, use a recursive function

```python
def recursive_task(friends, count):
  if count == 4:
    return
  else:
    print(friends[count])
    return recursive_task(friends, count+1)

friends = ("Aymen", "Emma", "Sandra", "Yasmin")
recursive_task(friends, 0)

```
