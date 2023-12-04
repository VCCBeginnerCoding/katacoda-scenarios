# Useful Functions

## Filter
The `filter()` function is useful for filtering lists by specific conditions.

The first parameter of the filter function takes a function that will be used to filter the list. It is common to use a lambda function for these types of scenarios. The second parameter is the list to be filtered.

Note! The filter function returns a filter object, if you wish to keep the items as a list, you must then cast it into a list as shown in the example below.
```python
nums = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15]
multiples_of_3 = list( filter( lambda x: x % 3 == 0, nums ) )
print(multiples_of_3)
```{{exec}}

## Map
The `map()` function will create a new list by apply a function on each item in another list.

Note! Similarly to the filter function, the map function returns a map object and needs to be casted to a list to turn it back into a list.
```python
nums = [1,2,3,4,5,6,7,8,9,10]
nums_squared = list( map( lambda x: x ** 2, nums ) )
print(nums_squared)
```{{exec}}

## Sorted
The `sorted()` function returns a sorted copy of the list provided. Similar to the `.sort()` function, lambda functions can be used to alter the sorting function used.
```python
nums = [5, 7, 29, 95, -6, 4, 7, 11, 9]
nums_largest_to_smallest = sorted( nums, key = lambda x: x * -1 )
print(nums_largest_to_smallest)
```{{exec}}

## Join
The `.join()` function turns a list into a string.
```python
nums = [1, 2, 3, 4, 5]
nums_with_commas = nums.join(",")
nums_with_spaces = nums.join(" ")
nums_with_dashes = nums.join("-")
nums_with_words = nums.join(" and ")
print(nums_with_commas)
print(nums_with_spaces)
print(nums_with_dashes)
print(nums_with_words)
```{{exec}}