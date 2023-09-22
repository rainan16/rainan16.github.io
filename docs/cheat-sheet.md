<!-- .slide: -->
# Cheat sheets
<--break-vertical-->

## Git

### How to set git username/email
To set your global username/email
```bash
git config --global user.name "FIRSTNAME LASTNAME"
git config --global user.email "MYNAME@example.com"
```

To set repository-specific username/email
```bash
git config user.name "FIRSTNAME LASTNAME"
git config user.email "MYNAME@example.com"
```

Verify configuration by
```bash
cat .git/config
```
<--break-vertical-->

### Undo last commit (local, NOT pushed)
Undo last commit, `--soft` leaves changed files as "Changes to be committed":
```bash
git reset --soft HEAD~
```

### Undo previous commits (local, NOT pushed)
Identify the hash of the "last good" commit with `log` and ust it in `reset`. The option `--hard` deletes any changes (throw away):
```bash
git log --oneline
git reset --hard *commit_hash*
```

### Undo a specific commit (local, ALREADY pushed)
Actually this is not removing a commit, but reverting any changes by adding new "revert"-commit.  
So identify the hash of a specific commit with `log` and use it in `revert`:
```bash
git log --oneline
git revert *commit_hash* --no-edit
```

<--break-vertical-->

## Docker / Docker Compose

Todo

<--break-vertical-->

## k8s

Todo






