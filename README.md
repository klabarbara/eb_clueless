# eb_clueless
Clue-less game project for spring 2021 Foundations of Software Engineering 



## Gitflow isntructions
Once you create a branch for your issue, if you are using git's command line interface, do the following in the directory where you would like your clueless project to live locally: 

`git clone https://github.com/[username]/eb_clueless.git`  (note, you can copy this location directly from the green 'Code' button on our repository's github page) 

This clones our repository into your present working directory. If you use the git clone https option, you will have to user your login credentials every time you want to make a change. You can instead set up an SSH token so github recognizes your machine, that way you can git around with impunity. Requires a few extra steps. (to be filled in later)

`cd eb_clueless` Head into our repo.

`git pull`  

Pull the latest updates from the repo. Since you just cloned, there probably won't be any unless someone (me?) ninja-pushed something. This is also the command to pull future changes to our repository (mainly new branches, updates to current branch you're on)

`git checkout 9001-example-issue-name` 

This checks out your specific feature branch created under your issue. Once your feature branch is checked out, begin to address your issue! As you create files, you'll need to stage them to prepare for committing to your branch. You do this by adding them to the git tracker using `git add newfile(s)`. If you just want to add all new files created within the current directory `git add .` or `git add -all` do the trick. 

If you want to see what has yet to be added/committed, `git status` is a friend. It also will tell you what branch you are currently on, and how far ahead or behind it is from its remote version. I use `git status` compulsively like one would twirl a pen. 

Once you add all your new files to the git tracker, when you are happy with their state to the point that you want to push them up to your remote repository (your feature branch on github.com), it's time to commit! ~~If you want to see the difference between what is currently on the branch and what you are about to commit, try `git diff file(s)` or just `git diff` for everything. Note this is only for things that have not already been committed. ~~ (TODO: Why you no work git diff?)

`git commit file(s)/directory -m "comment describing commit"`

Committing your changes saves them to the local git branch, which is usually (and definitely for the sake of our tutorial) your feature branch you are working on. Once your local branch has the changes committed, it's time to push them up to the remote branch for your feature!

`git push`

Now your remote feature branch has the most up-to-date changes that you have made locally. Congratulations. If you are satisfied that your issue has been addressed, it's time to create a ~~merge~~ pull-request. This will be demonstrated during the tutorial (haha), readme instructions or a link to someone better possibly to follow.