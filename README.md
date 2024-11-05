Git Command Learning.

1. Setting Up Git
Install Git: Download from git-scm.com, and follow the instructions for installation.
Configure Git: Set up your name and email (required for commits).
bash
Copy code
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"

2. Creating a New Repository
Create a Directory: Make a folder for your project and navigate to it.
bash
Copy code
mkdir project-name
cd project-name
Initialize Git: Initialize a new Git repository in your project folder.
bash
Copy code
git init
Add a README (Optional): Create a README file to describe your project.
bash
Copy code
echo "# Project Title" >> README.md
git add README.md
git commit -m "Add README"

3. Making Changes and Committing
Check Status: See what changes are pending for commit.
bash
Copy code
git status
Add Files: Stage files to commit (use . to add all changed files).
bash
Copy code
git add filename   # or
git add .
Commit Changes: Commit your changes with a message.
bash
Copy code
git commit -m "Describe your changes"

4. Connecting to GitHub
Create a Repository on GitHub: Go to GitHub, create a new repository, and copy its URL.
Add Remote Origin: Link your local Git repository to the GitHub repo.
bash
Copy code
git remote add origin <repository-URL>

5. Pushing Code to GitHub
Push Initial Commit: Send your code to GitHub (for the first push, you may need to specify -u origin main).
bash
Copy code
git push -u origin main
For subsequent pushes:
bash
Copy code
git push

6. Pulling Changes from GitHub
Fetch Changes: Retrieve updates from the remote repository.
bash
Copy code
git fetch origin
Pull Changes: Update your local repository with changes from GitHub.
bash
Copy code
git pull origin main

7. Branching Basics
Create a New Branch: Useful for adding features or working on separate tasks.
bash
Copy code
git branch branch-name
Switch to a Branch:
bash
Copy code
git checkout branch-name
Merge a Branch: Merge a branch into the main branch after completing work.
bash
Copy code
git checkout main
git merge branch-name

8. Useful Commands
Check Commit History:
bash
Copy code
git log
View Changes Before Committing:
bash
Copy code
git diff
Undo Last Commit (use carefully):
bash
Copy code
git reset --soft HEAD~1  # Keeps changes
git reset --hard HEAD~1  # Discards changes

9. Cloning an Existing Repository
Clone Repository: Copy a repository from GitHub to your local machine.
bash
Copy code
git clone <repository-URL>

Key Concepts to Remember
Remote: Link to the GitHub repository (usually named origin).
Staging Area: Where files are added before committing.
Commit: Saves your changes locally with a description.
Push/Pull: Send changes to or retrieve updates from GitHub.
This should cover the essential Git commands to start working with GitHub.
