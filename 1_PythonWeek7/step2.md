# Writing to Files

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