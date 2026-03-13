# Git Homework - Repository

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