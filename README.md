# git-workshop

An introduction to collaborative coding and open source via the wonderful world of version control.

*Version 1.0, for Workshop on June 11th*

##Before the workshop

###Install Git

*Full instructions for installing git can be found [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).*

#####Mac

With Mavericks or above, simply run the command `git` from Terminal.

You can also use an installer, found [here](https://git-scm.com/download/mac).

#####Windows

Use the installer [here](https://git-scm.com/download/win).

#####Linux

Use the appropriate package manager for your flavour of Linux:

`$ sudo yum install git-all`

`$ sudo apt-get install git-all`

###Configure Your Settings

Set your name and email:

`git config --global user.name "Jane Doe"`

`git config --global user.email janedoe@example.com`

###Make a Github Account

If you're viewing this, you're probably already on Github.com. Go ahead and make an account!

##During the workshop

###Basic Git

Create a git repository using `git init`.

Inside your repository, use `git status` to check the current status of the "working tree" (any changes you've made, files you're tracking, etc.) You'll be on a branch called `master`. You should use this command **very often**.

Use `git checkout -b <branch>` to create and switch to a new branch named <branch> (pick your own branch name for this!)

Now, if you `git status`, you can see that you're on the new branch.

Go make some changes to the code in the repository. Add a file, change a line, etc.

Now, try `git status`.

You'll see that you have some unstaged changes! Add them to your staging area using `git add <filename>`.

*You can also use `git add .` or `git add -A` to add all files in the directory, but this should be used with caution.*

`git status` again and you'll see that the changes are now "staged".

Once you're happy with your changes, use `git commit -m "Your message"` to commit them! A commit is a record of changes in the repository. Later on, you'll be able to see your changes at each commit, and roll back to a previous commit if necessary.

###Merging

Now that you have some commits on your branch, you may want to update your `master` branch.
