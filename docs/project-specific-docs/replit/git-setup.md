The main GitHub repository for Replit is at github.com/replit/replit.github.io.

We keep a fork of this at github.com/ritza-co/replit.github.io

When adding new work, we branch off our fork (usually set this to `origin` if you're working with git locally). We collaborate on this branch for writing, QA, editing, etc, and then make a request to merge it directly into their repository

So the pull request would be something like 

`ritza-co/replit.github.io/add-chatbot-tutorial` into `replit/replit.github.io/master`.

We then do a hard reset of our master to upstream to bring that work in to our 'main' branch. We don't merge feature branches directly into our master branch, nor do we use this for anything except as a clean slate to start new feature branches.


<img width="735" alt="image" src="https://user-images.githubusercontent.com/2641205/114547571-e18e7280-9c5e-11eb-9131-7c03f1bd0965.png">

