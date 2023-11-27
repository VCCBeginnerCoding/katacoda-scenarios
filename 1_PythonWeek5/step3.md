# Sets
Sets are similar to lists as they are used to store multiple items in a single variable. However, sets have additional properties.

## Set Properties
* Unindexed
* Unordered
* Values cannot be changed but they can be added or removed
* Cannot hold duplicates

## Defining a Set
Sets are defined similarly to dictionaries however, instead of key:value pairs, they are a list of items.
```python
items = {2, 5, 7, 8, 3, 3, True, "Test"}
print(items)
```{{exec}}
Notice that when more than one of the same item is in the set, only 1 instance of the item is kept in the set. Additionally, the items in the set are randomly shuffled.

## Common Set Functions
* add()
* pop
* clear()
* discard()
* remove()

### Add
The add function will add an item to a set.
```python
a = {1,2,3}
print(a)

a.add(5)
print(a)
```{{exec}}

### Pop
The pop method will remove an item from the set and return the value.
```python
a = {1,2,3}
val = a.pop()
print("Set: ", a)
print("Popped Value: ", val)
```{{exec}}

### Clear
```python
a = {1, 2, 3}
print(a)

a.clear()
print(a)
```{{exec}}

### Discard and Remove
Both the discard and remove function perform the role of removing an item from the set. However, the difference between discard and remove is that remove will throw an error message if the item is not in the set, whereas discard will not.

```python
a = {1,2,3}
a.discard(2)
print(a)

a.remove(3)
print(a)
```{{exec}}

# Exercises:
## 1
* Initialise a set with 3 fruit.
* Output the following instructions to the user
* 1) View Fruit, 2) Add a Fruit, 3) Remove a Fruit, 4) Clear, 5) Exit
* Ask the user for a number that corresponds with the above instructions
* Allow the user to perform the desired operation

## 2
* Define the following list: ["cat", "turtle", "pig", "mouse", "cat", "dog", "pig"]
* Output a list without any duplicates of the existing list, the variable that is outputted must be of a list data type 