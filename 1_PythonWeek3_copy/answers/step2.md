# Module 3 Part 2 Answers:

## 1.
Create a list of fruits and print the last item
```python
fruits = ["apple", "banana", "cherry", "date", "elderberry"]
print(fruits[-1])
```

## 2.
Start with an empty list, then ask the user to add three items to their shopping list
* Once the user has added their 3 items print it back to them
* On the next line print the length of the list
```python
shopping_list = []
item1 = input("Please enter the first item for your shopping list: ")
item2 = input("Please enter the second item for your shopping list: ")
item3 = input("Please enter the third item for your shopping list: ")
shopping_list.append(item1)
shopping_list.append(item2)
shopping_list.append(item3)

print("Your shopping list is:", shopping_list)
print("The length of your shopping list is:", len(shopping_list))
```

## 3.
Starting with a list of countries, ask the user if they want to remove the first item or last item of the list
* Carry out the correct operation on the list based on the user's input
* Print the new list
```python
# define a list of countries
countries = ["USA", "Canada", "Mexico", "Brazil", "Argentina", "Chile"]

# ask the user which item to remove
choice = input("Do you want to remove the first or last country in the list? ")

# check if the user chose to remove the first item
if choice.lower() == "first":
    # remove the first item from the list
    removed_item = countries.pop(0)
    print("Removed:", removed_item)

# check if the user chose to remove the last item
elif choice.lower() == "last":
    # remove the last item from the list
    removed_item = countries.pop()
    print("Removed:", removed_item)

# handle invalid input
else:
    print("Invalid choice. Please enter 'first' or 'last'.")

# print the updated list
print("Updated list:", countries)

```

## 4.
Create a list containing 5 shopping list items
* Ask the user which item they would like to remove
* Print the final list once the item is removed
* Challenge - prevent a possible value error if the user enters an item that is not in the list using if statements.
```python
# define the shopping list
shopping_list = ["eggs", "milk", "bread", "cheese", "apples"]

# ask the user which item they want to remove
item_to_remove = input("Which item would you like to remove? ")
shopping_list.remove(item_to_remove)
print(item_to_remove, "has been removed from the list.")

# print the final list
print("Final shopping list:", shopping_list)
```
Challenge:
```python
# define the shopping list
shopping_list = ["eggs", "milk", "bread", "cheese", "apples"]

# ask the user which item they want to remove
item_to_remove = input("Which item would you like to remove? ")

# check if the item is in the list
if item_to_remove in shopping_list:
    # remove the item
    shopping_list.remove(item_to_remove)
    print(item_to_remove, "has been removed from the list.")

# if the item is not in the list
else:
    print("Sorry, that item is not on the list.")

# print the final list
print("Final shopping list:", shopping_list)
```
We use an if statement to check whether the item to remove is in the shopping list using the in keyword.

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

```python
movies = ["WallE", "The Dark Knight", "Forrest Gump", "The Godfather", "The Matrix"]
action = input("Do you want to add or remove a movie? ")

if action == "add":
    title = input("Enter the movie title: ")
    position = int(input("Enter the position to insert the movie: "))
    movies.insert(position-1, title)
elif action == "remove":
    title = input("Enter the movie title to remove: ")
    movies.remove(title)
else:
    print("Invalid action")

print("New length of the list:", len(movies))
print(movies)
```
Challenge:
```python
movies = ["WallE", "The Dark Knight", "Forrest Gump", "The Godfather", "The Matrix"]
action = input("Would you like to add or remove a movie? ")

if action.lower() == 'add':
    new_movie = input("What movie would you like to add? ")
    index = int(input("Where in the list should the movie go? "))
    if index > len(movies):
        movies.append(new_movie)
    else:
        movies.insert(index, new_movie)
elif action.lower() == "remove":
    movie_to_remove = input("What movie would you like to remove? ")
    if movie_to_remove in movies:
        movies.remove(movie_to_remove)
    else:
        print("Invalid movie")
else:
    print("Invalid action")

print("New length of the list:", len(movies))
print(movies)

```

