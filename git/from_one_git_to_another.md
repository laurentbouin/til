# To migrate all tag/branches from one git to another: 


### 1. Clone every branches

```git clone --mirror current_repository_url```

### 2. Open the repo

### 3. Setup a new remote

```git remote add remoteName new_repository_url```

### 4. Push all refs under refs/heads

```git push -f --tags remoteName refs/heads/*:refs/heads/*```


