## Create an object
Creating an object is simplier than you think. All this does is make you classes useful - now you'll finally see some results from the terminal!

<br>

## Set values for an object's attributes
Although the structure of the previous code examples help you understand how the code works better, this is not the traditional format for classes. **Note that self refers to the object created.**

<pre class="file" data-target="replace">
Syntax:

  objectName = className(value1, value2, value3...)     # 'values' will set the variables for that object to those values
  
</pre>

The below code is much more professional and widely used. If you can, do classes in the below format. For now, if this is too complicated, then theirs is example code showing how to use the class data in the simpler format previously shown.

<pre class="file" data-filename="objectAttribute.py" data-target="replace">
class Calculator(object):
    total = 0
    
    # the variable values established when creating the object
    def __init__(self, var1, var2):
        # assigning the input values to the class variables
        self.int1 = var1
        self.int2 = var2

# creating an object from the class
example = Calculator(24, 391)

# calling the 'sum' method and printing the results
print("Storage: Value 1 = ", example.int1, ", Value 2 = ", example.int2)
</pre>

`python objectAttribute.py`{{execute}}

<br>

## Call a method using an object
This is very similar to ordinary functions.

<pre class="file" data-target="replace">
Syntax:

  objectName = className(value1, value2, value3...)     # sets values to attributes
  objectName.methodName()                               # executes method
  
</pre>

<pre class="file" data-filename="objectMethod.py" data-target="replace">
class Calculator(object):
    calc = 0
    
    # the variable values established when creating the object
    def __init__(self, var1):
        # assigning the input values to the class variables
        self.name = var1
        
    # method for this class - self represents the object that is calling the method
    def sum(self, int1, int2):
        # increase number of times calculator's used
        self.calc += 1
        # return the sum of input
        return int1 + int2
        
    def numOfTrys(self):
        return self.calc
    
    # method prints a message indicating how many times the calculator was used
    def calcUse(self):
        # if num of times used is more than 1...
        if (self.numOfTrys() > 1):
            print(self.name + " has used this calculator " ,self.numOfTrys(), " times")
        # if num equals 1...
        elif (self.numOfTrys() == 1):
            print(self.name + " has used this calculator once")
        # anything else...
        else:
            print(self.name + " has not used their calculator yet")

# creating an object from the class
example = Calculator("Emma")

# printing the object's variables
print(example.name + "'s Storage: Calculator")

# Calling class class method
print(example.sum(23, 184))
print(example.sum(2, 481))

# More objects
example2 = Calculator("Cameron")
example2.sum(1, 1)
example3 = Calculator("Phillip")

# Calling a method which states how many times the calculator has been used
example.calcUse()
example2.calcUse()
example3.calcUse()
</pre>

`python objectMethod.py`{{execute}}

<br>

## The Above Code Using The Simplier Format
I urge you again to only use this structure if you're really struggling understanding the professional format. Feel free to ask for help :)

### Attribute Code

<pre class="file" data-filename="ex1.py" data-target="replace">
class Calculator(object):
    total = 0
    int1 = 0
    int2 = 0

# creating an object from the class
example = Calculator()
example.int1 = 24
example.int2 = 391

# calling the 'sum' method and printing the results
print("Storage: Value 1 = ", example.int1, ", Value 2 = ", example.int2)
</pre>

`python ex1.py`{{execute}}

<br>

### Method Code

<pre class="file" data-filename="ex2.py" data-target="replace">
class Calculator(object):
    calc = 0
    name = ""

    # method for this class - self represents the object that is calling the method
    def sum(self, int1, int2):
        # increase number of times calculator's used
        self.calc += 1
        # return the sum of input
        return int1 + int2

    def numOfTrys(self):
        return self.calc

    # method prints a message indicating how many times the calculator was used
    def calcUse(self):
        # if num of times used is more than 1...
        if (self.numOfTrys() > 1):
            print(self.name + " has used this calculator " ,self.numOfTrys(), " times")
        # if num equals 1...
        elif (self.numOfTrys() == 1):
            print(self.name + " has used this calculator once")
        # anything else...
        else:
            print(self.name + " has not used their calculator yet")

# creating an object from the class
example = Calculator()
example.name = "Emma"

# printing the object's variables
print(example.name + "'s Storage: Calculator")

# Calling class class method
print(example.sum(23, 184))
print(example.sum(2, 481))

# More objects
example2 = Calculator()
example2.name = "Cameron"
example2.sum(1, 1)

example3 = Calculator()
example3.name = "Phillip"

# Calling a method which states how many times the calculator has been used
example.calcUse()
example2.calcUse()
example3.calcUse()
</pre>

`python ex2.py`{{execute}}

<br>

## DIY: Create a class that has purpose
Have a go at creating more complicated classes. If you like, you can use the scenarios below for inspiration.

<p align="center">
  <img width="500" alt="Screenshot 2022-03-16 154138" src="https://user-images.githubusercontent.com/60058170/158629863-99226230-d2a9-4d8e-8865-007fb7ac96d1.png">
</p>

<pre class="file" data-filename="DIY.py" data-target="replace">
</pre>
`python DIY.py`{{execute}}

**Scenario 1:** Use the class you previously created for a car. What useful attributes/methods could you now add to your class? Attempt to redesign your code to be in the more advanced format. What could be usefule for a car dealership? 

After completing this task, create at least 3 objects from this class with different values. Play around with the methods you have created.

<br>

**Scenario 2:** Mmmmmm. I don't know about you but I love ice cream! I'd love to use an automatic register but I have no way of keeping track of all of my customers and products! I have all the classics you see, and they love them. Some are regulars that I give special 50% discounts too so I'm scared of switching to an automatic system that logs who my customers are and what they are eating as it's important to me that they still recieve my special treatment! Can you help me?

I would like a system that stores a customer's name, number of products bought and total spending. I need to give each customer the option for a receipt. I have many products you'll easily find online. My special treatment customers are Roxanne, Jinx, Jamal and litty Trixy. But I consider any customer who spends more than £30 a week a special treatment customer. Every product costs £2.
