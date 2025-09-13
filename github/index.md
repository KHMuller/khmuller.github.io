---
title: Frequently Used Git/Github Commands
description: Steps and commands used in different version control operations
layout: default
canonical: https://khmuller.github.io/github/
---

# Frequently Used Git/Github Commands

## Clone github repository

~~~bash
git clone https://github.com/username/repository.git
~~~

## Delete file from current branch

Deletes a file from local and remote repository.

~~~bash
git rm <file>
git commit -m "Deleted a file"
git push
~~~

## Delete all history of a git repository

Delete repository history and hence clean up tracking of deleted files. This is achieved by creating a branch without history, deleting the original branch and then rename the new branch with the old name.

~~~bash
git checkout --orphan temp_branch
git add -A
git commit -am "The First Commit"
git branch -D main
git branch -m main
git push -f origin main
~~~

{: .enhanced}
Markdown for paragraph with assigned class.
