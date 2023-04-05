# Comparison
<hr>

`=` is an assignment operator. `a = 2` assigns `a` with the value of `2`.

`==` instead asks the question *are the values equal*?

```
print(100 == 100)
print(100 == 200)
```{{exec}}

```
a = 100
print(a == 100)
```{{exec}}

You can also use the `!=` not equal to operator.

```
print(100 != 100)
print(100 != 200)
```{{exec}}

Other operators include `>` greater than, `>=` greater than or equal to, `<` less than, and `<=` less than or equal to.

```
print(100 > 100)
```{{exec}}

```
print(100 >= 100)
```{{exec}}

```
print(100 < 100)
```{{exec}}

```
print(100 <= 100)
```{{exec}}

# and

Returns `True` if both statements are true.

```
x = 5
print(x < 5 and x < 10)
```{{exec}}

# or

Returns `True` if one of the statements is true.

```
x = 4
print(x < 5 or x < 4)
```{{exec}}

# not

Reverse the result, returns `False` if the result is true.

```
x = 999
print(not(x < 5 and x < 10))
```{{exec}}

<hr>

<hr>

# Practical Uses
Is the password that you typed the same as the password that's associated with your account? Comparisions can help. If a project deadline on your database has been missed, we can use comparisions to identify that and then sound the alarm. (Again, there's a few more steps involved in real life, but you get the idea.)
