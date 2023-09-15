<!-- .slide: -->
# Cheat sheets


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