# Week 1 notes

[Kahoot Module 2 Part 1](https://create.kahoot.it/details/f3315997-4ece-445c-a751-f096d3726cf2)
[Kahoot Module 2 Part 2 (Variables)](https://create.kahoot.it/details/eb041ba9-310d-46ea-b57a-2857b3c501ba)

## Intro
- Use this as backup in case Katacoda dies on the day https://replit.com/languages/python3
- Go slow - attendees may be beginners
- "Don't hesistate to ask us for help. Google is your friend" - emphasise that coders Google all the time so it's normal.
- Why we are teaching Python and what you can do with it, add examples of our own work. Show people how flexible Python can be.
    - [Justin's map visualisation](https://colab.research.google.com/drive/1gUeDDBZOztwLgDDhdVjHhRXwhE2MAdEI?usp=sharing)
    - Ellie's Tkinter GUI
    - [Perry's/ Alex's/ Alex's Spotify Timer Flask App](https://github.com/perryliuofficial/MusicTimerForSpotify)
    - [Perry's motion activated light via Raspberry Pi](https://cdn.discordapp.com/attachments/895696933958590506/904125440908734494/VID_20211030_213502.mp4)
- Have a quick summary of the 4 weeks, what we will be covering and what it leads up to.
- If attendees provide an answer, give them the opportunity to explain as well if they want to make it more interactive.
- Add Katacoda sign-on instructions into teams chat during session.

## 1. Variables
- Imagine it's a folder on your computer, where you can create new folders or files. Simply type code into our .py file (like how image files end in .png or .jpg) and then run it via the Terminal.
- Explain print(), the circle brackets, and adding variables in between those brackets.
- Emphasise the practical uses of variables.
- \# Explain code comments.
- For the page with instructions on how to install/run Python outisde Katacoda, let attendees know that it exists.
- Mention that they can use ```clear``` to clear the terminal.
- Encourage participants to edit the code/ variable values.

Quiz Solution:
https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md
```
# Save your age as a variable
age = 22

# Save the current year (2022 as of writing) as a second variable
year = 2022

# Subtract your age from the current year (using the variables) and save that as a third variable
birthYear = currentYear - age

# Print out the third variable
print(birthYear)
```

## 2. Strings & Input
- Remind them they can clear the Terminal with ```clear```
- Emphasise the practical uses

Quiz Solution:
https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md
```
# Ask the user for their favourite colour.
colour = input("What's your favourite colour? Mine is Rich Black #121F2B")

# Print that variable.
print (colour)

# Optional: Chain it by putting input() inside of print() so you only need 1 line of code.
print(input("What's your favourite colour? Mine is Rich Black #121F2B"))

```

## 3. Numbers
- Go slow. This part might be confusing.
- Reassure them by saying that this is not immediately relevant so they can come back later.
- Get them to try ```print(0.1+0.2)``` to see why rounding is needed.
- Emphasise the practical uses part.

Quiz Solution:
https://gitlabce.tools.aws.vodafone.com/vodafonecodingclub/Crash-Course/-/blob/master/Python%20Solutions/Week%201.md
```
# Use input to ask a user for their age.
age = input("What's your age?")

# Subtract 1 from that and print it.
print(age - 1)

# There's a chance that it results in an error.
# So let's convert the input into an integer before subtracting 1 and printing.
print(int(age)-1)
```

## 4. Comparision
- Go slow. This part might be confusing.

## 5. Indentation
- We'll cover if statements in Week 2. Just teach them indentation and show them why comparisions can be very useful.

## 6. Practical Uses
- Talk about Python uses in daily life/ work. Emphasise all the different projects, from games to physical Rapsberry Pi sensors, map visualisation to database management.

## 7. How Katacoda Works
- Try to find time to go through this section with the group. It's essential they they know how to run Python outside of Katacoda, in order for this course to be practical.

## 8. Optional Reading
- Try to find time to go through this section with the group. It's essential they they know how to run Python outside of Katacoda, in order for this course to be practical.