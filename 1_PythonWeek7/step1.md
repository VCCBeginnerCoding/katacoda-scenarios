# Reading Files

## Opening Files
To open files in python we use the `open()` function.
The open function takes 2 parameters, the first parameter is the path to the file, the second is the mode you want to open the file in.
In this example we are accessing the file with the path `./file1.txt` and the mode is set to `r` which stands for read mode.
```python
file = open("./file1.txt", "r")
file.close()
```{{exec}}
Note! It is important to close the file after using it, otherwise it may leave the file open as a background process which will prevent you from accessing the file again.

## With Statement
The `with` statement is used with special objects known as context managers; these objects perform setup and teardown functions automatically. With the use of the `with` statement, we do not need to close the file as that is handled automatically in the teardown of the context manager object that is returned given to us by the `open()` function.
Note! The `with` statement is the recommended approach for file handling in python.
```python
with open("./file1.txt", "r") as file:
    # do something with the file
    pass
```{{exec}}

## Reading Files as Text
By default when you specify the file mode to be read, python will open the file in text read mode. You can then use the `.read()` function to read the contents of the file.
```python
with open("./file1.txt", "r") as file:
    content = file.read()
    print(content)
```{{exec}}
The read function takes in an optional parameter which specifies the number of bytes to return. The default value is -1 which means it will try to read everything. In the example below, we are getting only the first 5 bytes, this will return the first 5 characters in the file.
```python
with open("./file1.txt", "r") as file:
    first_5 = file.read(5)
    print(first_5)
```{{exec}}

### readline() Function
The `readline()` function will return the contents of the next entire line in the file.
```python
with open("./file2.txt", "r") as file:
    line_1_content = file.readline()
    line_2_content = file.readline()
    print(line_1_content)
    print(line_2_content)
```{{exec}}

### Looping Through a File
You can use a for loop to loop through each line of a file.
```python
with open("./file2.txt", "r") as file:
    for line in file:
        print(line)
```{{exec}}

### readlines() Function
To store the contents of each line of a file in a list you can use the `.readlines()` function.
```python
with open("./file2.txt", "r") as file:
    content = file.readlines()
    print(content)
```{{exec}}

## Reading Files as Binary
To tell python to open the file in binary read mode, we set the mode parameter to `rb`.
```python
with open("file1.txt", "rb") as file:
    content = file.read()
    print(content)
```{{exec}}

# Exercises:
## 1
Display the contents of 'file3.txt' line by line.

## 2
Get the contents of 'file4.txt' and sort the numbers from largest to smallest Then print them out.

