# GitHub Tutorial

_by Josiah Elbey_

---
## Git vs. GitHub
Git is a tool people in many professions use to keep track of their projects whether it be a script for a play or keeping track of code. Github is similar but it uses
the cloud in order for multiple professionals to work on the same project. Git can work independently from that of Github but Github cant operate without Git.  


---
<h2> Initial Setup</h2>
The initial setup is basically making sure the computer knows where exactly you  `push` your edits to. When you make a Github account you will be `push`ing changes to the repository that bears the same name as the file your working on. A nice thing about it is you can make the computer remember where you put the changes.   
When setting up your repository it's important to form a connection to your local machine.
When ever my mention the idea of a "local machine" it just means the compter your working on but 

## Repository Setup
So to begin a project, go to the icon next to your name and press the + sign and click on new repository. After clicking on the new repository make sure you title it the same name as the file you are working on. 
Then go back to your cd account type the command 

`git init` this turns on git within your file. 
`git remote add origin (your github account link)`
`git push -u origin master` This portion simply makes sure the computer remembers where you want to push your changes.

---
## Workflow & Commands
When ever working on a project the main things you will be doing will be as follows:
* editing your project
* `git add "filename"` will add the file to the stage to be committed
* There are different kinds of adds you can make however
  * `git add.` will add all changed files to your staging area
  * `git add --all` will include all changes made, including deleted files
* `git commit -m message` takes a snapshot of the files on stage and the message should describe what you chnaged in the snapshot (Note:The message should be in past tense to make sure other professionals know what thye do to their file)
* `git push -u origin master` will push your commits onto your repo in git
* `git status` shows which files are set to be committed/ placed on the stage
* `git log` shows a list of all your previous commits which is used to keep track of your work
* `git diff` shows you the difference between your current code and all of your previous commits

In short: 
edit/add/commit/push
---
## Rolling Back Changes
Although it is tricky it is infact possible to undo many commandes that you give to Git like the following: 
* Edits
* `add` commands
* `commit` commands 
* `push` commands 

##### To undo edits to the project 
Type `git checkout -- filename` You dont literary write "filename"! 
This command allows all your changes to your protoflio to be undone. 

##### To undo a `add` command after edits are made
Type `git reset HEAD filename` This keeps your previous edits but rolls back the add command. Basically unstageing the file. 

##### To undo a `commit` command after the file is added to the stage
Lets say you just commited a file to changes and it was a mistake. You can write the command `git reset --soft HEAD-1` this places you back to where you were before you typed the commit command.    

##### To undo a `push` command to go back to after you edited the file
Lets say you edit, add, commit and then push your changes and you realize a mistake  you can write `git reset HEAD-1` to go back to after you wrote edits to the file. 


