---
permalink: /lectures/f19/week2.html
---

class: center, middle

# Everybody Gits

.copyright[
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a>
** [Pat Pannuto](http://patpannuto.com) / Marcus Darden **
]

---

# What is version control?

## Why is it important?

## ...and how might we build a version control system?

---

# The Last Pun You'll Git

---

# Git Basics

## The Top 5

 - `git init`

 - `git status`

 - `git add` and `git commit`

 - `git log`

--

## Let's peek under the hood

 - History is a linked list

 - What's `master`, `HEAD`?

 - Where's the old versions?

???

## I'm lazy, let's make `git st` == `git status`

 - `git config --global --edit`
.small-75[
 - (Fancy way of saying `editor ~/.gitconfig`)

 - (Fancy way of saying `editor /home/ppannuto/.gitconfig`)

 - (Fancy way of saying `[nano/vim/emacs/...] /home/ppannuto/.gitconfig`)
]

```
[alias]
  st = status
```

???

master is a branch like any other, and just a name _nothing special to git_
                                                  _special to users by convention_

HEAD is an alias for what is currently "checked out", the files that you
see on disk at this moment

where are the others?
   - .git/objects

Check out .git/HEAD while we're here

---

# A good commit message

## Use an editor!

## Take your time

--

## The "Title"

 - 50 chars or less

 - Starts like a sentence but doesn't end like one

 - Imperative!

--

## The "Body"

 - 72 chars or less per line

 - What and why

 - NEVER how (that's what the code is for)

 - Add any external references (eg. Fixes issue #42)

---

# Using git locally

 - What is a commit?

 - Working Directory, Staging Area, Repository

 - Moving around the triangle
--

<hr />

.center[
![Diagram of git operations](img/git_triangle-local.svg)
]

---

# Slow down!

## Git help

 - `man git` (the stupid content tracker)

 - `git help <command>` or `man git-<command>`

 - `man gittutorial`

 - `man giteveryday`

 - The Internets
--

## Some git "tools"

 - `git config`

 - `git diff`

 - `git stash`

 - `git show`

 - `git blame`

---

# Collaborating with git

## Git remotes

 - `git remote`

 - `git clone`

--

<hr />

![Diagram of git operations with remote server](img/git_triangle.svg)

---

# To and from the "Cloud"

 - `git push`, `git fetch`

 - `git merge`

 - `git pull`

---

# Attendance

## [tinyurl.com/csprag-f19-everybody-gits]()


---

name: git-examples

# Other

## Examples of git in IDE/editors

 - [Xcode](#xcode-gallery)

 - [VS Code](#vscode-gallery)

 - [Vim/gVim](#vim-gallery)

--

## Darden's git favorites

 - [Git Golf](https://learngitbranching.js.org)

 - [Git Commit Messages](https://hackernoon.com/git-it-together-some-tips-on-commit-etiquette-and-best-practices-for-junior-developers-1f147b8dfd56)

 - [Pragmatic Guide to Git](https://pragprog.com/book/pg_git/pragmatic-guide-to-git)

---

# Closing remarks

## **You (EECS 201) must use git for something non-trivial this term**

 - You (everyone) _should_ use version control for all your class projects

    - And I don't mean folder-copying

 - Not in any programming classes?

    - Try using it for other homework or a side project!

 - Deadline for this is Week 5 — Git II (February 08)

