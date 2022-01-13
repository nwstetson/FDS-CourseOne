
# Make a New Repository on GitHub.

Learning Goals:

* Create and use a repository
* Add files to the repository (without coding)
* Make changes to files
* Push changes to your repository file.

Prerequisites:

* Internet access
* An active GitHub Account

## What is a repository?

A [GitHub Repository](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories) contains all the files and folders innvolved in a software projects. In addition, a repository also contains a properly logged history of all changes that have been made to the code in the files. This history is kep secret, using a parsimonious method that keeps the history small but informative. 

The files inside a repository can be text-files, code, images, spreadsheeets as well as datasets. Yet, git is a suboptimal tool to handling large-binary files, such as large datasets, so in geenral large images and datasets are avoided and not stored inside a GitHub repository. 

Repositories can be owned by a single user, or by an [organization](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations) (think about a team of users). 

GitHub repositories can be public or private, that means, only visible to the owner and to any user the owner shares the repository with. 

## Create a repository

#### 1. Navigate to GitHub.com/yourUserID and Sign in to your account.

First, we will use our rpeferred web browser and navigate to GitHub.com. More specifically, we will want to navigate to your GitHub account website. This website is automatically generated by GitHub when you create a user. Your User ID is added after to GitHub.com, so for example my user account on GitHub.com can be found at https://GitHub.com/francopestilli (remember your User ID was defined in [the previous Tutorial](https://github.com/psychdatascience/FDS-CourseOne/blob/main/tutorial002.md)). After navigating to our user account, we will Sign In to GitHub account. That is it! Once logged in your GitHub User Account we will start working with Repositories.

[![This is a Video on How to Login on GitHub!](https://img.youtube.com/vi/KGLG-0VIEDM/0.jpg)](https://www.youtube.com/watch?v=KGLG-0VIEDM)

#### 2. Create a repository: Using the Web User Interface (WebUI).

We will next learn how to use the GitHub.com Web User Interface (WebUI) to create an empty git repository. We will not do much with it at first. Yet, we will select the automated create of a ReadMe file and pick a license (MIT 2.0). [This is a nice article on why it is important to add Licenses to GitHub.com Repositories](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/licensing-a-repository). Also ReadMe files have become critical to GitHub repositories. They provide a "landing page" for your project and there are multiple ways to customize them. You can read more about ReadMe Files [here](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-readmes).

[![This is a video showing you how to Create A New Repository Using the Web User Interface on GitHub!](https://img.youtube.com/vi/2RjRdYPjjD8/0.jpg)](https://www.youtube.com/watch?v=2RjRdYPjjD8)

#### 3. Edit a repository: Add a file to it and then edit the file.

Once a repository is created the next thing we will want to do is to add / remove and edit files. This is indeed why we have created the repository in first place! We will want to use GitHub and get help with content management or code versioning as we develop data analysis skills. Although this might sound confusing at first (we have not yet used the repository), please bare with us for the moment and let's experiment a little bit on how to add and edit the file all via the WebUI.

[![This is a video that shows you how to Create A New File Inside a Repository Using the Web User Interface on GitHub!](https://img.youtube.com/vi/hKj0bay-39A/0.jpg)](https://www.youtube.com/watch?v=hKj0bay-39A)

#### 4. Edit a repository: Edit an existing file.

Now that we have created a repository. Added a ReadMe file, a license and an additional file. Let's practice opening one of the files and editing the content of the files using the Web UI. We will edit the ReadMe.md file, this will give us the opportunity to understand little bit more about MarkDown (or .md files) and have fun with the landing page for the repository. The video below will show you how to edit a ReadMe file using the [MarkDown Syntax](https://guides.github.com/features/mastering-markdown/). MarkDown is a very rich language, but simple at the same time. In our example, we show how to add headings (I called them headers in the video, oh well...) and a list of items.

[![This is a video that shows you how to Edit An Existing File Inside a Repository Using the Web User Interface on GitHub!](https://img.youtube.com/vi/p1HxXwKJrp4/0.jpg)](https://www.youtube.com/watch?v=p1HxXwKJrp4)


Additional readings about repositoroes can be found [here.](https://docs.github.com/en/repositories/creating-and-managing-repositories/about-repositories)

#### 4. Git Commits

##### What is a `commit`? 

As we edited and saved files in the GitHub repository following the tutorial above, you might have noticed that GitHub added information on the files that appeared on top of the repository files. The image below shows where GitHub diplayed information about one change I made to a file in this the repository for this class using the web browser. This is an example of a commit, and GitHub displays information about the commit (ID, User that commited and timestamp) because commits are important.

<img width="1194" alt="GitHubCommits" src="https://user-images.githubusercontent.com/2119795/149251330-5cdd1315-51ba-4345-aff4-bc9806cf0acf.png">

Our goal is to write code. We use Git and GitHub as version control systems to help us track down any potential mistakes and correct them. A commit is the operation of saving the latest code changes to the repository. The commit makes the code part of the most up-to-date version of the repository. More specifically, we use commits to both save the recent code inside the repository of code and to add a record in the log of the history of the repository to remind us (in case neded) that we made a change at a specific time. Commits are kept in the repository history indefinitely. 

Once a recent change to the code is 'committed' to the repository the new changes become officially part of the code repository. Uncommitted code versions are visioble only to you, locally on your machine or in your web broswer. Committed code is visible to everyone that has access to the repository.

We use a commit method to keep track of the changes. At every commit `git` will create a timestamp in the log of the code repository. The commit code will also be saved in the repository and protected so to easily roll back, to the version before the change, in case we were to find that the code introduced by the commit had a bug. See https://en.wikipedia.org/wiki/Commit_(version_control) for further reading.

Commits are not just special to `git` and GitHub. Commits existed before `git` in `SVN` for example. Imagine a lonely developer in an ivory tower. It takes many hours of solitude for the developer to write useful blocks of code. The developer writes for seevral hours going back and forth on the same lines of code. After multiple tests, the developer decides that the code she wrote is OK. It serves the purpose. That is when the developer is ready to `commit`. The words literaly means that the code block that was written is meangfull for the project (or at least the developer things so at the time), so meanigful that it would be important to save a copy of the code into the code base in the repository.

Now, so far we have not really written code. Only created repositores, files and edited them. Yet, if you go back to the previous tutorials you can appreciate that everytime we made a change to the repository. Before the change became live and visible online we had to click a `green button` indicating that we were committing. So we have been committing to the repository all this time without knowing. Or at least, without discussing it. Great.

[Here](https://github.com/git-guides/git-commit) is some additional reading material about `commits`. 

##### How does a commit work in Git (in broad strokes)?

In a nutshell, commits in `git` are snapshots of the entire repository (copies, or almost copies, only the files changed are actually duplicated, but that is for another time). A commit should be thought of as a copy of your entire repository, made at a specific time. The copy will contain the status of the repository at that time. Changes 

You should make new commits often, based around logical units of change. Over time, commits should tell a story of the history of your repository and how it came to be the way that it currently is. Commits include lots of metadata in addition to the contents and message, like the author, timestamp, and more!