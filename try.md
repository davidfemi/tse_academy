TSE Academy: Github and Version Control

👩‍🏫 Objective
By the end of this lesson, teammates will be able to:
Clone a GitHub repository
Create and switch to a new branch
Make a small contribution to a Markdown file
Stage, commit, and push changes
Open a pull request (PR) on GitHub

🗂️ Materials Needed
A GitHub account
Git installed on your computer <https://coda.io/d/Engineering-Wiki_duvlW1VbQXK/Setting-GitHub-SSH-Key_suExA4-V#_luIxGxjo> 
A code editor like VS Code
Terminal access (Command Prompt, Git Bash, etc.)
This repository: https://github.com/davidfemi/tse_academy

What are Git and Github?
Git is a tool that helps people keep track of changes in files—especially when working on a project with others. Think of it like a detailed history or “undo” button for your code. You can use Git to see what changed, who changed it, and when. It also makes it easy to test new ideas without messing up the main version of your project.

GitHub is a website that lets you store your Git-tracked project online, so you and your team can collaborate from anywhere. It keeps everyone’s work in sync and provides tools to review and discuss changes before they go live.

How do they work together?
Together, Git and GitHub let you:
Make edits confidently, knowing you can always go back
Work in parallel with others without stepping on each other's toes
Share your project with collaborators (or the world)
Review and merge contributions in a structured way
In this tutorial, we'll learn how to use Git and GitHub to make a small contribution to a shared project—just like professional developers do.
Step 1: Clone the Repository
Visit: https://github.com/davidfemi/tse_academy
Click the < > Code button
Copy the HTTPS link
Now, open your terminal and type the two following commands:


cd Desktop
git clone https://github.com/davidfemi/tse_academy.git


Step 2: Navigate Into the Project Folder
List files to confirm the project is there:
ls


 Move into the project folder:
cd TSE_academy_project

Step 3: Create Your Branch
Run this command, replacing the branch name with your own initials and a short description:
git checkout -b 'fo/add_fun_fact'


Step 4: Make Your Change
Open the project folder in your file explorer or VS Code
Open the CONTRIBUTORS.md file
Add fun fact sentence where your name is:
# Our Awesome Contributors
- [Your Name] fun fact

Step 5: Stage and Commit Your Change 

Check what's changed:
git status

Stage the file:
git add .

Commit your change with a message:
git commit -m "Added [Your Name]'s fun fact to the list"

Step 6: Push Your Branch to GitHub

Push your branch up to GitHub:
git push -u origin 'fo/add_fun_fact'
✅ This connects your local branch to GitHub.
Step 7: Open a Pull Request (PR)
Go to the GitHub repo in your browser
Look for the yellow banner and click "Compare & pull request"
 If not visible, click the Pull Requests tab → New pull request
Confirm the title (auto-filled with your commit message)
Leave a message in the description (e.g., "I've added my name to the list.”)
Click Create pull request


Key GitHub Terms
Repository (Repo)
A folder for your project on GitHub. It stores your files, history of changes, and allows others to collaborate.

Remote Repository
The version of your project that lives online (e.g., on GitHub). It’s the source of truth that your team shares and updates.

Clone
Copying a GitHub project from the remote repo to your own computer, so you can work on it locally.

Terminal (or Command Line)
A text-based way to tell your computer what to do—like opening folders, copying files, or running Git commands.

Branch
A separate version of the project where you can make your changes without affecting the main version (usually called main or master).

Checkout
Switching to a different branch, or creating a new one to work on.

Markdown (.md file)
A simple text file that uses symbols (like # or -) to format text. GitHub uses it for documentation.

Stage
Telling Git which files you’re preparing to commit (save). Think of it like selecting items before checking out at a store.

Commit
Saving your changes with a short message describing what you did. Each commit is like a snapshot of your work.

Push
Uploading your commits from your computer to the remote repo on GitHub.

Origin
The name Git uses to refer to the original remote repo you cloned from.

Pull Request (PR)
A way to ask for your changes to be added to the main project. Others can review and approve before merging your work.

Merge
Combining your branch into the main version of the project.

Key Git Commands
git status
A command to check what files you've changed, and whether they’re staged, committed, or need attention.

git add .
Stages all the changed files in the project so you can commit them.

git commit -m "message"
Commits the staged files with a message explaining the change (keep it short and clear).

git push -u origin your-branch-name
Sends your branch and commits to GitHub, making your work visible to others.

