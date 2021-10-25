Elements can also be removed from a list at any point in time, we will explore some of the apporaches you can use to remove elements from a list below.

</br>

## **The delete instruction**
The delete instruction **del** is an instruction, not a function, which takes the index of the element being removed in the list and removes that element completely. When this method is used the element will vanish from the list and the lists length will be reduced by one, as shown below:

`
    numbers = [10, 90, 23, 46, -20]
    del numbers[1]
    print(numbers)
    print(len(numbers))`{{execute}}

When you run the code you will see that the number 90 (the element with an index of 1 in the original numbers list) is no longer in the list and that the length of the list has now decreased by one. 

</br>

## **Remove**
The remove method allows you to specify the value you want to remove from the list rather than using the index of the variable. Below is an exmample of us removing a number from the same list using the remove() method:

`
    numbers = [10, 90, 23, 46, -20]
    numbers.remove(90)
    print(numbers)
    print(len(numbers))`{{execute}}

As you can see it removes the element 90 from the list and reduces the length of the list by one. An issue with this method is if there are multiple instances of 90, what will happen? Try and run some code with two 90s in the list and see. 

</br>

## **Pop**
Finally, there is the pop method. This method does not require you to know the index of the element either (though the method does allow you to pass in an element's index if you wish to remove a specific element). By default, this method removes (pops) the last element in the list and reduces the list length by one. However it also returns the removed element so that you can then use that element elsewhere if you wish, without losing it. Below is an example of the pop method being used: 

`
    numbers = [10, 90, 23, 46, -20]
    removed_number = numbers.pop()
    print(numbers)
    print(len(numbers))
    print(removed_number)`{{execute}}

As you can see when running the code, the numbers list is updated and no longer has the -20 element, the length is also down to 4 now. However, the removed number variable contains the -20 variable rather than it just being lost. 

</br>

As you  may have noticed when removing any element from a list, all the other elements that come after that element in the list change position, therefore have different indexes. This is important as it means you could accidentally delete the wrong element if you try and delete elements concurrently (one after the other), or you may end up retrieving the wrong element as its index may have changed. This is something that you should always keep in mind and adjust your code to. The same issue can occur when you add elements to a list via insertion, since all the elements after the inserted element will have a different index. 