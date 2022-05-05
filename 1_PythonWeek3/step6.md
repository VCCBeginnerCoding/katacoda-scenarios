


# Further reading!

## Why do we use functions?

Today, virtually all programming languages support user generated functions. But why are they useful?

Well, suppose you are writing some code that changes the background colour of a page everytime you click a button. If you wanted to change to ten different colours, this would mean having to write the same line of code ten times. With a function, we only have to do it once! The benefits of this, other than making your code neat is that if the code needs to be changed, we only need to change it once rather than ten times.

## The do not repeat yourself (DRY) principle!
In computer science, we have a principle called Do Not Repeat Yourself which is aimed at reducing the levels of repetitive code. The DRY principle is stated as "Every piece of knowledge must have a single, unambiguous, authoritative representation within a system". 

Read more about the DRY principle <a href="https://en.wikipedia.org/wiki/Don%27t_repeat_yourself"> here</a>:

## Splitting the task up:
The other benefit of functions is that we can split a task up into multiple functions, and have this called by one function. This means that we don't need to have a massive function with hundreds of lines of code. We could have 4 functions with 25 lines of code for example that gets called by one function.

## Recursion!
Recursion is a mathematical and computing concept that allows us to loop through data without using for or while, and works by having a function return a call to itself. You may see this practice used in other languages, such as Java, since recursion makes the code more efficient. Having said that, this is not the case for Python. The reason we have included this in further reading is to give you an understanding of the code you might see if you move onto other languages, as well as deepening your understanding of loops and functions in Python. 

For example, we can pass in a counter to a recursive function and increment it until it reaches a desired value, then simply return the end amount:

<pre class="file" data-filename="recursiveCall.py" data-target="replace">
# This is a recursive functuon that returns the addition
# of 5 decreasing numbers
def recursive(number, count, answer):
  
  if count == 5:
    return answer
  else:
    # decreasing the value added using number-1
    # increasing the count of numbers used using count+1
    # calculating the addition of the next number using answer+number
    return recursive(number-1, count+1, answer+number)

# For reference, this is what the recursive call would look like in a while loop:

def loop(number, count, answer):

  while count < 5:
    answer += number
    number -= 1
    count += 1
  
  return answer

# We need (start val, number of values already added, total addition) to pass into the functions
# in this case, the last two numbers are 0 as we are at the start of the loop

print("RECURSIVE")
print(recursive(10,0,0))
print ("LOOP")
print(loop(10,0,0))
</pre>

`python recursiveCall.py`{{execute}}

## Additional links

For further information on functions, check <a href="https://realpython.com/defining-your-own-python-function/">this</a> out!

For further information on the while loop, check <a href="https://realpython.com/python-while-loop/">this</a> out!

For further information on the for loop, check <a href="https://realpython.com/python-for-loop/">this</a> out!

For functions and tuples, check <a href="https://edube.org/study/pe1">this</a> out!

For further information on recursion in Python, check <a href="https://analyticsindiamag.com/ultimate-guide-to-recursion-and-iteration-in-python/">this</a> out!
