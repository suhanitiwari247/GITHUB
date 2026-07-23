# 🚀 Git - Zero to Hero

> A complete Git guide from beginner to advanced with commands, examples, workflows, interview questions, and best practices.

---

# 📚 Table of Contents

1. Introduction
2. What is Git?
3. Why Git?
4. Git vs GitHub
5. Installation
6. Configure Git
7. Create Repository
8. Git Workflow
9. Git Areas
10. Basic Commands
11. File States
12. Commit
13. Branching
14. Merging
15. Merge Conflicts
16. Stashing
17. Remote Repository
18. GitHub Workflow
19. Pull Requests
20. Rebase
21. Cherry Pick
22. Reset
23. Revert
24. Tagging
25. Logs
26. Ignore Files
27. Undo Changes
28. Git Internals
29. Git Best Practices
30. Common Mistakes
31. Interview Questions
32. Cheat Sheet

---

# 1. Introduction

Git is a Distributed Version Control System (DVCS).

It tracks changes in source code.

Created by:
Linus Torvalds (2005)

Used by:

- Google
- Microsoft
- Amazon
- Netflix
- Meta
- Open Source Projects

---

# 2. Why Git?

Without Git

Developer A
↓

Developer B

↓

Files get overwritten

↓

Code lost

With Git

Developer A
        ↘
         Git Repository
        ↗
Developer B

Advantages

✔ Version Control

✔ Team Collaboration

✔ Backup

✔ Branching

✔ Easy Rollback

✔ Open Source Contribution

---

# 3. Git vs GitHub

Git

- Software
- Installed locally
- Tracks code
- Free

GitHub

- Cloud platform
- Stores repositories
- Collaboration
- Pull Requests
- Issues

Remember

Git != GitHub

---

# 4. Installation

Windows

Download Git

https://git-scm.com/

Linux

sudo apt install git

Mac

brew install git

Check Version

git --version

---

# 5. Configure Git

Username

git config --global user.name "John"

Email

git config --global user.email "john@gmail.com"

Check Config

git config --list

---

# 6. Create Repository

New Repository

git init

Clone Existing Repository

git clone URL

Example

git clone https://github.com/user/project.git

---

# 7. Git Workflow

Working Directory

↓

Staging Area

↓

Local Repository

↓

Remote Repository

Commands

git add

↓

git commit

↓

git push

---

# 8. Git Areas

Working Directory

↓

Files you edit

Staging Area

↓

Files ready to commit

Repository

↓

Permanent history

---

# 9. File States

Untracked

↓

Tracked

↓

Modified

↓

Staged

↓

Committed

---

# 10. Basic Commands

Status

git status

Initialize

git init

Clone

git clone URL

Add

git add file

Add All

git add .

Commit

git commit -m "message"

Push

git push

Pull

git pull

Fetch

git fetch

Log

git log

---

# 11. Commit

Commit saves snapshot.

Example

git commit -m "Added Login Page"

Good Commit Message

Add login validation

Bad

update

---

# 12. Branch

Create Branch

git branch feature

Switch

git checkout feature

Modern

git switch feature

Create + Switch

git checkout -b feature

Delete

git branch -d feature

List

git branch

---

# 13. Merge

Main

↓

Feature

↓

Merge

Command

git merge feature

---

# 14. Merge Conflict

Occurs when

Same file

Same line

Different changes

Resolve

Open file

Fix manually

git add .

git commit

---

# 15. Remote Repository

Add Remote

git remote add origin URL

View

git remote -v

Change URL

git remote set-url origin URL

---

# 16. Push

First Push

git push -u origin main

Next

git push

---

# 17. Pull

Download latest code

git pull origin main

---

# 18. Fetch

Downloads changes

Does NOT merge

git fetch

---

# 19. Git Ignore

Create

.gitignore

Example

node_modules/

dist/

.env

*.log

---

# 20. Logs

Simple

git log

One Line

git log --oneline

Graph

git log --graph

Decorated

git log --decorate

---

# 21. Diff

Compare changes

git diff

Staged

git diff --staged

---

# 22. Stash

Temporary save

Save

git stash

List

git stash list

Apply

git stash apply

Pop

git stash pop

Delete

