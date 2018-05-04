
Ensure you understand the github workflow: https://guides.github.com/introduction/flow/index.html

Please keep pull requests focused on one thing only, since this makes it easier to merge and test in a timely manner.

If you need help with pull requests there are guides on github here:

https://help.github.com/articles/creating-a-pull-request/

The main flow for a contributing is as follows:
## 1. Install Git (newest version)
https://gist.github.com/derhuerst/1b15ff4652a867391f03
## 2. Clone repo from Git to local
### 2.1 Change to working folder
cd [path to your directory]
### 2.2 Clone project from Git to local
Command:  $git-clone [Project URLS]

Example: git -clone https://github.com/coretech1111/IOT_Prototype.git

## 3.  Add modified, new file to stage
Command:  $ git  add . 
## 4. Check status for files
Command:           $git status
## 5. Commit files: 
Command:  $ git commit -a -m  "comment"

Example: $ git commit -a -m  "Sync 31_3: Correct ADC handling to fix ESP issue, add new ECUmanager module"

## 6. Commit to git sever
Command: $ git push [Remote name] [Branch]

See: https://git-scm.com/docs/git-push

Example:
git -push origin master
## 7. Create a new branch with git and manage branches

See: https://github.com/Kunena/Kunena-Forum/wiki/Create-a-new-branch-with-git-and-manage-branches

Create pull request using github UI to merge your changes from your new branch into IOT_Prototype/master
Repeat from step 3 for new other changes.
The primary thing to remember is that separate pull requests should be created for separate branches. Never create a pull request from your master branch.

Once you have created the PR, every new commit/push in your branch will propagate from your fork into the PR in the main github/IOT_Prototype repo. Checkout another branch first if you want something else.

Push will often fail if you edit or squash commits in a branch already pushed. Never do such things after creating the PR.

Later, you can get the changes from the IOT_Prototype repo into your master branch by adding IOT_Prototype as a git remote and merging from it as follows:

git remote add IOT_Prototype https://github.com/coretech1111/IOT_Prototype.git

git checkout master

git fetch IOT_Prototype

git merge IOT_Prototype/master

git push origin master is an optional step that will update your fork on github

You can also perform the git commands using the git client inside Eclipse. Refer to the Eclipse git manual.

Reference: Betaflight project
