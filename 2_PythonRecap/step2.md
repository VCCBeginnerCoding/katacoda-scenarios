# Number Operators, Boolean, Conditions & IF Conditions

## Number Operators
* Addition: +
* Subtraction: -
* Division: /
* Multiplication: *
* Modulus: %
* Integer Division: //
* Power of: **
```python
print("5 + 3 = ", 5 + 3)
print("5 - 3 = ", 5 - 3)
print("5 / 3 = ", 5 / 3)
print("5 * 3 = ", 5 * 3)
print("5 % 3 = ", 5 % 3)
print("5 // 3 = ", 5 // 3)
print("5 ** 3 = ", 5 ** 3)
```{{exec}}

## Boolean Conditions
* Equal: ==
* Not equal: !=
* Less than: <
* Greater than: >
* Less than or equal: <=
* Greater than or equal: >=
* is None
* in list
```python
print("5 == 5 = ", 5 == 5)
print("5 == 3 = ", 5 == 3)
print("5 != 5 = ", 5 != 5)
print("5 != 3 = ", 5 != 3)
print("5 < 3 = ", 5 < 3)
print("5 > 3 = ", 5 > 3)
print("5 <= 3 = ", 5 <= 3)
print("5 >= 3 = ", 5 >= 3)
print("5 is None = ", 5 is None)
print("5 in [1,2,3,4,5] = ", 5 in [1,2,3,4,5])
```{{exec}}

## IF Conditions
* IF Statement
* IF-ELSE Statement
* IF-ELIF Statement
* IF-ELIF-ELSE Statement
```python
name = None
test_score = 4
if name is None:
  name = "Ben"

if name == "Jack":
  print("Hi Jack")
else:
  print("You are not Jack")

if test_score == 5:
  print("You have the highest test score")
elif 2 <= test_score >= 4:
  print("You have a medium test score")
elif test_score == 1:
  print("You have the lowest test score")
else:
  print("Something weird happended you should not have got a number above 5 or lower than 1")
```{{exec}}

# Exercise
* Ask the user for a number.
* Print a message stating if the number is or is not a multiple of 7.