In the previous step you may have noticed we used the **equal to** operator as part of the conditional checks, you can use all of the other Comparison operators we learnt last week as well to ensure your conditional is only executing when you want it to. 

Below are a few examples of Comparison operators being used in Python to have different bits of code run, can you guess what will be printed?

</br>

### **Example 1:**

<pre class="file" data-filename="ifelif.py" data-target="replace">
    a = "Lisa"
    b = "Sandy"
    c = "lisa"
    d = "Sandy"

    if(a == b):
        print("Lisa is equal to Sandy")
    elif(a == c):
        print("Lisa is equal to lisa")
    elif(b == d):
        print("Sandy is equal to Sandy")
    else:
        print("None of the above are equal")

    if a != b:
        print("Lisa is not equal to Sandy)
</pre>

*Hint: Lower and Upper case matters in string equality*

</br>

**Now try running the code and seeing which print statement is executed.**

Open new Python file: `ifelif.py`{{open}}

Copy the code above over to the editor and then press
`python ifelif.py`{{execute}}

</br>
</br>

### **Example 3:**

<pre class="file" data-filename="greaterthan.py" data-target="replace">
    x = 3
    y = 20

    if x > y:
        print("x is a bigger number than y")
    elif x >= y:
        print("x is the same number as y or bigger")
    elif y < x:
        print("Y is a smaller number than x")
    elif x <= y:
        print("x is the same number as y or smaller than it")
    else:
        print("x is an unknown number")
</pre>

*Hint: Remember how the greater than/less than and equal to operators work in combination and pay attention to which side of the operators x and y are on.*

</br>

**Now try running the code and seeing which print statement is executed.**

Open new Python file: `greaterthan.py`{{open}}

Copy the code above over to the editor and then press
`python greaterthan.py`{{execute}}

</br>
</br>

### **Answers:**

For the first set of code, you should have seen the statement **"Sandy is equal to Sandy"** printed. You may have thought the statement "Lisa is equal to to lisa" would print, but in fact you would be incorrect in that assumption, since the strings have different capatilisation on the 'L' in them, so they are not seen as equal in Python. However the two versions of 'Sandy' both have the same capitalisation and spelling so are treated as equal.

Now for the final set of code, the statement **"x is the same number as y or smaller than it"** should have been printed. This is simply because all the other statements relied on x being larger than y, which it is not, whereas the final statement checked if x was lesser than or equal to y, which  it is, so a condition was finally met. 


