# Dictionaries Part 1
Dictionaries in python are used to store values using key:value pairs.

## Defining a Dictionary
Dictionaries are defined using <b>{}</b> or the <b>dict</b> keyword.
```python
example = {
    "key": "value"
}

cat = {
    "name": "Tom",
    "age": 4,
    "is_chipped": True
}

empty_dict_1 = {}

empty_dict_2 = dict()
```{{exec}}

## Accessing Dictionary Values
You can access specific values inside a dictionary by writing the specific key you are looking for inside of `[]`.

```python
cat = {
    "name": "Tom",
    "age": 4,
    "is_chipped": True
}

print(cat["name"])

# NOTE you need to use different speechmarks for in the inside and outside of a string

print(f"{cat['name']} is {cat['name']} years old!")
```{{exec}}

## Adding and Updating Values
Adding and updating values inside a list is achieved in the exact same way. However, if you define a key that is not already present in the dictionary, it will be added. If the key is already defined then the value is changed.

```python
person = {
    "name": "Ben"
}

# adding a new key:value pair to person
person["age"] = 5

# updating an existing key:value pair in person
person["age"] = 6

print(person)
```{{exec}}

## Removing a Key:Value Pair
You can remove a key:value pair from a dictionary by using the `del` keyword.

```python
person = {
    "name": "Ben"
    "age": 5
}

del person["age"]

print(person)
```{{exec}}

## Viewing Dictioanry Keys and Values On their Own
To view only the keys of a dictionary you can use the `.keys()` method. 
```python
cat = {
    "name": "Tom",
    "age": 4
}

print(cat.keys())
```{{exec}}

Similarly, to view only the values of a dictionary you can use the `.values()`.
```python
cat = {
    "name": "Tom",
    "age": 4
}

print(cat.values())
```{{exec}}

## Checking if a Key Exists
To check if a key exists in a dictionary, you would use the conditional operator `in`.
```python
mouse = {
    "name": "Jerry"
}

print( "name" in mouse.keys() )

print( "age" in mouse.keys() )
```{{exec}}
You can also combine the `in` operator with an if condition.
```python
mouse = {
    "name": "Jerry"
}

if "name" in mouse.keys():
    print(f"Hi {mouse['name']}")

if "age" in mouse.keys():
    print(f"You are {mouse['age']} years old!")
```{{exec}}


# Exercises:
# 1
* Create a dictionary and store your favourite colour, favourite fruit and your name
* Prompt the user to pick a number between 1 and 3 inclusively, denote that the numbers will represent a different option e.g. 1) Name, 2) Favourite Colour, 3) Favourite Fruit
* Prompt the value for the key selected by the user

## 2.1
* Ask the user for their name and favourite colour
* Store their answers in a dictionary
* Output a message to the user telling them their name and favourite colour

## 2.2
* Ask the user if they would like a season pass
* Add the key `has_seasson_pass` and assign it True or False based on the user's response.
* Output the dictionary

