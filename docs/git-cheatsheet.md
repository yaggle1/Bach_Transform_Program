# Git and GitHub Cheat Sheet

## Daily Workflow

When you start working each day:
```powershell
# Switch to development branch
git checkout development

# Get latest changes from GitHub
git pull

# Check what branch you're on and status
git status
```

When you make changes:
```powershell
# See what files you've changed
git status

# Add your changes
git add .                  # Add all changes
git add filename.py        # Add specific file

# Commit your changes
git commit -m "type: description of changes"

# Push to GitHub
git push
```

## Commit Message Types
When writing commit messages, start with one of these:
- feat: New feature (like a new transformation type)
- fix: Bug fix
- docs: Documentation changes
- style: Code formatting
- refactor: Code restructuring
- test: Adding tests

Example: `git commit -m "feat: Add R4L2 transformation support"`

## Branch Operations

```powershell
# See all branches (* marks current branch)
git branch

# Create and switch to new feature branch
git checkout -b feature/new-feature

# Switch between branches
git checkout development
git checkout master
```

## Common Scenarios

If you forgot to add a file:
```powershell
git add forgotten-file.py
git commit --amend --no-edit
```

If you need to undo changes to a file:
```powershell
git checkout -- filename.py
```

If you need to see your commit history:
```powershell
git log
```

## GitHub Operations

View your repository online:
- Go to https://github.com/yaggle1/Bach_Transform_Program
- Switch branches using the dropdown menu
- Click on files to view their contents
- Click the "Code" button to get the repository URL

## Best Practices

1. Always work in the development branch or a feature branch
2. Pull before starting new work
3. Make regular, small commits with clear messages
4. Push your changes at the end of each session
5. Create a new branch for major new features

## Getting Help

View help for any command:
```powershell
git help command
# Example: git help commit
```

## File Status Lifecycle

1. Untracked: New files Git doesn't know about
2. Modified: Changed files Git knows about
3. Staged: Files ready to commit (after git add)
4. Committed: Files safely stored in Git

## Professional Tips

Remember to:
- Keep commits focused on single changes
- Write clear commit messages
- Push your changes regularly
- Pull before starting new work
- Always work in development branch
- Create new branches for major features

## What Files to Commit

Do commit:
- Python source files (.py)
- Documentation files (.md)
- MusicXML files
- Configuration files

Don't commit (they're in .gitignore):
- __pycache__ folders
- Virtual environment files
- IDE settings
- Temporary files

## When You're Done Working

No special logout needed! Just:
1. Commit your changes
2. Push to GitHub
3. Close your editor and terminal

Everything will be safe in both your local repository and on GitHub.
