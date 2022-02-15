# Using Git for Replit

We keep a fork of Replit's documentation repository in the Ritza organization.

Replit merges their own work into the docs repository throughout the month. In order to make sure we are always working from a 'fresh' version, we should branch off *their* master branch, not ours.

The easiest way to do this is as follows.

## Setting up

**This assumes you already have git installed locally, and are set up with the correct permissions on the Ritza GitHub org**

Clone our fork of their repository to your local machine

```bash
git clone git@github.com:ritza-co/replit.github.io.git
```

You now have a copy on your own machine, with the remote called "origin" pointing to our fork on GitHub

```bash


Local   ------> origin


```

Add the Replit version as a new remote by running:

```bash
cd replit.github.io
git remote add replit git@github.com:replit/replit.github.io.git
```

Now your local version knows about two remotes, "origin" (Ritza) and "replit" (Replit). You can verify this by running

```bash
git remote get-url origin
git remote get-url replit
```

```bash

              /- origin
Local   -----/
              \- replit


```
For convenience, add `ritza` as a remote too, with the same URL as `origin`.

```bash
git remote add ritza git@github.com:ritza-co/replit.github.io.git
```

## Making a change to the documentation

To make a change to the docs (e.g. adding a new tutorial, or fixing an existing page), you should always

1. Update your local master branch, so that it matches Replit's master
2. Branch off your (now up-to-date) local master branch into a new local branch
3. Push this new branch to the *Ritza* remote (you won't have permission to push to Replit's version directly)
4. Open a pull request into Ritza's mater branch (this won't be merged, and will be transfered to a PR against the Replit version, but we can use it for internal coordination)


```bash
[ Replit's version]         [Ritza's Fork]
    master

     |                              ^
     | git pull                     | git push ritza add-wordle-tutorial      
     |                              |
     v                              |

[Your local version]----------- add-wordle-tutorial
       master         git checkout -b 
```

## Steps to achieve this

```bash
# ensure you're on master, pull in the new changes, and hard reset your branch to match theirs
git checkout master
git pull replit master
git reset --hard upstream/master

# create a new branch off your clean local master branch
git checkout -b add-wordle-tutorial

# make the changes you want
# ...
# -------------------------

# push your changes to ritza
git add .
git commit -m "added draft wordle tutorial"
git push ritza add-wordle-tutorial

# you'll now see a link that you can visit to open the PR
```










