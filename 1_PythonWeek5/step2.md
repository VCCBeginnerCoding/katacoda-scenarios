# Dictionaries Part 2

## Nested Dictionaries
Nested dictionaries allow us to store data in a more structured manner.

```python
customers = {
    1: {
        "name": "Sarah",
        "loyalty_rating": 2
    },
    2: {
        "name": "James",
        "loyalty_rating": 3
    },
}
# Output loyalty rating of second customer
print(customers[2]["loyalty_rating"])
```{{exec}}

## Iterating Dictionaries
You can iterate over a dictionary by using a for loop to iterate over the keys in the dictionary and use the value of the key to access the value.
```python
customers = {
    "c1": {
        "name": "Sarah",
        "loyalty_rating": 2
    },
    "c2": {
        "name": "James",
        "loyalty_rating": 3
    },
}

for customer_id in customers.keys():
    customer_data = customers[customer_id]

    print(f"Name: {customer_data['name']} \nLoyalty Rating: {customer_data['loyalty_rating']}")

    # Print empty line to have visual seperation
    print()
```{{exec}}

# Exercises:

## 1
* Create a dictionary called shopping list and add 5 items to the dictionary as the keys. The value of each key should be the quantity.
* Loop through the items in the shopping list and output the item followed by the quantity

## 2.1
Define a dictionary called animals and store 5 animal species as the keys of the dictionary. For each key, the value should be another dictionary with the keys "number_of_legs" and "number_of_eyes". Populate these values for each animal.

## 2.2
* Ask the user for an animal
* If the animal is not present, output the message "I do not know about that animal"
* If the animal is present, output a message stating the animal's specie, it's number of legs and it's number of eyes.

