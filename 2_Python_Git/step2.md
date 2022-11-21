# Git Commits

## What is a commmit?

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

This in itself could be acommit. Obviously how you want to commit is up to you and your team; if you want to make plenty of commits that represent lots of changes, this would be a valid approach. Some teams might prefer you to make commits less regularly than this, but this changes on a case-by-case basis.

You should always attach messages to each commit you make so you know what changed. For the example above, it could be: "Comment added to age calculation". 

## How to make a commit

When performing Git version control from the command line, the following command would be used to commit these changes to the local copy of your repository:

```
git commit -m "Documentation added to user age calculation"
```

In order to make these changes to the remote copy of your repository (likely hosted in GitHub or Bitbucket), you have to "push" these local changes to the remote repository. Before you do this, it is wise to check the status of your repository:

```
git commit status
```
This command provides information like what branch you are on, how many commits ahead/behind that branch is compared to "main", as well as suggesting you push your changes to the remote version of your repository.

Once we have confirmed that we are on the correct branch, we can push our changes:

```
git push origin
```

For more information, W3Schools is always a good resource for programming: https://www.w3schools.com/git/git_push_to_remote.asp?remote=github

Tip: One of the many great features of GitHub is that you can link commits to specific issues that have been listed for a project. A comment that links to a specific issue could be: "Algorithm structure changed to eliminate bottleneck. Fixes issue <ins>#5</ins>."

