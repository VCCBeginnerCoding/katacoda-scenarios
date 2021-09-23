# while
```
while there is something to do
    do it
```

As you can see, ```while``` and ```if``` work similarly.

```
# Store the current largest number here.
largest_number = -999999999

# Input the first value.
number = int(input("Enter a number or type -1 to stop: "))

# If the number is not equal to -1, continue.
while number != -1:
    # Is number larger than largest_number?
    if number > largest_number:
        # Yes, update largest_number.
        largest_number = number
    # Input the next number.
    number = int(input("Enter a number or type -1 to stop: "))

# Print the largest number.
print("The largest number is:", largest_number)
```

If you want the loop to stop running you can press *Control-C*, *Control-Break* or *Command-C* depending on your computer.