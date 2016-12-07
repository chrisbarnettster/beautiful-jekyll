---
layout: post
title: Careful merges with git
subtitle: let's not lose anything!
bigimg: /img/octocatninjas.jpg
tags: [git, tips]
---

*For when you worry that a merge may overwrite things that you don't want overwritten and you are a little bit paranoid (maybe you've lost things before)*

## Start the merge
Tell git not to commit by default because you assume all content on this branch will be lost somehow.

 - `git merge --no-commit master`

Note this will autocommit a fast forward [(that is good!)](http://stackoverflow.com/questions/8640887/git-merge-without-auto-commit)

## Double check all is in order
Make sure you're happy. Make edits as appropriate. Maybe run a unit test.

- `Git difftool --cached ; git diff --cached`

## Abort the merge!!
If things are not cool:

-   `git reset --merge`

## Confirm the merge

- use `git status` to see what is going on
- add necessary changed files  `git add files-that-need-adding`
- commit. `git commit`

Credits:
Created the pic using [kimonocat](https://s-media-cache-ak0.pinimg.com/originals/aa/e9/fa/aae9fa8f8275b347515627de7e537d18.png) and [ninjaoctocat](https://s-media-cache-ak0.pinimg.com/564x/c6/52/55/c65255299cf0bf369a3b192b204e507d.jpg)
