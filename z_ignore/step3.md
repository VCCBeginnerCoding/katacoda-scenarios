# Comparison
```=``` is an assignment operator. ```a = 2``` assigns ```a``` with the value of ```2```.
```==``` instead asks the question *are the values equal*?

`100 == 100`{{execute}}
`100 == 200`{{execute}}

`a = 100
a == 100`{{execute}}

You can also use the ```!=``` not equal to operator.

`100 != 100`{{execute}}
`100 != 200`{{execute}}

Other operators include ```>``` greater than, ```>=``` greater than or equal to, ```<``` less than, and ```<=``` less than or equal to.

`100 > 100`{{execute}}
`100 >= 100`{{execute}}
`100 < 100`{{execute}}
`100 <= 100`{{execute}}

# and

Returns ```True``` if both statements are true.

`x = 5
x < 5 and x < 10`{{execute}}

# or

Returns ```True``` if one of the statements is true.

`x = 4
x < 5 or x < 4`{{execute}}

# not

Reverse the result, returns ```False``` if the result is true.

`x = 999
not(x < 5 and x < 10)`{{execute}}