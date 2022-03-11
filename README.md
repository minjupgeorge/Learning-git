# Learning-git
My Learnings about `Git`
+ Git clone makes an identical copy of the latest version of a project in a repository and saves it to your computer.
  - git clone <https://name-of-the-repository-link>
+ do not forget to run `git pull origin main` as the first step
+ *Is git pull the same as `git pull origin master`?*
   - Remember, a pull is a fetch and a merge. git pull origin master fetches commits from the master branch of the origin remote (into the local origin/master branch), and then it merges origin/master into the branch you currently have checked out.
+ By using branches, several developers are able to work in parallel on the same project simultaneously. 
  - `git branch <branch-name>`
+ Creating a new branch:
  - 1- Change to main branch using command `git checkout main` . 
  - 2- Make sure the main branch is updated using command `git pull` .
  - 3- Create the branch using `git branch branch-name` .
+ then you need to move to that branch:
`git checkout branch name`
- Add my changes to the staging area. `git add file name`  
- Commit my changes. `git commit -m "adding the header of the main page"`
- push my changes to gitHub. `git push origin header`

Creating a new branch is not related to Pull Request.
Pull Request means that you want to merge the changes from your branch into main branch in Github and the reviewer will check your branch then can accept or ask you to edit something.

You can clone the repository then create a new branch and add your work using your local branch and directory.
Sure, you will user terminal in VSCode to git pull and git push .
  
  
  
  
  
  
  
  This command git add <file> means that the files will be added to the stage and this can happen by two ways:
  
1- git add . to add all files at once to stage and this is with dot . at the end.
2- git add file_name to add file by file ex: git add README.md
    
    To add your credentials to Git you need to use
  <hr/>
git config --global user.name "your gitHub user name"
git config --global user.email "your gitHub email"
  
  
  ![REFERENCES](https://github.com/samirm00/workflows/tree/master/workflow-class)
  
  
