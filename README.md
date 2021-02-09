# git-bash

git bash commands

```shell
git --version
```

### init:

init with a empty dir:
```shell
git init
```

### config:

Global config (just once):
```shell
git config --global user.name "your-name"
```
```shell
git config --global user.email "your-git-email"
```

Local config (for each project):
```shell
git config user.name "your-name"
```
```shell
git config user.name "your-mail"
```

### commit:

Index files before commit:
```shell
git add your-file.txt
```
```shell
git add .
```
```shell
git add *
```

Commit:
```shell
git commit -m "Commit comment"
```

### status:

```shell
git status
```

### log:

```shell
git log
```
exit from git log preview CTRL+Z.

```shell
git log --pretty=oneline
```
```shell
git log --pretty=oneline --max-count=3
```
```shell
git log --pretty=oneline --all
```
```shell
git log --pretty=oneline --author="your-name"
```

Log with custom format:
```shell
git log --pretty="%h %ad | [%an] : %s" --date=short
```

### checkout:

```shell
git checkout [shorthash|hash]
```
```shell
git checkout main
```
```shell
git checkout "file-name"
```

### reset:

```shell
git reset HEAD "file-name"
```
```shell
git reset [shorthash|hash]
```

### clean:

```shell
git clean -n
```
```shell
git clean -f
```
```shell
git clean -fd
```

### revert:

```shell
git revert HEAD --no-edit
```
```shell
git revert [shorthash|hash] --no-edit
```
```shell
git revert --continue
```
```shell
git revert --abort
```

### branch:

```shell
git branch [-a]
```
```shell
git checkout -b new-branch-name
```
```shell
git checkout branch-name
```
```shell
git merge branch-name
```

### rebase:

```shell
git rebase branch-name
```

### clone:

```shell
git clone https://github.com/popexandru/git-bash.git
```
```shell
git clone git@github.com:popexandru/git-bash.git
```

### origin & push:

```shell
git remote add origin https://github.com/popexandru/git-bash.git
```
```shell
git push -u origin main
```
