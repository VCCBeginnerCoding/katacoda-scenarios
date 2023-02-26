# Week 1 Step 3 Variable Types Answers:

## 1.
* Use input to ask a user for their age.
* Subtract 1 from that and print it.
* There's a chance that it results in an error.
* So let's convert the input into an integer before subtracting 1 and printing.

```python
age = input("What is your age? ")
print("Your new age is: " int(a) - 1)
```

## 2.
Ask user for a number and print out the square.
* Added challenge to print out in a sentence, eg if 5 is entered, print “The square of 5 is 25”
```python
number = float(input("Enter number: "))
square = number*number
print(square)

###Challenge:###
print("The square of", number, "is", square)
```

## 3.
Ask user for the length and height of a rectangle and print out the area.
```python
length = int(input("Enter length: "))
height = int(input("Enter height: "))
print(length * height)
```

## 4.
Ask user for 3 different numbers and print out the sum of the 3 numbers.
* Can you print out the average?
```python
n1 = int(input("Enter a number: "))
n2 = int(input("Enter a number: "))
n3 = int(input("Enter a number: "))
sum = n1 + n2 + n3
print("Sum: ", sum)

###Challenge:###
print("Average: ", sum / 3)
```

## 5.
Ask user for a number and print out the previous and next number.
```python
number = int(input("Enter number: "))
print(number - 1, "and", number + 1)
```