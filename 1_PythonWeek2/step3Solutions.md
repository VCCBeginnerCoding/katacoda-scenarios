# Week 2 Step 3 Conditional Answers:

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

## **Exercise 4:**
Ask user to enter 2 numbers. If the number is the same, print “SNAP”.
```python
num1 = int(input("Enter a number: "))
num2 = int(input("Enter a number: "))
if num1 == num2:
    print("SNAP")

```
* Added challenge – if the first number is higher, print “Your first number is higher than the second number”, else print “Your second number is higher than the first number”
```python
num1 = int(input("Enter a number: "))
num2 = int(input("Enter a number: "))
if num1 == num2:
    print("SNAP")
elif num1 > num2:
    print("Your first number is higher than the second number")
else:
    print("Your second number is higher than the first number")
```

## **Exercise 5:**
Ask user to enter 3 numbers.  Print “SNAP” if all 3 numbers are the same.
```python
nb1 = int(input("Enter a number: "))
nb2 = int(input("Enter a number: "))
nb3 = int(input("Enter a number: "))
if nb1 == nb2 and nb1 == nb3 and nb2 == nb3:
    print("SNAP")
```
* Added challenge – print the smallest number if they are not the same.
```python
nb1 = int(input("Enter a number: "))
nb2 = int(input("Enter a number: "))
nb3 = int(input("Enter a number: "))
if nb1 == nb2 and nb1 == nb3 and nb2 == nb3:
    print("SNAP")
else:
    if nb1 < nb2 and nb1 < nb3:
        print(nb1)
    elif nb2 < nb1 and nb2 < nb3:
        print(nb2)
    else:
        print(nb3)
```


## **Exercise 6:**
Write a program that uses If, else and elif statements to tell the user it wants a certain number as input. Below is a list of things the program should do:
- print the sentence "No, I want a bigger number!" on the screen if the inputted number is less than 5
- print the sentence "This number is too big!" on the screen if the inputted number is greater than 10
- print the sentence "This number is just right!" on the screen if the inputted number is 7
- otherwise, print the sentence "This number is close, but still not right!" on the screen

## **Exercise 7:**
Write a program for the following:
* Three friends have been collecting money for charity.
* A local company has offered to double the amount of money they collect if they raise over £1000.
* Write a program that allows the friends to enter their individual amounts.
* The program should then add the three amounts and store the total.
* If the total is greater or equal to 1000, the total should be doubled.
* Finally the total should be displayed.

```python
money1 = int(input("[Person 1] Enter amount raised: £"))
money2 = int(input("[Person 2] Enter amount raised: £"))
money3 = int(input("[Person 3] Enter amount raised: £"))
total = money1 + money2 + money3if total >= 1000:
    total *= 2
print("£" + str(total))
```