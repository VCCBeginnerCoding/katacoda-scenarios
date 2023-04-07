# Module 2 Part 1.2 Answers:

## **Exercise 1:**
Ask the user to enter a number, if the number is less than 10, print “Your number is too low!”.
```python
num = int(input("Enter a number: "))
if num < 10:
    print("Number is too high!")
```

## **Exercise 2:**
Ask user to enter a password. If the password is “PASSWORD”, print “Login successful”. If not, print “Incorrect password!”
```python
password = input("Enter password: ")
if password == "PASSWORD":
    print("Login successful")
else:
    print("Incorrect password!")
```

## **Exercise 3:**
Ask user to enter a name. If name is “Tom”, print “Welcome Tom!”, if not, print “Sorry <name>, we are expecting Tom.”
```python
user_name = input("Enter name: ")
if user_name.capitalize() == "Tom":
    print("Welcome Tom!")
else:
    print("Sorry " + user_name + " we are expecting Tom.")
```