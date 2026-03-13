# Git Homework - Repository

## Overview
This repository demonstrates Git workflow skills including history cleanup,
recovering lost commits, branching, tagging, and custom aliases.

## Steps Completed
1. Initialized a Git repository
2. Made commits with unclear messages (`update`, `stuff`, `final`)
3. Cleaned up history by squashing commits into one meaningful message
4. Simulated a lost commit using `git reset --hard`
5. Recovered the lost commit using `git reflog`
6. Created a new branch `recovered-work` from the recovered commit
7. Created a custom Git alias for visual history
8. Tagged the clean version as `v1.0`

## Custom Git Alias
To view commit history in a clear and visual format, I created the following alias:

### Setup
```bash
git config --global alias.hist "log --oneline --graph --decorate --all"
```

### Usage
```bash
git hist
```

### Output Example
```
* 83ec403 (recovered-work) bad commit - should not be here
* c381820 (HEAD -> main) feat: initialize project with feature A and bug fix
```

This alias displays a visual tree of all branches and commits in a clean, readable format.

## Branches
- `main` — clean, squashed commit history
- `recovered-work` — branch created from recovered lost commit

## Tags
- `v1.0` — marks the cleaned-up version of the project