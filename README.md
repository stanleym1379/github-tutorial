# GitHub Tutorial

_by Stanley Mei_

---
## Git vs. GitHub
Git is a version control that takes snapshots of your code. You can refer back to the snapshots you take later. Github is an online cloud server where you can store your snapshots you took with Git. Git is like more of an application rather than a server like Github. Github can also be used a visual to check your changes of your snapshots of code. 




---
## Initial Setup
C9 and Github are linked together. You have to connect your c9 repository, which is your local repository to your Github repository which is a storage server for your files changes or edits. To be able to link together Git and Github, you have to use a SSH Key. First, you have signup for Github. After you signup, you go to the top right corner and click your profile picture. You should see a dropdown of options. You click settings and then you should options on the left hand side. Find SSH and GPG keys. Find the create new SSH key button. The title of the new SSH key is cloud9. To get the key, you have to go to your c9 dashboard. Your c9 dashboard is where all your workspaces are stored. You should see a gear icon on the top right corner where your profile picture is. Click the gear icon. You should see SSH keys on the left column. Copy the second SSH key to your clipboard that is under **"Connect to your private git repository"**. When that is copied, go back to Github settings where you began adding your new SSH key. Paste that key into the box. Then click **"Add SSH key"**. 




---
## Repository Setup
There are steps to setup a repo in your **local repository** and in your server repository in **Github**. Here is the list for the steps. 
Git is an "application" that has commands using the terminal in your local repository. Some commands include ,**"git init"**, **"git status"**, **"git add"**, **"git commit -m"**, and **"git push"**. These command are part of the **"workflow"** for Git_ and Github. A good habit of workflow or git workflow is using git init. Git init is a comamnd that initializes the "application" in the terminal. It's what get's you access to the all commands you use like the one's I stated before. Some important things to note about the command git init is to make sure to never use it if you are in the "~/workspace" folder. If you do git init by accident in the workspace folder, the command to undo the initialization is **"rm -rf .git"**. To prevent this mistake, developing a habit of changing your directory to the one you just cloned or forked.
1. When you have a new repository in your local repository, you have to use the cd command to change to that new repository. The "cd" command is to change your directory.
2. Then you use "git init" in the directory to make a "Git Repository"
3. After you make changes in your file, you git add 



---
## Workflow & Commands
 We have the "git status" command. This command is very useful when you editing or making a new file. Git status helps you differentiate a file if its ready for committing or not. I will explain comitting later. When you use the command git status, the file you are on or using will be red or green. If the file is in a red text, it's not ready for a commit. If the file is in green text, you will be able to commit the file. The "git add" command is what changes the text color when you use the git status command. The "git add" command is usually the first command that you do in "Git Workflow".When you git add, the file will be put in the **"staging area"**. When the file is in the staging area it means that it is ready for a commit and the file will be green when you use "git status." An analogy to the "git add" command is adding people to a picture as the slide said. You Another important part of Git workflow is the command "git commit." You will use the git commit command often with the git add command. When you git commit, you are actually taking the picture or a snapshot of the code. The full git commit command is **"git commit -m"**. After the "-m", you type a message about what you edited or changed in present tense. After you take the "snapshot" of your code, you have to **"git push"**. When you git push, it pushes the changes to the file in the repository you created for file. The explanation for creating a repository will be in Repository setup. 



---
## Rolling Back Changes
Screenshot of slide- Rollback Scavenger hunt 
1. git checkout filename
2. git reset head filename~1
3. git reset --soft HEAD~1
4. git reset --hard HEAD~1
5. git reset head filename