---
title: "Tips for Setting Up Your Blog With Hugo 2018"
date: 2018-01-09T17:50:19+09:00
draft: true
---

There are many open source softwares for making a blog. Particularly, **Hugo** is becomming a first option when we make our blog without any dynamic softwares like WordPress. As far as I remember there is also a product named Octopress, but its development is stopped from 2015.

There are several useful tips when you make an actual blog with Hugo and GitHub Pages:

## Use snap for installation (for Linux users)

Snapcraft is a relatively new package system for Linux. It's easy to use and providing faster installation time compared to install via Go or options.

```
snap install hugo
```

## Do not commit raw contents to master

If you want to make a GitHub user's page, you will be affected by the limits that GitHub Pages only allows using master branch for deploying. So that I recommend following steps.

1. Clear all files inside master branch and make an empty commit.
2. Switch to develop branch, then `git worktree add -B master public`

Step 2 mounts master branch as `/public` directory
