# Writing, Creating & Deleting

## Overriding or Creating a New File
To tell python to open a file in write mode we need to specify the file mode to be `w`.
If the file already exists, it will be re-written and if the files does not exist it will be created.
To write content to the file we use the `.write()` function which takes 1 argument that is the text to write to the file.
```python
# creating a new file
with open(".new_file.txt", "w") as file:
    file.write("Hello, this is a new file")

# overriding an existing file
with open("./file2.txt", "w") as file:
    file.write("I have rewritten the contents of file2.txt\n")
```{{exec}}

## Appending to an Existing File
To append to an existing file we need to specify the file mode as `a`.
Afterwards, we can use the `.write()` function to add content to the end of the file.
```python
with open("./file2.txt", "a") as file:
    file.write("This is a new line being added to file2.txt")
```{{exec}}

## Creating a New File
If you want to write to file but only if the file does not already exist you can use the create mode; to do this we set the file mode to `x`.
Note! You should always use a try-catch statment when opening a file in create mode.
```python
try:
    with open("./new_file2.txt", "x") as file:
        file.write("This is another new file created using the create mode")
except FileExistError:
    print("Error file already exists, cannot be created again!")
```{{exec}}

If you attempt to open a file in create mode when it already exists, it will give an error message.
```python
try:
    with open("./file2.txt", "x") as file:
        file.write("This is another new file created using the create mode")
except FileExistError:
    print("Error file already exists, cannot be created again!")
```{{exec}}

## Deleting a file
To delete a file we need to import the `os` library, from their we can use the `.remove()` function to remove a file located at a specified path.

# Exercises
## 1.1
Create a file using create mode that has 5 lines and each line has a random word.
## 1.2
After closing the file or exiting the with statment. Using the append mode, ask the user for 3 random words 1 by 1 and append them to the file.
## 1.3
Display the contents of the file line by line.
## 1.4
Ask the user if they want to delete the file, if they say yes, delete the file.

## 2
* Create two files, one to store usernames and the other to store passwords.
* Build a program that allows the user to create an account with a username and password. Make sure thee username does not already exist.
* Allow the user to login using their username and password.