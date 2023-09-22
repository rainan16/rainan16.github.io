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
`--soft` leaves changed files
```bash
git reset --soft HEAD~
```

### Undo previous commits (local, NOT pushed)
`--hard` deletes any changes (throw away)
```bash
git log --oneline
git reset --hard *commit_hash*
```

### Undo a specific commit (local, ALREADY pushed)
not removing, but adding a new "revert"-commit
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






