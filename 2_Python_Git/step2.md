# Git Commits

## What is a Commmit?

A commit is an action you perform which involves addidng a new version of a file(s). Take the following snippet of code as an example:

<pre class="file" data-filename="commits.py" data-target="replace">
userAge = currentYear - yearOfBirth
print(userAge)
</pre>

I might look at that code and want to add a comment to it so that it's more readable for other developers in my team.

<pre class="file" data-filename="commits.py" data-target="replace">
# Calculate user age
userAge = currentYear - yearOfBirth
print(userAge)
</pre>

This in itself could be  commit. Obviously how you want to commit is up to you and your team; if you want to make plenty of commits that represent lots of changes, this would be a valid approach. Some teams might prefer you to make commits less regularly than this, but this changes on a case-by-case basis.

You should always attach messages to each commit you make so you know what changed. For the example above, it could be: "Comment added to age calculation". 

Tip: One of the many great features of GitHub is that you can link commits to specific issues that have been listed for a project. A comment that links to a specific issue could be: "Alogrithm structure changed to eliminate bottleneck. Fixes issue <ins>#5</ins>.

