# Initialize a Git repository
git init

# Add files to the staging area
git add .

# Commit changes with a descriptive message
git commit -m "Initial commit: Project setup"

# Create a new branch
git branch develop
git checkout develop

# Create a feature branch
git checkout -b feature/feedback-entry

# Make changes, add, and commit
git add src/feedback_entry.py
git commit -m "Implement feedback entry feature"

# Push the branch to the remote repository (e.g., GitHub)
git push origin feature/feedback-entry

# (On GitHub) Create a pull request to merge feature/feedback-entry into develop

# After review and merge:
git checkout develop
git pull origin develop
git merge feature/feedback-entry
git push origin develop

# (Less frequent) Merge develop into main
git checkout main
git pull origin main
git merge develop
git push origin main
