# Basic Git

## Basic Commands

### Initialize a Repository
```bash
git init

Clone a Repository
clone <repository-url>

Check the Status of Your Repository
git status

Add Files to the Staging Area
git add <file-name>         # Add a specific file
git add .                   # Add all changes

Commit Changes
git commit -m "Commit message"

View Commit History
bash
Copy code
git log
git log --oneline           # Simplified view

Branch Management
Create a New Branch
bash
Copy code
git branch <branch-name>

Switch to a Branch
bash
Copy code
git checkout <branch-name>
# OR (modern Git version):
git switch <branch-name>

Create and Switch to a New Branch
bash
Copy code
git checkout -b <branch-name>
# OR:
git switch -c <branch-name>

List All Branches
bash
Copy code
git branch

Merge a Branch into the Current Branch
bash
Copy code
git merge <branch-name>

Delete a Branch
bash
Copy code
git branch -d <branch-name>         # Delete merged branch
git branch -D <branch-name>         # Force delete unmerged branch

Remote Repositories
Add a Remote Repository
bash
Copy code
git remote add origin <repository-url>

View Remote Repositories
bash
Copy code
git remote -v

Push Changes to a Remote Repository
bash
Copy code
git push origin <branch-name>

Pull Changes from a Remote Repository
bash
Copy code
git pull origin <branch-name>

Fetch Changes Without Merging
bash
Copy code
git fetch origin

Stashing
Save Changes Temporarily
bash
Copy code
git stash

List All Stashed Changes
bash
Copy code
git stash list

Apply Stashed Changes
bash
Copy code
git stash apply

Apply and Drop Stashed Changes
bash
Copy code
git stash pop

Clear All Stashed Changes
bash
Copy code
git stash clear

Reverting Changes
Undo Changes in the Working Directory
bash
Copy code
git checkout -- <file-name>

Unstage Files
bash
Copy code
git reset <file-name>

Reset a Commit (soft, mixed, hard)
bash
Copy code
git reset --soft <commit-hash>     # Keep changes staged
git reset --mixed <commit-hash>    # Keep changes in working directory
git reset --hard <commit-hash>     # Discard all changes

Revert a Commit
bash
Copy code
git revert <commit-hash>

Tagging
Create a New Tag
bash
Copy code
git tag <tag-name>

List All Tags
bash
Copy code
git tag

Push Tags to a Remote Repository
bash
Copy code
git push origin <tag-name>
git push origin --tags             # Push all tags

Delete a Tag Locally
bash
Copy code
git tag -d <tag-name>

Delete a Tag from Remote
bash
Copy code
git push origin --delete <tag-name>

Other Useful Commands
Show Changes Between Commits/Files
bash
Copy code
git diff
git diff <branch1> <branch2>

Create an Archive of a Repository
bash
Copy code
git archive --format=zip --output=<file-name>.zip HEAD

Check Configuration
bash
Copy code
git config --list
Set Up Global Username and Email
bash
Copy code
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
