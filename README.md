# AVC CompSci GitHub Tutorial

## Contents

### [Downloading and opening your own copy of the project][section 1]
### [Making changes in your copy of the project and sending them to the master project][section 2]
### [Updating your copy of the project with changes that other people have made][section 3]

## Downloading and opening your own copy of the project

First thing's first, you need to make sure you have a GitHub account. So if you aren't already logged into an account when reading this, go ahead and do that now.

Next, we want to open the "origin" or source of the project in the web browser. If you don't have it open yet, here's a link to it: https://github.com/adjelardin/AVC_Computer_Science_2018-19

Now, you'll see a button there, labelled "Fork". If you click on that, you will create a copy (called a "fork") of the project on your own account. Neat!

![fork][fork]

&nbsp;

Now that the project copy is in your account, you want to download it so you can work on it. To do so, you first want to install GitHub Desktop from https://desktop.github.com/

(Note: if you choose to use Git, the command line version, I assume you are experienced and/or motivated enough to learn that on your own. This tutorial will only use GitHub Desktop)

After installing it, open it from your desktop:

![desktop][desktop]

&nbsp;

Next, you need to "clone" or download the project from your account, using the button or the file drop-down menu. Then select the project in the window that opens, and clone it.

![clone button][clone 1] ![alt clone button][clone 2] ![clone menu][clone 3]

&nbsp;

Now you can open the project in Unity. To do so, launch Unity and at the project selection screen, click on "Open".

![open project][open 1]

&nbsp;

Unless you changed the folder when you were cloning the project, you will need to go to Documents>GitHub (C:/Users/\[your username\]/Documents/GitHub) to find the project folder. Then go into the folder and select the folder "Unity_Project".

![select folder][open 2]

&nbsp;

Then you simply select the project and Unity will launch it. 

Fun fact: When you launch it the first time, it will automatically create some extra files that weren't in the GitHub project. Don't worry, this is normal. Unity creates and uses hundreds of extra files that we don't need to download or keep updated when they're changed, so we tell Git to ignore them. That's what the ".gitignore" file does!

&nbsp;

## Making changes in your copy of the project and sending them to the master project

As you are working on the project, you will want to send your work to the rest of the group. It's a good idea to do so at regular intervals so everyone stays on the same page in the project! But don't worry about pushing every little change you make to the original project right away.

First you of course need to make some changes to the project before you can send us anything. In this tutorial, I've created an empty script called Example.cs inside the Scripts folder.

![example][unity]

&nbsp;

Now that you've made some changes to the project (and *saved* them, that's important), you need to upload them to the project in your account on GitHub.com. However, if you go to GitHub.com and try to upload your files (or the entire project folder), you will run into some problems, such as GitHub telling you that you tried to upload too many files at once. "Yowza!"

So instead, open up GitHub Desktop (and your "repository" or project, if it's not already open). You'll see, immediately, that it automatically noticed all the changes that you made. Kinda creepy... but useful. Here you can review the changes you made, and when you're ready to upload you need to provide a summary (required) and description (optional), and click "Commit".

![commit][commit]

&nbsp;

Now that you are "committed" to the changes you've made, you need to "push" or upload them. All you do is press the "Push" button. Simple enough. (Note: in this case, the "origin" is referring to the project in your account on GitHub.com)

![push][push]

&nbsp;

And finally, you can see the changes you've made in your project on GitHub.com. But recall that you are working with a copy of the project, not the original project. You should see a message saying that you are some number of commits ahead of the origin (here, the "origin" is the original project that yours is "forked" or copied from). To send your changes to all of us, you need to create a "Pull Request" which means you are requesting that we "pull" your changes into the original project.

![pull request][pull]

(Note: if you instead or also see a message that says you are *behind* the origin, you can look at the next section to find out how to keep your project up to date with all the changes *we* make)

&nbsp;

You'll get a chance to make a new summary and description (useful if you've made multiple "commits" before making a pull request) before sending the pull request to the original project.

After that you wait for one of the co-chairs of the team to review the changes you've made and add it to the project. Teamwork!

![waiting for merge][wait]

&nbsp;

## Updating your copy of the project with changes that other people have made

