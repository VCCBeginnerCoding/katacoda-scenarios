# Comparison
<hr>

`=` is an assignment operator. `a = 2` assigns `a` with the value of `2`.

`==` instead asks the question *are the values equal*?

<pre class="file" data-filename="week1.py" data-target="replace">
print(100 == 100)
print(100 == 200)

a = 100
print(a == 100)
</pre>

You can also use the `!=` not equal to operator.

<pre class="file" data-filename="week1.py" data-target="replace">
print(100 != 100)
print(100 != 200)
</pre>

Other operators include `>` greater than, `>=` greater than or equal to, `<` less than, and `<=` less than or equal to.

<pre class="file" data-filename="week1.py" data-target="replace">
print(100 > 100)
print(100 >= 100)
print(100 < 100)
print(100 <= 100)
</pre>

# and

Returns `True` if both statements are true.

<pre class="file" data-filename="week1.py" data-target="replace">
x = 5
print(x < 5 and x < 10)
</pre>
<div><span style="color:green">print(</span><span style="color:blue">x < 5</span><span style="color:orange"> and </span><span style="color:blue">x < 10</span><span style="color:green">)</span></div>

# or

Returns `True` if one of the statements is true.

<pre class="file" data-filename="week1.py" data-target="replace">
x = 4
print(x < 5 or x < 4)
</pre>
<div><span style="color:green">print(</span><span style="color:blue">x < 5</span><span style="color:orange"> or </span><span style="color:blue">x < 4</span><span style="color:green">)</span></div>

# not

Reverse the result, returns `False` if the result is true.

<pre class="file" data-filename="week1.py" data-target="replace">
x = 999
print(not(x < 5 and x < 10))
</pre>
<div><span style="color:green">print( </span><span style="color:orange">not (</span><span style="color:blue">x < 5</span><span style="color:orange"> and </span><span style="color:blue">x < 10</span><span style="color:orange">)</span><span style="color:green">)</span></div>

<hr>

# Quick Exercise
- You have made it half way lets see how much you have learnt 
- Go back to teams and answer the questions on the screen!

<hr>

# Practical Uses
Is the password that you typed the same as the password that's associated with your account? Comparisions can help. If a project deadline on your database has been missed, we can use comparisions to identify that and then sound the alarm. (Again, there's a few more steps involved in real life, but you get the idea.)
