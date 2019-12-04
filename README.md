# GitHub Tutorial

*By: Kelly Tang*

---
## Git vs. GitHub
***Git:***
- version control; keeps *"snapshots"* of the code
-  Doesn't require Github
-  Runs on command line  

***Github:***
- Store code in cloud
- Visually track changes
- Easily collaborate on files
- Requires Git
---
## Initial Setup
1. Go to [github](https://github.com/)
2. Top right corner press _sign up_
3. Log in CS50 with github
4. Follow the following intruction [here](https://github.com/hstatsep/ide50)

- ```SHH```-known as Secure Shell where log in isn't required used to interact with other's repository 
---
## Repository Setup
1. Use ```mkdir``` to make new repo
2. Then ```cd``` into the repo
3. Use ```git init``` and check for the word master
4. Use ```touch <file name>``` to create file and ```c9 <file name>``` to edit the file
5. After editing file, go to [github](https://github.com/)
6. Go to top right corner and click on *New Repository*
7. Find the SSH key then copy and paste it into your repo

---
## Workflow & Commands
***Basic Workflow***

-  Add file by using ```git add .``` or ```git add <file>```
-  Commit the change by using ```git commit -m "commit message"```
- Then push the changes to local repo if needed by using *git push*  
- ```git diff```: see the difference between your current code and the previous commit
- ```git log```: see past commits
- ```git pull```: bring any change from the remote repo "down" to local
- ```git status```: lets you see which changes have been staged
- ```..```: go up to parent directory
- ```~```  : goes to the root directory
- ```(tab)```: auto complete a word
- ```git init```: initializes git in our directory (now called a repository) for version control
- ```git push``` :send any changes from local repo to remote repo
---
## Rolling Back Changes
### *Undo edit*
- ```git checkout --filename``` to undo recent changes from an edit
### *Undo add*
- ```git reset --filename``` to undo anything you added
### *Undo push*
- Use ```git log``` to copy SHA and ```git revert``` then paste SHA. Use ```git reset HEAD^ --hard``` along with ```git push origin master``` to replicate the commit on the local to remote.
### To undo any changes use the following
- If you used *git init* incorrectly, use *rm -rf .git*