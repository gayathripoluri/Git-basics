To Connect VS Code with GIT Hub:
1)Create a Folder. click on the folder and right click and click on the open terminal and give the command      git init  to initialize git in the folder
2)Open VS code, open the folder eg: DSA-git, and open the terminal automatically the path will be all set 
3)Create a new repository in GitHub copy and paste the link of the repository and back in VS code give this command to connect the VS code with the repository
         		git remote add origin https://github.com/yourusername/yourrepo.git

✅ 1️)Clone an Existing Repository
bash
git clone <repo-url>
Example:
git clone https://github.com/user/repo.git
Copies a repository from GitHub to your local machine.
________________________________________

✅ 2️)Check Repository Status
git status
Shows which files are modified, untracked, or staged.
________________________________________

✅ 3️)Add Files to Staging Area
git add <filename>
Example:
git add syntax.md
To add all files:
git add .
Prepares files for commit.
________________________________________

✅ 4️)Commit Changes
git commit -m "Your commit message"
Example:
git commit -m "Added docs folder and syntax.md"
Saves changes locally.
________________________________________

✅ 5️)Push Changes to GitHub
git push origin <branch-name>
Example:
git push origin main
Sends local commits to GitHub.
________________________________________

✅ 6️)Pull Latest Changes from GitHub
git pull origin <branch-name>
Example:
git pull origin main
Gets the latest updates from the remote repository.
________________________________________

🔹 Branching & Merging
✅ 7️)Create a New Branch
git checkout -b <branch-name>
Example:
git checkout -b feature-login
Creates and switches to a new branch.
________________________________________

✅ 8️) Switch Branches
git checkout <branch-name>
Example:
git checkout main
Switches to another branch.
________________________________________

✅ 9️)Merge a Branch into Main
git checkout main
git merge <branch-name>
Example:
git checkout main
git merge feature-login
Combines changes from another branch.
________________________________________

🔹 Fixing Mistakes
✅ 🔟 Undo Last Commit (Before Pushing)
git reset --soft HEAD~1
Keeps changes but removes the last commit.
________________________________________

✅ 1️1)Discard Local Changes (Before Staging)
git checkout -- <filename>
Example:
git checkout -- syntax.md
Restores the last committed version of the file.
________________________________________

✅ 1️2) Remove Staged Files (Before Commit)
git reset <filename>
Example:
git reset syntax.md
Unstages a file but keeps the changes.
________________________________________

✅ 1️3) Force Push (Use with Caution ⚠️)
git push origin <branch-name> --force
Example:
git push origin main --force
Overwrites history on GitHub (only if necessary).
________________________________________

🔹 Advanced Daily Commands
✅ 1️4)View Commit History
git log --oneline --graph --decorate --all
Shows a compact commit history.
________________________________________

✅ 1️5)Stash Changes Temporarily
git stash
Saves changes temporarily without committing.
To bring changes back:
git stash pop
________________________________________

✅ 1️6)Delete a Branch (After Merging)
git branch -d <branch-name>
Example:
git branch -d feature-login
Deletes a branch locally.
________________________________________

✅ 1️7)Delete a Remote Branch
git push origin --delete <branch-name>
Example:
git push origin --delete feature-login
Deletes a branch from GitHub.
________________________________________

✅ 1️8)Check Remote Repository URL
git remote -v
Shows the URL of your GitHub repository.
________________________________________

✅ 1️9)Change Remote Repository URL
git remote set-url origin <new-repo-url>
Example:
git remote set-url origin https://github.com/user/new-repo.git
Changes the remote GitHub URL.
