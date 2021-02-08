# git-bash

git bash commands

```shell
git --version
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

Checkout allow return back to a specific commit.
```shell
git checkout [shorthash|hash]
```
```shell
git checkout master
```
