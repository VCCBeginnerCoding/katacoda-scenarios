# Module 2 part 1.1 Answers
## 1.
Is 100 == "100" true or false?
False

## 2.
Ask the user to enter a number, print true or false if the number is less than 100 but also greater than 50
```python
num = int(input("Enter a number: "))
result = num > 50 and num < 100
print(result)
```

## 3.
Ask the user to enter two numbers, print true or false if the two numbers are equal to each other and both are less than 100
```python
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

result = (num1 == num2) and (num1 < 100 and num2 < 100)

print(result)
```
