## The big task - Recursion!

Open new Python file: recursion.py{{open}}

### Instructions:

Lets say, we need to create a countdown function.

We could do this by repeating the code over and over again, like so:

<pre class="file" data-filename="recursion.py" data-target="replace">
def countdown_fun(value):
  print(value)
  value--
    print(value)
  value--
    print(value)
  value--
    print(value)
  value--

  countdown_fun(50)
</pre>

`python recursion.py`{{execute}}

However, this is really inefficient. Your task is to build this same system, but recursivley (where the function calls itself) to countdown from the inputted value to 0.
  
<marquee style='color: blue;'><b>Yay you've completed part 4!</b></marquee>
