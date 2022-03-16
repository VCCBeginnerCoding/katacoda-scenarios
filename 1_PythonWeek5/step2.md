# **Creating Classes**

## Classes and attributes
Attributes are the variables you define for every obeject. In other words, ever object that you create from a class will adopt those variables. The values for the variables are not constant for each object.

Click here to create new Python file: `createClass1.py`{{open}}

**For example:**
<pre class="file" data-filename="createClass1.py" data-target="replace">

# defining code for a class
class className():
  # variables associated for this class
  name = "default"
  number = 0

</pre>

Copy the code above over to the editor and then press
`python createClass1.py`{{execute}}. You can also type that yourself via the Terminal (bottom right) and then press <kbd>ENTER</kbd> to execute it.

<br>

## Classes and methods
Methods are functions you define for every obeject. In other words, ever object that you create from a class will adopt those functions. 

Click here to create new Python file: `createClass2.py`{{open}}

**For example:**
<pre class="file" data-filename="createClass2.py" data-target="replace">

# defining code for a class
class className():
    # method for this class - self represents the object that is calling the method (this will be explored more in the next section)
    def sum(self, int1, int2):
        return int1 + int2

</pre>

<br>

**Please note:** _this code format is more common so majority of example code will use this format. Whenever you're stuck and look for examples online, it will use this alternative format._

<br>

# DIY: Create your own class
Have a go at creating your own class with attributes and methods. If you like, you can use the scenario below for inspiration.

**Scenario:**
Define a class for a car. Think of all of the features a car has for the attributes and any method calculations you could perform, e.g. acceleration.

[Click here for solutions.](https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Week%205)

<br>

## Move on once you are confident with the following:
<ol>
  <li>Creating a class with attributes</li>
  <li>Creating a class with methods</li>
  <li>How a class works and what you could use it for</li>
  <li>You are able to at least attempt the DIY challenge</li>
</ol>
