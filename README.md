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
 
1. use **git config --global user.email "you@example.com"**
- *example:* git config --global user.email "kellyt7407hstat.org"
2. use **git config --global user.name "Your Name"
- *exmaple:* git config --global user.name "Kelly Tang"
3. in your root directory use *cd ~*
4. use ssh-keygen -t rsa -b 4096 -C "you@example.com" and press enter repeatly until you see a random image

**you didn't explain that you need a github account first and for the ide setup link the directions that mr.mueller gave us because your directions are confusing**


---
## Repository Setup
1. 


---
## Workflow & Commands
***Basic Workflow***
1. Initial Repository (if there's no existing project)  
   -OR-  
fork/clone, push/pull
2. Edit file  (**talk about creating a README fi)
3. Add file by using ```git add .``` or ```git add <file>```
4. Commit the change by using ```git commit -m "commit message"```
5. Then push the changes to your remotr if needed by using ```git push``` 
- ```git diff```: see the difference between your current code and the previous commit
- ```git log```: see past commits
- ```git pull```: bring any change from the remote repo "down" to local
- ```git status```: lets you see which changes have been staged
- ```..```: go up to parent directory
- ```~``` : goes to the root directory
- **(tab)** : auto complete a word
- ```git init```: initializes git in our directory (now called a repository) for version control

---
## Rolling Back Changes
### to undo any changes use the following
- If you used ```git init``` incorrectly, use```rm -rf .git```
- 