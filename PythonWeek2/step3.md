## **Exercise 1a:**
You've learnt the basics of If and Else statements now, so lets see if you can write one yourself. Write a program that uses If, else and elif statements to tell the user it wants a certain number as input. Below is a list of things the program should do:
- print the sentence "No, I want a bigger number!" on the screen if the inputted number is less than 5
- print the sentence "This number is too big!" on the screen if the inputted number is greater than 10
- print the sentence "This number is just right!" on the screen if the inputted number is 7
- otherwise, print the sentence "This number is close, but still not right!" on the screen


</br>

## **Exercise 1b:**

Below is example code that compares 3 numbers to see which is the smallest:

<pre class="file" data-filename="smallestnum.py" data-target="replace">
    x = 20
    y = 9
    z = 12

    smallest_number = x

    if y < smallest_number:
        smallest_number = y
    
    if z < smallest_number:
        smallest_number = z

    print("The smallest number is: " + str(smallest_number))
</pre>
    
This finds the smallest number of the three by firstly setting the variable smallest_number to x and then comparing that variable with each of the other variables. Run the code to see it work.

To run the code copy it over to your editor and press `smallestnum.py`{{execute}}

Now let's see you write your **own version** to **find the biggest number** between x, y and z. You can set the variables to any numbers you like. 