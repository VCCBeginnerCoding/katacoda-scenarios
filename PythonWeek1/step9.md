# What is a module?

Computer code has a tendency to grow. A larger code always means tougher maintenance, while searching for bugs is always easier where the code is smaller. Multiple programmers working on the same file at the same time isn't ideal either.

As a result, you might want to divide your code into many smaller parts.

The best part? You can incorporate other people's code so you don't have to reinvent the wheel every time!

Open new Python file: `modules.py`{{open}}

<pre class="file" data-filename="modules.py" data-target="replace">
import datetime

x = datetime.datetime.now()
print(x)
</pre>

`python modules.py`{{execute}}