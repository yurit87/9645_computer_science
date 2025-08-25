

1. Install `homebrew` by running the following commands in your terminal.

``` shell
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```


2. Use homebrew to install Git, Github CLI and Obsidian.

``` shell
brew install git
brew install gh
brew install obsidian
```

3. Make an account for GitHub using your school Microsoft email address.
4. Log into GitHub in your browser.
5. Visit https://github.com/Kellett-School/9645_computer_science
6. Click fork - replace `<name>` with your initials.
7. Open your forked version of the repository.
8. Back in your terminal, use `cd` to navigate to the folder where you are storing your Computer Science work this year.
9. Back on the GitHub website, click on the green Code button and choose GitHub CLI copy the `gh repo clone` and paste this into your terminal and run the command.
10. `cd` into the new repository.
11. `cd` into the `Student Notes` subdirectory.
12. Now, open the **Obsidian** app.
13. Choose the option to **Open folder as vault** and choose the repository folder you cloned from GitHub.
14. On the left hand side you will find the **explorer panel**.
15. Inside the `Student Notes` subdirectory, make a new note and call it something like `my_first_note`
16. Go back to your terminal and run the following commands:


``` shell
git config --global user.name yourusername
git config --global user.email youremail@yourdomain.com
```

*Well done*! You have finished the set up of Git, Obsidian & GitHub - this will be the backbone of your workflow for A Level CS.


You will use these commands **throughout** each lesson. This will allow you to push your local changes to the cloud (GitHub) so that a) your teachers can access your work and b) you can sync your work between multiple devices as necessary.

The three commands are `stage`, `commit` and `push`

**`stage`** - register local changes that have been made to files
*alternatively* you can use **`add`** instead of **`stage`** to add files to a commit, both work the same way. You can also use a dot `.` to represent all e.g. `git stage .` means stage all changes for commit.
**`commit`** - save these changes to the git working tree (add a message to describe what you changed)
**`push`** - upload the changes to the server.

``` shell
git stage <name of the file you just created>
git commit -m "made my first note"
git push
```

Another thing that you will be told to do is update your repository by downloading updates from the origin repository - this will allow your teachers to distribute work to you.

To set this up to always merge the changes from the upstream server, run this command:

``` shell
git config pull.rebase true
```

we need to ensure we can still access the course notes in case your teachers update these notes and add new content, this means we need to add the original git repository as a remote called 'upstream' like this:

``` shell
git remote add upstream https://github.com/Kellett-School/9645_computer_science.git
```

Now, whenever you are prompted - run this command to download your teacher's new changes:

``` shell
git pull upstream main 
git pull
git push
```