git stash drop

---

# 23. Reset

Soft

git reset --soft HEAD~1

Mixed

git reset HEAD~1

Hard

git reset --hard HEAD~1

---

# 24. Revert

Undo commit safely

git revert COMMIT_ID

---

# 25. Rebase

Cleaner history

git rebase main

Interactive

git rebase -i HEAD~5

---

# 26. Cherry Pick

Copy one commit

git cherry-pick HASH

---

# 27. Tags

Create

git tag v1.0

Push

git push origin v1.0

List

git tag

---

# 28. Remove Files

git rm file

Restore

git restore file

---

# 29. Undo Changes

Discard

git restore file

Undo Add

git restore --staged file

Undo Commit

git reset

---

# 30. Branch Strategy

main

↓

develop

↓

feature/login

↓

feature/payment

↓

bugfix

↓

release

---

# 31. GitHub Workflow

Fork

↓

Clone

↓

Create Branch

↓

Commit

↓

Push

↓

Pull Request

↓

Review

↓

Merge

---

# 32. Pull Request

Purpose

Merge code

Review

Comments

Approval

---

# 33. Git Internals

Git Objects

Blob

Tree

Commit

Tag

HEAD

Pointer to current branch

---

# 34. Useful Commands

Current Branch

git branch

History

git log

Remote

git remote -v

Branches

git branch -a

Last Commit

git show

---

# 35. Git Aliases

git config --global alias.st status

git config --global alias.co checkout

git config --global alias.br branch

git config --global alias.cm commit

git config --global alias.last "log -1"

---

# 36. Best Practices

✔ Commit frequently

✔ Small commits

✔ Meaningful messages

✔ Pull before push

✔ Use branches

✔ Never commit passwords

✔ Write README

✔ Review code

---

# 37. Common Errors

Error

Permission denied

Solution

SSH Key

-------------------

Error

Merge Conflict

Solution

Resolve manually

-------------------

Error

Repository not found

Solution

Check URL

-------------------

Error

Nothing to commit

Solution

Modify files

---

# 38. Git Interview Questions

### Beginner

What is Git?

Difference between Git and GitHub?

What is repository?

What is commit?

What is branch?

What is merge?

What is clone?

What is pull?

What is push?

What is fetch?

---

### Intermediate

Difference between Merge and Rebase?

Difference between Reset and Revert?

HEAD?

Detached HEAD?

Cherry Pick?

Stash?

Fast Forward Merge?

Merge Conflict?

---

### Advanced

Git Object Model

Pack Files

Garbage Collection

Hooks

Reflog

Submodules

Git LFS

Bisect

Sparse Checkout

Worktrees

---

# 39. Git Cheat Sheet

Initialize

git init

Clone

git clone URL

Status

git status

Add

git add .

Commit

git commit -m "message"

Branch

git branch

Switch

git switch branch

Merge

git merge branch

Push

git push

Pull

git pull

Fetch

git fetch

Log

git log

Diff

git diff

Reset

git reset

Revert

git revert

Stash

git stash

Tag

git tag

Remote

git remote -v

---

# 40. Complete Git Flow

Create Project

↓

git init

↓

git add .

↓

git commit

↓

Create GitHub Repo

↓

git remote add origin URL

↓

git push

↓

Create Feature Branch

↓

Develop

↓

Commit

↓

Push

↓

Pull Request

↓

Merge

↓

Delete Branch

---

# 🎯 Learning Roadmap

Week 1
- Git Basics
- Repository
- Commit
- Status
- Add

Week 2
- Branch
- Merge
- Pull
- Push

Week 3
- GitHub
- Pull Request
- Fork
- Collaboration

Week 4
- Rebase
- Cherry Pick
- Hooks
- Git Internals

---

# 📖 Recommended Resources

Official Docs:
https://git-scm.com/docs

GitHub Docs:
https://docs.github.com/

Atlassian Git Tutorials:
https://www.atlassian.com/git

---

# ⭐ Conclusion

Git is one of the most essential tools for every software developer.

Master:
- Git Basics
- Branching
- Merging
- GitHub Workflow
- Collaboration
- Advanced Git

Practice daily to become proficient.

Happy Coding! 🚀
