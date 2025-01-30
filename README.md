# The gp-meta-repo

## The meta tool
To install the meta tool, execute:

**$ npm i -g meta**

Once the meta tool is installed, it is ready for use.

## Cloning the fin-meta-repo and all of its children repositories using SSH.

To setup **GitHub with SSH**, see [Connect to GitHub with SSH using Linux/WSL](https://trimino.com/tools-tips-tricks/connect-to-github-with-ssh-using-linux-wsl/).

**$ meta git clone git@github.com:juan-carlos-trimino/gp-meta-repo.git**

## Using the meta tools
To get meta project updates, first get the .meta file and then get the missing projects:<br>
**$ git pull origin main**

**$ meta git update**

To list all of the files in each project:<br>
**$ meta exec "ls -al"**

To get the status for all repositories:<br>
**$ meta git status**

To pull code changes for all repositories:<br>
**$ meta git pull**

To push code changes for all repositories:<br>
**$ meta git push**

### Branching & Merging
To switch branch:<br>
**$ meta git checkout \<new-branch-name\>**

To create a local branch based on an existing branch other than the current branch and switch to the new branch:<br>
**$ meta git checkout -b \<new-branch-name\> \<existing-branch-name\>**

To create a local branch based on the current branch and switch to the new branch:<br>
**$ meta git checkout -b \<new-branch-name\>**

To push a local branch to a remote repo:<br>
**$ meta git push origin \<local-branch-name\>**

To merge a remote-tracking branch set up locally:<br>
**$ meta git checkout \<branch-name-to-merge-into\>**

**$ meta git merge \<branch-name-to-merge-from\>**

**$ meta git push origin \<branch-name-to-merge-into\>**

To delete a local branch:<br>
**$ meta git branch -d \<local-branch-name\>**

To delete a remote branch:<br>
**$ meta git push origin -d \<remote-branch-name\>**
