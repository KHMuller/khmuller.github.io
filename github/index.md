---
title: Frequently Used Git/Github Commands
description: Steps and commands used in different version control operations
layout: default
canonical: https://khmuller.github.io/github/
---

## Frequently Used Git/Github Commands

### How to Connect Local Folder to Private GitHub Repository
I use this approach when I want to maintain a backup of a folder which I later can easily clone on another computer.

1. Create private repository in GitHub with README.md
2. Copy url of this new repository (under &lt;code&gt; / Code)
3. In terminal change directory to future parent folder where the local copy will reside and clone the new repository.
4. Add files to the new created local folder, commit and push changes. Don't forget adding a .gitignore file

Cloning repository. You may have to login first with git login
~~~bash
git clone <url-to-git-repository>
~~~

### Delete file from current branch
Deletes a file from local and remote repository.

~~~bash
git rm <file>
git commit -m "Deleted a file"
git push
~~~

### Delete all history of a git repository
Delete repository history and hence clean up tracking of deleted files. This is achieved by creating a branch without history, deleting the original branch and then rename the new branch with the old name.

~~~bash
git checkout --orphan temp_branch
git add -A
git commit -am "The First Commit"
git branch -D main
git branch -m main
git push -f origin main
~~~


