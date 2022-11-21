# Introduction to Git Version Control

Version control is a very important aspect of software development. It is a framework which allows software collaborators to simultaneously work on projects and organise their code base properly as they move through developmet.

Version control allows teams to track changes that occur in code as time goes by so that if a new bug is introduced, the version can be rolled back to a working version. All companies with a software team will employ Git version control, and even hobbyist programmers will use it for solo projects.
This makes Git version control an essential skill for any software engineer, so what you learn here will be incredibly useful to you going forward. 

To understand the concept of Git version control, a good place to start is to picture a time where you were submitting a report for school or university. 
We all know the frustrating feeling that comes when we can't remember which file has the most recent draft of the report. As bad as this is for this scenario, imagine how bad this would be if you're working on a software project with hundreds of files that customers depend on for their app to run.

In Git version control, you create a "repository" for each project. This repository holds all of the files for your project. Instead of overiting the files you started with every time you make a change, you essentially upload a new, separate version of the same file. This is called a "commit" in Git version control.
Each commit should be used anytime something significant changes in your code. What people define as significant changes, and we'll go over this later.

During this module, we will cover commits in more detail, as well as branching and pull requests. There are several tools you can use to perform Git version control, with the most popular being GitHub.
We will show you how to perform Git version control from the GitHub website and the terminal as well to give you a broad idea of what's available.

## Creating a repository
Creating a repository is very simple in the GitHub website. You simply open the website, log in to your account and select the "new repository" button:
![image](https://user-images.githubusercontent.com/110603725/203100943-dcfb8fd5-061d-408b-bab3-8a162a5a3991.png)
Source: https://docs.github.com/assets/cb-11427/images/help/repository/repo-create.png

Repositories can either be private, public or internal (https://docs.github.com/en/get-started/quickstart/create-a-repo). Whenever you're doing work for Vodafone, it must never be a private repo - speak to your manager about this before creating a repo. When completing hobby projects in your spare time outside of work, make sure you only make it public if you're happy to share it. If you have a unique idea, releasing it into the public domain may prevent you from making money from it in the future! Also, some online tutorials instruct you to write code which contains sensitive infomration like user credentials for paid services (think cloud services such as AWS). Having your credentials visible online leaves you vunerable to people running up large bills for paid services &mdash; not a situation you want to find yourself in!
