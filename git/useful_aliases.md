# Git aliases


### Today’s Work

# full command: 

```git log --since=00:00:00 --all --no-merges --oneline --author=<your email address>```

# Alias: 

```git config --global alias.today "log --since=00:00:00 --all --no-merges --oneline --author=<your email address>"```

### Leaderboards

Top commiters for the repository:

```git shortlog -sn```

```git config --global alias.leaders "shortlog -sn"```

### Remind Yourself What You’ve Been Up To

git config --global alias.recap "git log --all --oneline --no-merges --author=<your email address>"


### See What Everyone’s Been Getting Up To

```git log --all --oneline --no-merges```
