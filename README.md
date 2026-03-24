# OST Git Demo

## Steps Performed

### Step 1: Configure Git User

```
C:\Users\harsh> git config --global user.name \"Dev Malde\"
C:\Users\harsh> git config --global user.email \"dev.malde12@gmail.com\"
```

### Step 2: Verify Git Installation

```
C:\Users\harsh>git --version
git version 2.53.0.windows.1
```

### Step 3: Create and Initialise Repository

```
C:\Users\harsh>mkdir ost
C:\Users\harsh>cd ost
C:\Users\harsh\\ost>git init
Initialized empty Git repository in C:/Users/harsh/ost/.git/
```

### Step 4: Check Repository Status

```
On branch master
No commits yet
nothing to commit (create/copy files and use \"git add\" to track)
```

### Step 5: Create and Verify File

```
C:\Users\harsh\\ost>echo Hello > sample.txt
C:\Users\harsh\\ost>type sample.txt
Hello
```

### Step 6: Add and Commit File

```
[master (root-commit) eb75f55] Initial Commit
 1 file changed, 1 insertion(+)
 create mode 100644 sample.txt
```

### Step 7: Rename Default Branch

```
git branch -m master main
```

### Step 8: Create Development Branch

```
git checkout -b dev
Switched to a new branch 'dev'
```

### Step 9: Modify File and Commit

```
echo Hello from dev >> sample.txt
git add .
git commit -m \"Update in dev\"
[dev 88c70b6] Update in dev
 1 file changed, 1 insertion(+)
```

### Step 10: Merge Branches

```
git checkout main
git merge dev
Updating eb75f55..88c70b6
Fast-forward
 sample.txt | 1 +
 1 file changed, 1 insertion(+)
```

### Step 11 & 13: Push to Remote Repository

```
git remote add origin https://github.com/hdave-mu/ostdemo.git
git push -u origin main
To https://github.com/hdave-mu/ostdemo.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
```

Repo is fully set up and pushed to GitHub.
