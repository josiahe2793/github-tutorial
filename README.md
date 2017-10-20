# GitHub Tutorial

_by Josiah Elbey_

---
## Git vs. GitHub
Git is a tool people in many professions use to keep track of their  projects. Github is similar but it uses
the cloud in order for multiple professionals to work on the same project. Git can work independently
from that of Github but Github  cant opperate without it. 


---
<h2> Initial Setup</h2>
The initial setup is basically making sure the computer knows what exactly where you  `push` your edits to the repository you intended. A nice thing about it is you can make the computer remember where you put the changes.   

---
## Repository Setup
When setting up your repository it's important to form a connection to your local machine. If you dont do this 
it will be increbibly difficult to work effectively and you wont be able to `push` your work to the cloud. 


---
## Workflow & Commands
When ever working on a project the main things you will be doing will be as follows:
* Edit 
* `add` file to the staging area
* `commit` file to the changes made 
* then finally `push` changes to your online GitHub repository 


---
## Rolling Back Changes
Although it is tricky it is infact possible to undo many commandes that you give to Git like the following: 
* Edits
* `add` commands
* `commit` commands 
* `push` commands 

##### To undo edits to the project 
Type `git checkout -- filename` You dont literary write "filename"! 
This command allows all your chnages to your protoflio to be undon 

##### To undo a `add` command after edits are made
Type `git reset HEAD filename` This keeps your previous edits but rolls back the add command. Basically unstageing the file. 

##### To undo a `commit` command after the file is added to the stage
Lets say you just commited a file to changes and it was a mistake. You can write the command `git reset --soft HEAD-1` this places you back to where you were before you typed the commit command.    

##### To undo a `push` command to go back to after you edited the file
Lets say you edit, add, commit and then push your changes and you relize a mistake  you can write `git reset HEAD-1` to go back to after you wrote edits to the file. 
