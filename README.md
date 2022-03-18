# Learning-git
My Learnings about `Git`

+ Git clone makes an identical copy of the latest version of a project in a repository and saves it to your computer.
  - git clone <https://name-of-the-repository-link>

You can clone the repository then create a new branch and add your work using your local branch and directory.
Sure, you will user terminal in VSCode to git pull and git push .

+ do not forget to run `git pull origin main` as the first step
+ 
+ *Is git pull the same as `git pull origin master`?*

   - Remember, a pull is a fetch and a merge. git pull origin master fetches commits from the master branch of the origin remote (into the local origin/master branch), and then it merges origin/master into the branch you currently have checked out.
+ By using branches, several developers are able to work in parallel on the same project simultaneously. 
  - `git branch <branch-name>`
+ Creating a new branch:
---
  - 1- Change to main branch using command `git checkout main` . 
  - 2- Make sure the main branch is updated using command `git pull` .
  - 3- Create the branch using `git branch branch-name` .
+ then you need to move to that branch:
`git checkout branch name`
- Add my changes to the staging area. `git add file name`  
- Commit my changes. `git commit -m "adding the header of the main page"`
- push my changes to gitHub. `git push origin header`

- to delete a branch, first you would switch to another branch (like main) and then run `git branch -D branchname`

Creating a new branch is not related to Pull Request.
Pull Request means that you want to merge the changes from your branch into main branch in Github and the reviewer will check your branch then can accept or ask you to edit something.

`Pull request` is a request to merge your changes to the master branch.
It is me telling my collaborators that they can review my changes and merge them to the master branch.

Note: You will never review your changes, you will never merge your changes to the master branch. your collaborators will review your changes and merge them to the master branch.
   
+ Switching to the Master branch
  - To switch between branches simply use the `git checkout` command.
  Run:
    `git checkout master`
+ Commit changes of README file in the master branch.
  Run:
    git checkout master
    git add README
    git commit -m "Added README"
  
  
  This command `git add <file>` means that the files will be added to the stage and this can happen by two ways:
  
+ 1- `git add .` to add all files at once to stage and this is with dot . at the end.
+ 2- `git add file_name` to add file by file ex: git add README.md
    
+ To add your credentials to Git you need to use

git config --global user.name "your gitHub user name"
git config --global user.email "your gitHub email"

+ To learn how to move a file within the repository.
  ---
  Move the hello.html file to the lib directory
*Run:*
  
 `mkdir lib`
  
 `git mv hello.html lib`
  
 `git status`

Result:

$ `mkdir lib`

$ `git mv hello.html lib`

$ `git status`

On branch master
Changes to be committed:
(use "git reset HEAD <file>..." to unstage)
renamed:    hello.html -> lib/hello.html
  
+ To learn how to merge two distinct branches to restore changes to a single branch.
  
+ Merging to a single branch
  
Merging brings changes from two branches into one. Let us go back to the style branch and merge it with master.

Run:

`git checkout style`
  
`git merge master'
  
'git hist --all'

Run:
  
`git commit -m "Moved hello.html to lib"`
  
 + What is 'git stash'?
Image result for git stash
git stash temporarily shelves (or stashes) changes you've made to your working copy so you can work on something else, and then come back and re-apply them later on.
  **merge conflicts** usually happen if a line of code has different versions locally and remotely on GitHub or on different branches..you will run into many of this over the course.. one way to minimise them is to always run a git pull origin main before pushing, so that you are on the latest version of the remote repo.
+  What is origin in git

In Git, "origin" is a shorthand name for the remote repository that a project was originally cloned from. 
  
  
  [REFERENCES](https://github.com/samirm00/workflows/tree/master/workflow-class)
  
  [CREATING CONFLICTS](https://githowto.com/creating_a_conflict)
  
  [INTRODUTION TO GIT](https://www.notion.so/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049)
  
