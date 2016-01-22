# GitHub Workflows for ENG 7006
You can find the various ways to work with git, GitHub, GitHub Desktop, Atom, and so on here.

# <a id="top"></a>The overview
To download assignments, work with them, and submit them, you do these major steps:

* [Fork the repo](#fork).
* [Clone the repo](#clone).
* [Create a new branch](#branch).
* [Code](#code)!
* [Submit a pull request](#pull).

### <a id="fork"></a>Fork the repo
This is the easiest step.

* In a browser, get yourself to the repo hosted at the ENG 7006 organization. In general, the URL is https://github.com/eng7006/[repo name].

* On the repo page, click the "Fork" button at the top left.

* This will make a copy of the repo in your GitHub account, and will take you to the repo in your GitHub account.

![GitHub repo](https://github.com/ENG7006/github-workflow/blob/master/github-repo-annotated.png)

[Back to top](#top).

### <a id="clone"></a>Clone the repo
There's an easy way and a hard way.

The easy way is to click on the "Download to GitHub desktop" button, which, helpfully, isn't labelled. I've circled it in the image above. This may or may not work, depending on your local settings. Click it and see what happens. If this doesn't download the repo into GitHub desktop automagically, we'll have to do it the hard way.

The hard way:
* In GitHub Desktop, click the "Add Repo" button. It looks a bit like this: ```+ˇ```. See the GitHub Desktop image with important buttons circled, below.

* This will bring up the "Add repo" dialogue:
![Add repo](https://github.com/ENG7006/github-workflow/blob/master/add-repo.png)

* Select "Clone" and it will bring up the Clone repo dialogue, which will have a list of repos in your GitHub accoun that aren't synced locally. Select the repo you want to work with from that list:
![Clone repo](https://github.com/ENG7006/github-workflow/blob/master/clone.png)

* GitHub Desktop will ask you where to put the repo locally. ```git/[repo-name]``` is not a bad idea, but you can put it wherever you want. Especially since you'll be interfacing with the repo almost entirely through GitHub Desktop, and it will keep track of where the repo is.

* You now have a local working copy of the repo!

![GitHub desktop](https://github.com/ENG7006/github-workflow/blob/master/gh-desktop-annotated.png)

[Back to top](#top).

### Create a new branch
We haven't yet gone over this in class. Logistically, it's quite easy:

* Click on the "New branch" button; it's circled in the GitHub desktop image above.

* This will bring up the "New branch" dialogue:
![Add branch](https://github.com/ENG7006/github-workflow/blob/master/new-branch.png)

* Give the branch a descriptive name, one that will be readable to me. For example, if you were working with ```ball``` and were working on making it bounce horizontally, call your new branch ```horizontal```. Keep it brief, and don't use spaces.

That's it! The new branch will show up in your timeline:
![With branches](https://github.com/ENG7006/github-workflow/blob/master/ghd-with-branches.png)

Conceptually, branches are a bit more difficult. Each branch is an independent line of editing. Whenever you create a branch, it effectively is its own "track changes" history from that point forward. The weird thing is that the switching branches changes the whole folder, not just the file you're working on.

If you're working with multiple branches, and you will, you'll need to **be very careful to be sure you're working on the correct branch**.

Each time you start work on a different daily that uses the same repo, be sure to select the commit in the timeline where you'd like to branch off from. This can be right where you left off, modifying the code you've written, or it can be the repo as you forked it, all the way back at the beginning, or anywhere in between, on any branch. This might take some getting used to.

[Back to top](#top).

### <a id="code"></a>Code!
You can't just write code. You have to open files. Here are the basic steps:

* **Make a change.** Right click on the repo in the list of repos in the leftmost pane in GitHub Desktop, and select "Open in Atom." This will open the folder in Atom, where you left off the last time you were editing it.

* **Save the change.** This is a matter of hitting command-S or control-S (Mac, Windows). Atom lets you know if you have unsaved changes in any files by replacing the x to close the tab with a little blue circle.

* **Test the change.** This means opening the sketch in Google Chrome. To do this: in GitHub Desktop, right click the name of the repo in the leftmost pane with the list of repos. Select "Open in Finder" or "Open in Explorer." This will open the repo folder in your file browser. Double-click on ```index.html```, and this should open the sketch in Google. (It may open in your default browser instead. This is probably fine, but Google is better for debugging. I don't know how to do this in Windows, but on a Mac, if it opens in Safari and you want to open it in Chrome, you can right click on the filename, and select "Open With", and then select Chrome from that menu. In any case, in Chrome, you can always open the file using File > Open.)

* **Test the change: if there are errors.** If things aren't working as you expected, one thing you can do is open the JavaScript Console, to see if JavaScript has spit out any errors. To do this, in Chrome: View > Developer > Javascript Console.

* **Commit the change.** Once the small task at hand is completed, commit the change in GitHub desktop. In GitHub Desktop, you'll see a list of uncommitted changes. Give the commit a brief summary and a slightly less brief description, and then click "Commit."

* **Make another change.** Go back to the "Make a change" step, above.

* Once you're done working for a session, **Sync the change.** Click the "Sync" button at the top right of the timeline. Your changes have now been pushed up to GitHub.

[Back to top](#top).

### <a id="pull"></a>Submit a pull request.
Once your daily is working in a particular, named branch, you can "turn your work in," by submitting a pull request.

* Click the "Pull Request" button at the top right (circled above).

* This brings up the Pull Request pane. It will automatically make the summary of your most recent commit the summary of the pull request. Replace this with a descriptive name (e.g. "ball-horizontal"). Give the pull request a description; this is a little message to me, if you think I need a message.
![Pull request](https://github.com/ENG7006/github-workflow/blob/master/pull-request.png)

* Send the pull request! That sends it to me, and you're done. Time to start work on the next daily exercise! Create a new branch, and start working.
