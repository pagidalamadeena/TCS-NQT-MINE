**GIT:-**



🚀 1. Introduction to Git

Git is a distributed version control system (VCS) used to store project files and track changes over time.

✅ Why Git?:-

💾 Works offline

🛡 Reliable version history

🌿 Supports branching and merging

🤝 Helps teams collaborate

🔄 Lets you roll back to previous versions



✅ Important Terms

Repository (Repo): Project storage + history

Commit: Snapshot of your work

Branch: Parallel version of your project

Merge: Combine work from different branches

Remote: Repo stored on a server (GitHub, GitLab, etc.)





💻 2. Working Locally with Git

Local work happens on your machine, without internet.

✅ Common Local Commands



📌 Start a new repository

git init



📌 Check status

git status



📌 Add files to staging

git add <file>

git add .



📌 Commit changes

git commit -m "Commit message"



📌 View commit history

git log



🧩 Local Workflow



✏ Make changes

➕ Add them using git add

✅ Save snapshot using git commit

🔁 Repeat





🌐 3. Working Remotely with Git

Remote repositories are stored on platforms like GitHub, GitLab, Bitbucket, etc.

✅ Common Remote Commands



📌 Clone a repository

git clone <repo-url>



📌 Add a remote origin

git remote add origin <repo-url>



📌 Push commits to remote

git push origin main



📌 Pull latest updates

git pull origin main



📌 Fetch changes without merging

git fetch



🌍 Remote Workflow



Download repo → git clone

Work locally (add → commit)

Upload work → git push

Get updates → git pull





🌿 4. Branching, Merging \& Rebasing

These features allow parallel work without affecting the main project.



✅ Branching

A branch lets you work on new features safely.



📌 Create a branch

git branch feature/login



📌 Switch to branch

git checkout feature/login



📌 Create + switch

git checkout -b feature/login



📌 List branches

git branch





✅ Merging

Used to combine changes from one branch into another.

📌 Merge a branch into main

git checkout main

git merge feature/login



✅ Types of merge:



⚡ Fast-forward merge → Simple, straight-line history

🔀 Three-way merge → Creates a merge commit when branches differ





✅ Rebasing

Rebasing moves your branch on top of updated main branch to create a cleaner, linear history.

📌 Rebase command

git checkout feature/login

git rebase main



&#x20;Merge vs Rebase



Merge                   Vs             Rebase

Keeps full history              Rewrites history

Creates merge commits           Makes linear commits

Best for teamwork               Best for your local cleanup

⚠ Rule:

👉 Do not rebase branches others are using.

