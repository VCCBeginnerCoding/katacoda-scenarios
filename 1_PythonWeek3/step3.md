# Tuples

Tuples are similar to lists, however, once a tuple is defined it cannot be changed. This means that unlike lists, tuples do not have functions such as append and remove.

A tuple can be defined by placing a list of values inside normal brackets.

```python
a = (1,2,3,4,5)
print(type(a))
```{{exec}}

BEWARE! If a tuple only stores a single item, it should have a comma after the item. Without the comma, python will treat the brackets as part of a numerical expression and execute the code inside the brackets first.

```python
# with the comma
a = (1,)
print(type(a))
# without the comma
b = (1)
print(type(b))
```{{exec}}

## Tuple Indexing
Indexing a tuple is exact same as indexing a list.

```python
a = (1,2,3,4,5,6,7)
print(a[0])
print(a[-1])
print(a[1: -2])
```{{exec}}

## Useful Functions

The 'len' function can be used to get the number of items in a tuple.

```python
a = (2,6,4,3,2,5)
print(len(a))
```{{exec}}

The 'sorted' function can be used to sort a tuple. NOTE! Unlike the '.sort' function used by lists, the 'sorted' function does not sort the actual tuple but returns a copy of the tuple that is sorted.
```python
a = (2,6,4,3,2,5)
print(sorted(a))
```{{exec}}

## Exercises:

# 1
Create a tuple and store 5 names in non-alphabetical order. Output the tuple in alphabetical order.

## 1.2
Ask the user for a number between 0 and 4 (inclusively). Output the name at the index specified by the user.