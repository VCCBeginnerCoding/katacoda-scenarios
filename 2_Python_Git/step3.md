# Branching

The concept of branching is very important in Git version control. when you create a repository, a default branch called "main" is created. On this branch, you should only have working verisons of your code on the main branch.
Any time you want to work on a new feature or bug fix, you should create a new branch which has a name that reflects what you're working on. This is to prevent any new changes to your code creating new bugs in your main branch.

## Creating a branch via a terminal
Let's create a branch called "git_module" via the command line. To do this, enter the following command in your Git terminal: 

```
git branch git_module
```
In order to make changes on a specific branch, you must "checkout" that specific branch.

```
git checkout git_module
```
Now let's make sure we are on the correct branch:
```
git branch
```
The following command will make sure that all files are tracked in the current branch you are working on:
```
git add -all
```
As we established in the "Commits" section, it is always a good idea to check the status of your repo:
```
git status
```
There shouldn't be any untracked files since we used the ```git add -all``` command.
We are now ready to commit and push changes on this branch as we learned how to do it in the previous "Commits" section.

## Creating a branch via the GitHub website
Creating a branch via the GitHub website is very simple. Just select the branch button then type the branch name, press enter and you're done! Checking out a branch is as simple as clicking on the branch drop-down menu and selecting the branch you want to work on.

For information, take a look at W3Schools' Git exercises: https://www.w3schools.com/git/git_branch.asp?remote=github

## Merging a branch
Once you have completed all of the work you want to on a branch and all tests have been passed (as per the unit testing module of this course), you then need to merge your branch into the main branch. This will copy the changes you made over to the main branch, that way whatever improvements you made are now in the main branch.

When working in a team, you will usually have to make a "pull request" to merge your branch into the main branch. This gives the other people in your team to review your code and make sure it's up to standard before becoming approving the pull request and merging into main. 

When two people are working on serparate branches simultaneously, merge conflicts can sometimes arise. Resolving merge conflicts is a little bit beyond the difficulty level of this course, but it's something to be aware of when you join more complex Git projects.

Creating a pull request and merging a branch into main is very simple in the GitHub website. 

![image](https://user-images.githubusercontent.com/110603725/203048485-756c6978-d6fb-4123-b750-98a824811967.png)
Source: https://docs.github.com/assets/cb-13037/images/help/pull_requests/pullrequest-mergebutton.png

GitHub will check your branch for any merge conflicts and allow you to merge automatically if none are present. 
