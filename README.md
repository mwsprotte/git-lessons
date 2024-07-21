# Compiled of Git Commands
This repository it’s my personal little compiled of Git commands that I consider useful. I made this based in my diary use and expect this can be useful for another peoples.

- Clone a repository:

```
git clone REPOSITORY_LINK.git
```

- Upload modification to actual repository:
```
git status
```
```
git add .
```
```
git commit -m"MESSAGE"
```
```
git push
```

This commands may be combined like this:

```
git status && git add . && git commit -m"MESSAGE" && git push

```
- To download the remote modifications:

```
git pull

```
- Revert to a anterior commit (locally):
```
git log
```
> :bulb: **Tip:** To quit type `:q`

```
git commit -m"MESSAGE"
```
```
git reset COMMIT_HASH        
```
```
git clean -n
```

```
git clean -f
```

- To create a new branch and switch to him:
```
git checkout -b NEW_BRANCH
```
- List the available branches:
```
git branch
```
- Switch to another branch:
```
git checkout BRANCH_NAME
```
- Delete a branch (locally):
```
git branch -D BRANCH_NAME
```
- Turn the local branch the same as remote:
```
git fetch origin && git reset --hard origin/master && git clean -f
```
- Rename the actual branch:
```
git branch -m novo-nome-da-branch
```
- Rename the local branch from another local:
```
git branch -m nome-atual novo-nome
```

- Show the conflicts with remote:
```
git diff
```

- To init a local branch based on a remote one:

git fetch origin                             # update remote tracking branch
git checkout -b your_develop origin/develop  # create new local develop branch