There are several GitHub repos to keep in mind when working on Replit's docs site.

The main repo, owned by Replit, is at https://github.com/replit/replit.github.io. We refer to this as `upstream` and devs working on it will usually track is as 
`git remote add upstream https://github.com/replit/replit.github.io`

We also keep our own fork of this repo at https://github.com/ritza-co/replit.github.io. Devs working on Replit will usually track this as the `origin` remote, default 
after `git clone git@github.com:ritza-co/replit.github.io.git`

As a workflow, new tutorials should be added as a branch in *our* fork. We work internally by making pull requests to this branch, so e.g. the author or QA engineer 
will create the branch, and language and technical editing will happen in there. Once the branch is finalised internally, we open a pull request across the forks from 
our fork to the master branch of Replit's main repo, from where we can deploy the changes live.
