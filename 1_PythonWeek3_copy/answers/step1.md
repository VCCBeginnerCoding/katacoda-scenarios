# Module 3 part 1 Answers

## 1.
Create a list of your favourite movies and print it out.
```python
movies = ["WallE", "The Dark Knight", "Forrest Gump", "The Godfather", "The Matrix"]
print("My favorite movies are: ")
print(movies)
```

## 2.
Create a list of your 3 favourite holiday destinations and print it out in this format:
* "My favourite holiday destinations are: item1, item2, item3"
* Hint (you need to use the .join() command which you can research here: [.join()](https://www.programiz.com/python-programming/methods/string/join))
```python
destinations = ["Paris", "Hawaii", "Bali"]
print("My favourite holiday destinations are: " + ", ".join(destinations))
```

We use the join() method to join the items in the destinations list with commas and a space between them. We then concatenate this string with the first part of the message using the + operator.

## 3.
Write a program that creates a list containing 5 fruits:
* Ask the user for an index position
* Print the fruit that corresponds with the index position
* Challenge:
  * Validate the user's input before accessing the list to prevent the index out of bounds error.
```python
fruits = ["apple", "banana", "orange", "kiwi", "mango"]
index = int(input("Enter an index position between 0 and 4: "))
fruit = fruits[index]
print("The fruit at index position", index, "is", fruit)

### Challenge:
fruits = ["apple", "banana", "orange", "kiwi", "mango"]
index = int(input("Enter an index position between 0 and 4: "))

if index >= 0 and index <= 4:
    fruit = fruits[index]
    print("The fruit at index position", index, "is", fruit)
else:
    print("Invalid index position")
```

## 4.
Write a program that creates a list of 5 movies:
* Ask the user how many movies they would like to be recommended.
* Print out the number of movies the user requested
* E.g. If the list was: "one", "two", "three" and the user wanted 2 items, the program should print:
  * "one", "two"
* Challenge:
  * Validate the user's input to prevent an index out of bounds error

```python
movies = ["WallE", "The Dark Knight", "Forrest Gump", "The Godfather", "The Matrix"]
num_recommendations = int(input("How many movies would you like to be recommended? "))
print(movies[0:num_recommendations])

### Challenge:
movies = ["WallE", "The Dark Knight", "Forrest Gump", "The Godfather", "The Matrix"]
num_recommendations = int(input("How many movies would you like to be recommended? "))

if num_recommendations > len(movies):
    print("Sorry, we only have", len(movies), "movies in our list.")
else:
    print("Here are your recommended movies:")
    print(movies[0:num_recommendations])
```