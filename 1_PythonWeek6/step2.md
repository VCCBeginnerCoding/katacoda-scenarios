# Args, Kwargs and Lambda

# Args
It is also possible to pass an infinite number of positional arguments to function using the `*` operator in front of the name of the argument.

```python
def add(*numbers) -> float:
    total = 0
    for number in numbers:
        total += number
    return total

print(add())
print(add(1))
print(add(1, 3))
print(add(1, 3, 6, 8, 10))
```{{exec}}
Notice that the numbers parameter is treated as a tuple.

# Kwargs
 It is also possible to pass an infinite number of keyword arguments to a function using the `**` operator in front of the name of the argument.

 ```python
def display_info(**info) -> None:
    print(info)

display_info(name="james", age=25, fav_colour="green")
 ```{{exec}}
Notice that the info parameter is treated as a dictionary.

## Checking if a Parameter is Defined Within kwargs
You can check if a specific paramter is passed in the same way you would check if a key is present in a dictionary.

```python
def display_info(**info) -> None:
    if "name" in info.keys():
        print(f"Info about {info['name'].title()}:")
    
    print(info)

display_info(name="james", age=25, fav_colour="green")
print() # Print an empty line to create visual seperation
display_info(age=54, fav_colour="blue")
```{{exec}}
