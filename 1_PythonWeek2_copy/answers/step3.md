# Module 2 Part 2 Answers:

## **Exercise 1:**
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

## **Exercise 2:**
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


## **Exercise 3:**
Write a program for the following:
* Three friends have been collecting money for charity.
* A local company has offered to double the amount of money they collect if they raise over £1000.
* Write a program that allows the friends to enter their individual amounts.
* The program should then add the three amounts and store the total.
* If the total is greater or equal to 1000, the total should be doubled.
* Finally, the total should be displayed.

```python
money1 = int(input("[Person 1] Enter amount raised: £"))
money2 = int(input("[Person 2] Enter amount raised: £"))
money3 = int(input("[Person 3] Enter amount raised: £"))
total = money1 + money2 + money3if total >= 1000:
    total *= 2
print("£" + str(total))
```

## **Exercise 4:**
6. Write a program that asks the user to enter 3 words. If all 3 are the same (ignoring case) then print "all three are the same", if two words (ignoring case) are the same, print: "two words are the same". Otherwise print, there are no words that are the same.
