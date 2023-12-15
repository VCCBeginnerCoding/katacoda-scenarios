# JSON Files
JSON stands for JavaScript Object Notation and is a useful format for storing and passing complex data structures between programs. You can identify a JSON file easily as they have a ".json" file extension. To use JSON in python we need to import the `json` library.

## Loading Data from JSON
In python, if we wish to load the contents of a json file into our program, we can do so using the `json.load()` function, the contents will be stored in a dictionary.
```python
import json

with open("./file5.json", "r") as file:
    json_data = json.load(file.read())
    print(json_data)
```{{exec}}

## Storing Data into a JSON File
Likewise, we can store the contents of a dictionary into a json file using the `json.dumps()` function.
```python
import json

data = {
    "name": "Sarah",
    "age": 24,
    "favourite_colour": "lime green"
}

with open("./my_json_file.json", "w") as file:
    json_data = json.dumps(data)]
    file.write(json_data)
```{{exec}}
Note! If you would like the json string to be indented you can pass the optional argument `indent=4` to the "json.dumps()" function.

# Exercises
## 1
* Ask the user for their name, favourite colour and favoruite number. Store their answers in a dictionary.
* Store the dictionary as a json file.

## 2
* Using code, extract the favourite colour value from "file5.json".
* Ask the user for their favourite colour.
* If the colour provided by the user matches the favourite colour provided from "file5.json", display the message "Wow! That is my favourite colour too!".
* If the colours do not match display the message "My favourite colour is <colour_from_file5.json>"
