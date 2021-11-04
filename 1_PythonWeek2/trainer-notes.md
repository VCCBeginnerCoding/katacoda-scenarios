# Trainer notes for Week 2:
This document is some notes to help you lead Week 2 session as the content intends you to. We have split each step up into its own section for you to navigate through. Some sections will have little to no notes because additional information is not needed on the slides, since it is covered already in the actual course content.

## Step 1 - Conditional Statements
For the first step, just use the course content to explain what if statements are.

When you get to the actual code examples you can go through in a bit more detail how the code is checked on each line to see if the if/elif statement is triggered that time or if it moves onto the next line to check. Explain the results just like the course content does. 

The final note is important to mention since users should know that the else block should always come at the end of the if statements if it is included.

</br>

## Step 2 - If/Else Statements with Operators
Maybe mention which operators where actually learnt in the previous session as a reminder:
- Equals to (==)
- Not equals to (!=)
- Greater than (>)
- Greater than or equals to (>=)
- Less than (<)
- Less than or equals to (<=)
  
For these If/Else statements in this step we do not mention the other operators such as 'not', 'and', 'or' or 'xor' however you could mention how these can also be used in these conditional statements at the end of the session if you wish. 

Again like the previous step, just go through each line of the code for some of the examples and discuss why each line does or does not execute. But this time let them guess what will be printed first and run the code to see the result, before explaining why the result is that value.

</br>

## Step 3 - If/Else Exercises
Maybe break out into break out rooms with one instructor in each room, who can instruct by either:
- Sharing their screen and asking each person what they think the steps are to approaching the problem and what lines of code they should right next. Then after they have completed the problem getting them to write it up themselves
- Having an attendee share their screen and the group help them write the code all together
- Having each attendee write the code individually and ask for help when needed.

Bearing in mind that you will have about 10 minutes for each exercise so this may affect how you approach whichever technique or may make you alter the techniques you want to use (i.e. the first one may need to be altered since it may take up too much time for them all to write it individually as well).

If attendees get stuck on this exercise and there is not enough time to help them, you may want to loop back to them after the session or have them email/message one of the instructors for help after the session. 

</br>

## Step 4 - Lists
In this step we move onto the topic of lists and intialising them. It would be good here to use the course content and maybe your own knowledge to describe why lists are useful and how regularly in coding you actually use them. 

When going over how to initialise lists we compare it to how we intialise variables. It would be good in this instance to compare them directly (maybe in the code editor yourself) and show the difference between intialising a variable and a list clearly to the attendees. 

In this step we are not using code blocks in the code editor, we are using blocks which the attendees can just click and it will go straight into the console and print the result. 

The final note about how lists are numbered (indexed) from zero is very important and should be reinforced/reiterated by instructors. 

</br>

## Step 5 - Indexing Lists and Changing Values
Again in this step we should reinforce that lists start from an index of zero, as this is very important when we are indexing lists. You can show examples of using this to not only show how the indexing works but also to show how it starts from zero. 

We also explain methods in this step somewhat. I would avoid going through a lot of what methods are about, since they are explained in more detail (along with functions) in the next session, just mentioning that things exist called methods that we can call on lists is enough for now. 

For the index method explain how it is finding the location of the string in the list and giving you the number for that and again mention that the first element is at index zero, second at index one, etc. 

Explain for the last part that the value retrieved was the last value in the array, maybe explain how useful this can be in big arrays or in quickly retrieving something.

</br>

## Step 6 - Manipulating Lists
This step is all about the methods which you can use on lists to gain information from them or manipulate them to be displayed differently, such as sorting them. It would be good in this session to explain this and how useful methods for lists are since they are used quite regularly.

For the min-max function you may want to mention that min max can be used in a variety of ways and can be very useful, for example it can be used to find the longest string in an array of strings so you know the max storage you would need per string. 

For the len function, it may be good to mention that it is used regularly to find out the size of very large arrays and used to easily loop through them using range loops.

For the sort function, this generally is very useful and shouldn't need much explanation as to why it is so. However a good example would be sorting a group of names into alphabetical order so it can be displayed effectively to the user.

For the copy function, you should make it clear again that simply using an equals sign i.e. new_array = old_array does not create a new array which is seperate and does not affect the original, it is passing by reference so will change the original array if you change the new one. Therefore using the copy method is essential if you wish to create a copy of an array and edit it without altering the original. 

</br>

## Step 7 - Adding to a list
In this step we discuss the different methods of adding to a list. In this case it may be good to mention which each method is important in their own way. Append is the most used method by most people and is useful as it is quick and easy to complete and you do not need an index of where you want to insert the new variable.

For insert it is useful when you want to insert an element in a specific place, like a sorted list, which we used as an example. It takes more effort since you need to find the index you want to insert it at, but it ensures the array you are inserting into is not negatively impacted or needs reshuffling after you add the new element.

The extend method is similar to append except it adds a whole new array to the end of the current array. Which saves time if you wish to merge two arrays, you don't have to append each new element to the end of the array. 

</br>

## Step 8 - Removing from a List 
Similarly to adding to a list, this step discusses the different methods for removing from a list. In this section it would be good to discuss again why each method is good in it's own way and why one may be used over others in certain scenarios.

For the del method, this is a simple method which requires you have the index of the element you want to delete. Therefore if you already have the index of the element you want to delete, it is a quick and simple method to remove an element from a list.

Then there is the remove method, which does not require you to know the index of the element you wish to remove. Therefore in situations where you want to search for an element in a list and delete it in one method, this is the right method to use. This however does not remove all instances of an element, but it can be combined with a for loop to remove multiple instances.

Finally there is the pop method which by default removes the last element in an array but can be told to remove an element via index. Pop is useful if you want to remove an element but keep the element's value that you removed. 

As mentioned at the bottom of this step, it should be reinforced that if you delete/remove an element from a list, all the elements indexes after that element now have changed, so they should not do consecutive deletions without re-retrieving the index of the next elements. 

</br>

## Step 9 - Nested lists
This step covers nested lists in some detail and has quite a few examples of how nested lists look. In this step try and show with code and reinforce where the square brackets are and reinforce where each of the smaller arrays inside of the big arrays start and end. 

Reinforce how regularly nested lists are used and why they are used i.e. to keep associated data together and manipulate it all at once in a efficient way. 

Showing indexing of these nested lists in a more detailed way than the example, i.e. showing how to just retrieve a singular element in the double nested list would be useful.

However, this is just a brief intro to nested lists, for and while loops are covered in the next session.

</br>

## Step 10 - Lists Exercises
In this final step we just want the attendees to reinforce their learning of nested lists by creating and manipulating some nested lists themselves. You can use the same approaches as you did in the previous exercises and them talk through it as a team, talk through it yourself or have them work individually, whichever you think suits your teaching style best. 

The further work is for those attendees that are either done early or want more work to do after the session to further their learning. In the instance where they ask for help with this or they do not have time to complete the general exercise in the session, you can have them email/message an instructor for help or guidance/confirmation they are doing the right thing. 

</br>
</br>

That's it for Week 2 - Conditial statements and Lists. Hopefully you have found these trainer notes useful and have a better picture of how we intend for this course to be implemented.
