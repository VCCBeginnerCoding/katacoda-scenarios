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

## Making a commit via the GitHub webpage

It is possible to perform simple Git commnds directly on the GitHub webpage (this is what we do when we write these classes for Beginner Coding). This is useful when you want to quickly perform commits and branching without setting it up on Visual Studio Code (VSC) or a terminal. Performing Git commands in VSC on the terminal gives you much more flexibility, allowing you to perform more advanced commands like reverts; this is the preferred option in professional settings. The main advantage of using the GitHub website is that you can see exactly what you are doing as it happens, so it's harder to make mistakes.

A big difference between the two is that on the GitHub webpage, you are working on the remote version of the repository, so you don't need to push commits once you have made them; this step is already complete when you make a commit.

When you go onto your GitHub repository, you can either select a file and edit it directly on the website (shown below), or you can add a file that was saved on your local machine. Editing markdown files is very simple via the GitHub webpage, so if you ever find yourself doing this on a hobby project, you should consider editing directly on the website since it allows you to preview what the markdown will look like and you can work with the repo really quickly.

![image](https://user-images.githubusercontent.com/110603725/203023515-8f613787-44fc-43b8-8b3a-8d6a40640c3b.png)

As oyu can see in the image above, I have a markdown file open and I am editing it in the GitHub website. I can add a commit message and GitHub allows me to create a new branch with this commit (which I don't want to do since I am already working on the desired branch).

For more information, W3Schools is always a good resource for programming: https://www.w3schools.com/git/git_push_to_remote.asp?remote=github

Tip: One of the many great features of GitHub is that you can link commits to specific issues that have been listed for a project. A comment that links to a specific issue could be: "Algorithm structure changed to eliminate bottleneck. Fixes issue <ins>#5</ins>."

