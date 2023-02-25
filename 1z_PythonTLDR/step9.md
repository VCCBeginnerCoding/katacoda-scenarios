# What is a module?

Computer code has a tendency to grow. A larger code always means tougher maintenance, while searching for bugs is always easier where the code is smaller. Multiple programmers working on the same file at the same time isn't ideal either.

As a result, you might want to divide your code into many smaller parts.

The best part? You can incorporate other people's code so you don't have to reinvent the wheel every time!

Create and open new Python file: `modules.py`

<pre class="file" data-filename="modules.py" data-target="replace">
import time

print("this will print immediately")
time.sleep(3)
print("this printed after a 3 second pause")
</pre>

`python modules.py`{{execute}}

As you can see above, we found a built-in module `time`{{}} that allows us to work with time. We Googled the module and found a function `sleep()`{{}} that allows us to suspend code excution temporarily.

<pre class="file" data-filename="modules.py" data-target="replace">
import datetime

x = datetime.datetime.now()
print(x)
</pre>

`python modules.py`{{execute}}

As you can see above, we found a built-in module `datetime`{{}} that allows us to work with dates. We [Googled](https://www.w3schools.com/python/python_datetime.asp) *Python datetime module* to read up on how to use it, and then defined variable `x`{{}} as the time `now`{{}} within the class `datetime`{{}} using the module `datetime`{{}}.

# Renaming modules

Confused? Let's rename the imported module.

<pre class="file" data-filename="modules.py" data-target="replace">
import datetime as myCoolModule

x = myCoolModule.datetime.now()
print(x)
</pre>

`python modules.py`{{execute}}

That's better!

# Making your own modules

Create and open new Python file: `myPersonalModule.py`

<pre class="file" data-filename="myPersonalModule.py" data-target="replace">
def greeting(name):
    print("Hello, " + name)
</pre>

Copy and paste the code above over to your own module `myPersonalModule.py`{{}}.

Now let's reopen the original main Python file: `modules.py`{{open}}

<pre class="file" data-filename="modules.py" data-target="replace">
import myPersonalModule

myPersonalModule.greeting("Jonathan")
</pre>

`python modules.py`{{execute}}

# Others

If you want to dive deeper into modules, check out the `from keyword`{{}} for importing only parts of a module [right here](https://www.w3schools.com/python/python_modules.asp).