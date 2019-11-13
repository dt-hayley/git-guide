# git-guide

### Cloning
Just making a copy of what's on github to store on your computer.

1. Under the \<code> tab of the repo, there is a green "clone or download" button.
2. Copy the address in the box
3. Open up a terminal or powershell window
4. Navigate to where you want to put the file
  * cd path/to/wherever
  * ex: cd desktop
5. Clone the repo by typing `git clone` + the address you copied from github

### Branches
You can use git to improve on what you currently have by making branches. The master branch is where production code is stored. Any other branch is essentially a copy of the master branch-- this way you can work on writing and testing new code without risking loss of the current working production code. Make a new branch for each task you're working on and make sure they're deleted after they're pulled into master!

1. Using the terminal window, navigate inside the repo.
  * cd git-guide
2. Check the branch you're in using `git branch`
3. Create a new branch using ` git checkout -b name_of_your_new_branch`
4. Add the branch back into github using `git push origin name_of_your_new_branch`
5. Any time you navigate to a new branch, or start work up again, it's worthwhile to run `git pull` to ensure you are working on the most recent version of code.

### Saving changes
To share finished code or just to keep work in progress code safe, you will want to push your code back into github.

1. Using the terminal window, make sure you are in your repo's directory.
2. To add changes to all files use `git add .`
3. To prepare the code to by pushed, use `git commit -m "commit message, can be anything you want"`
4. To finalize your code push, use `git push`

**It's good to note now that all three of these git commands, in this order, are necessary to get your code pushed to github.**

### Pushing back up to master
Once you have written, checked, tested, and pushed your code, you can make a pull request to let others know you are ready for someone else to view your code, and have it pushed into the master branch.

1. On the github website, navigate to the "Pull requests" tab.
2. Click "New pull request"
3. The base is where you want your code to land, usually should be master. Choose which branch you want to pull into master under the "compare:" dropdown.
4. Add title and description of what you changed.
5. Add reviewers.
6. Create pull request. Reviewers can look at code and double check it for any discrepancies or merge conflicts.
**Something cool about github is that as you push updates to the branch, the pull request will automatically update!**
7. Once reviewers approve the pull request, they will merge into master branch and delete the old branches.