Sometimes, while working on the project in Unity, you will realize that you aren't the only one that is working on it. When this happens, you will want to check GitHub.com to see if anyone has made any changes. And you want to keep up-to-date so you can use the stuff that other people have made (or complain about it) right away! (It may also cause conflicts when you go to pull request and your copy is not up-to-date with the original project, though it should usually be okay depending on what is changed)

So to update your project copy, first go to it on GitHub.com. You'll see a message that says you are some number of commits behind the origin. Instead of making a pull request right away to "pull" the commits from the origin into your project, it's a good idea to click on "compare" first.

![compare][compare]

&nbsp;

At first you'll probably see that there aren't any changes, or you may see the incorrect changes (i.e. the changes that you've already made). This is because it compares *your* project against the *original* project by default, and we need to reverse it. We want to see the comparison of the *original* project against *your* project. Take a look at the drop-down menus that say "base fork" and "head fork", but don't click on them. You'll see the names of the accounts, followed by the name of the project, and you want *your* account to be on the left at the head of the arrow. All you need to do is click on the text for "switching the base".

![switching the base][switch]

&nbsp;

If that text is not there, you need to manually swap the two account names in the drop-down menus. When you try to do so, you will probably end up comparing two branches in your own project or two branches in the original project (the account names will disappear). Don't panic! You can still switch it to looking at the different accounts by clicking on "compare across forks".

![fork comparison][switch 2]

&nbsp;

Now you can finally see the changes! If they aren't important or relevant to you, you can safely ignore them, but it is a good idea to check in often. And if you aren't sure whether it is something you need or not, you're probably better off updating!

So to actually bring the changes into your project, you use a pull request again! Except this time, you're pulling from the original project, instead of the other way around.

![reverse pull request][reverse pull]

&nbsp;

Give the pull request a short name, and a description if you want, to finalize the process and create the request.

![reverse pull request description][reverse pull 2]

&nbsp;

Now you need to merge the pull request. This is what the co-chairs do when you make a pull request to the original project, after reviewing the changes you send.

![merge][merge]

&nbsp;

And your project is now updated on GitHub.com. But before you can go off putting that script that someone wrote onto every game object in the scene in Unity, you need to update your local files. So now we open up GitHub Desktop once again, and we use the handy "Fetch" button. This checks to see if there have been any changes to the project on GitHub.com.

![fetch][fetch]

&nbsp;

After checking for the updates, we want to confirm and actually download those updates. GitHub Desktop knows exactly what we want, so the "Fetch" button automatically changes to the "Pull" button. Click that, and all the changes are finally downloaded to your computer. Phew!

![pull][last pull]

&nbsp;

It may all seem like a long and confusing process now, but let it settle for a bit and you'll be developing games like a pro.

[fork]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/1-Fork.png
[desktop]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/2-Desktop.png
[clone 1]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/3-Clone.png
[clone 2]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/4-AltClone.png
[clone 3]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/5-Clone2.png
[open 1]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/6-OpenProject.png
[open 2]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/7-SelectFolder.png
[unity]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/8-UsingUnity.png
[commit]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/9-Commit.png
[push]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/10-Push.png
[pull]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/11-PullRequest.png
[wait]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/12-WaitForMerge.png
[compare]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/13-Compare.png
[switch]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/14-SwitchBase.png
[switch 2]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/Ad.20-SwitchBase2.png
[reverse pull]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/15-ReversePullRequest.png
[reverse pull 2]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/16-ReversePullRequest2.png
[merge]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/17-Merge.png
[fetch]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/18-Fetch.png
[last pull]: https://raw.githubusercontent.com/adjelardin/AVC_CompSci_GitHub_Tutorial/master/GitHub%20Demo/19-Pull.png

[section 1]: https://github.com/adjelardin/AVC_CompSci_GitHub_Tutorial#downloading-and-opening-your-own-copy-of-the-project
[section 2]: https://github.com/adjelardin/AVC_CompSci_GitHub_Tutorial#making-changes-in-your-copy-of-the-project-and-sending-them-to-the-master-project
[section 3]: https://github.com/adjelardin/AVC_CompSci_GitHub_Tutorial#updating-your-copy-of-the-project-with-changes-that-other-people-have-made
