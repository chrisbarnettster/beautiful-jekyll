---
layout: post
title: Is this tracked
bigimg: /img/octocatninjas.jpg
tags: [git, tips]
---

When jumping across branches, merging and maybe cleaning out a git repository, I often wonder...

# ** Is this thing tracked? **

- list all tracked files:
  - `git ls-files`
  - `git ls-files | grep myfile`
- see all untracked files:
  - `git status -u`
- see all untracked files and **all ignored files**:
  - `git status -u --ignored`

Credits:
Created the pic using [kimonocat](https://s-media-cache-ak0.pinimg.com/originals/aa/e9/fa/aae9fa8f8275b347515627de7e537d18.png) and [ninjaoctocat](https://s-media-cache-ak0.pinimg.com/564x/c6/52/55/c65255299cf0bf369a3b192b204e507d.jpg)
