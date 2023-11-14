# List operations
We are going to cover the most common list operations:
 * Length
 * Append
 * Insert
 * Remove
 * Pop
 * Sort

Messy Terminal? `clear`{{execute}} it.
<hr>

Lists can grow to any length you wish them to be (have as many elements as you want), can be added to at any point and any element can be changed at any point in time, as you saw earlier in this session. Methods for adding elements to a list are important to know as you will be using them regularly. Below we will explore some different methods you can use to do so.
## **Length of a list**
Like with strings we can use the `len()` method to get the number of items in a list:
```python
fruit = ["orange", "apple", "banana"]
print(len(fruit))
```{{exec}}

## **Append**
The append method is the default method most people use when adding an element to a list. It is simple and easy to understand and quite efficient, as it just adds the element to the end of the list and increases the lists length by one, as shown below:

```python
names = ["Ellie", "Dan", "Perry", "Justin"]
names.append("Max")
print(names)
print(len(names))
```{{exec}}

When you run the code you should see that the variable "Max" has now been added to the end of the list and the list length is now 5.


## **Insert**
The insert method allows you to state where in the list you would like the new element to be placed, by providing the method with an index. For this example the names list has already been sorted and we assume that the program knows the name "Max" fits between "Justin" and "Perry" in alphabetical order:

```python
names = ["Dan", "Ellie", "Justin", "Perry"]
names.insert(3, "Max")
print(names)
```{{exec}}

As you can see the insert method is provided two arguments, the index which it has to insert the element before and the element it is inserting.

When you run the code you should be able to see that the element "Max" has been inserted in the list between "Justin" and "Perry" as expected. This method also increases the length of the list just as the previous did, since we are adding another element.

## **Remove**
The remove method allows you to specify the value you want to remove from the list rather than using the index of the variable. Below is an exmample of us removing a number from the same list using the remove() method:

What is the output?
```python
numbers = [10, 90, 23, 46, -20]
numbers.remove(90)
print(numbers)
print(len(numbers))
```{{exec}}

```python
numbers = [10, 90, 23, 90, 46, -20]
numbers.remove(90)
print(numbers)
print(len(numbers))
```{{exec}}

```python
numbers = [10, 90, 23, 46, -20]
numbers.remove(100)
print(numbers)
print(len(numbers))
```{{exec}}

As you can see it removes the element 90 from the list and reduces the length of the list by one. An issue with this method is if there are multiple instances of 90, what will happen? Try and run some code with two 90s in the list and see.


## **Pop**
Finally, there is the pop method. This method does not require you to know the index of the element either (though the method does allow you to pass in an element's index if you wish to remove a specific element). By default, this method removes (pops) the last element in the list and reduces the list length by one. However it also returns the removed element so that you can then use that element elsewhere if you wish, without losing it. Below is an example of the pop method being used:

What is the output?
```python
numbers = [10, 90, 23, 46, -20]
removed_number = numbers.pop()
print(numbers)
print(len(numbers))
print(removed_number)
```{{exec}}

```python
numbers = [10, 90, 23, 46, -20]
removed_number = numbers.pop(-2)
print(numbers)
print(len(numbers))
print(removed_number)
```{{exec}}

As you can see when running the code, the numbers list is updated and no longer has the -20 element, the length is also down to 4 now. However, the removed number variable contains the -20 variable rather than it just being lost.

As you may have noticed when removing any element from a list, all the other elements that come after that element in the list change position, therefore have different indexes. This is important as it means you could accidentally delete the wrong element if you try and delete elements concurrently (one after the other), or you may end up retrieving the wrong element as its index may have changed. This is something that you should always keep in mind and adjust your code to. The same issue can occur when you add elements to a list via insertion, since all the elements after the inserted element will have a different index.

## Sort
The sort method is useful when you have an unordered list that needs to be sorted.

```python
numbers = [10, 90, 23, 46, -20]
print(numbers)
numbers.sort()
print(numbers)
```{{exec}}

The sort function can also work with strings. BEWARE! The sort function will not work if strings and number datatypes are in the same list and will give an error message instead.

```python
names = ["sam", "mark", "lilly", "aiden"]
names.sort()
print(names)
```{{exec}}

Also note that the sort function will prioritise uppercase words over lower case.

```python
names = ["sam", "Mark", "Lilly", "aiden"]
names.sort()
print(names)
```{{exec}}

# Exercises:
## 1.
Create a list of fruits and print the last item

## 2.
Start with an empty list, then ask the user to add three items to their shopping list
* Once the user has added their 3 items print it back to them
* On the next line print the length of the list

## 3.
Starting with a list of countries, ask the user if they want to remove the first item or last item of the list
* Carry out the correct operation on the list based on the user's input
* Print the new list

## 4.
Create a list containing 5 shopping list items
* Ask the user which item they would like to remove
* Print the final list once the item is removed
* Challenge - prevent a possible value error if the user enters an item that is not in the list using if statements.

## Challenge:
### 5.
Create a program that has a list of movies
* Ask the user if they want to add or remove a movie
  * If the user wants to add a movie, also ask where the movie should go in the list.
    * Insert this movie at the correct position in the list
  * If the user wants to remove a move
    * Ask which movie they want to remove
* Print the new length of the list
* Challenge - Prevent any possible errors by making sure the user can't insert the movie into an invalid position and that the user can't remove a movie that doesn't exist

## You have completed part 2

Kahoot time!!!