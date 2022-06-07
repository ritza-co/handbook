# Adding new docs

Each section you can see in the sidebar in [docs.replit.com](https://docs.replit.com) has a corresponding folder in the main repository at [https://github.com/ritza-co/replit.github.io](https://github.com/ritza-co/replit.github.io). To add a new doc, add a new markdown file to the relevant folder, update the sidebar.json file (covered below) and add any images/screenshots to a directory with the same name as the doc in `static/images...`.

## Images

Each section also has a folder in the `static/images` directory. These are not always named the same as the folder for the markdown files -- for examples `teams-edu` in the root folder corresponds to `teamsForEducation` in `static/images`. 

Inside the respective folder, create a new folder for your tutorial named the same as your markdown file without the `.md` extension.

To refer to the image in the markdown file, omit the `static` part of the relative reference.

### Example

You're adding a 'git command line tutorial' file to the 'programming ide' section. You would

* Create a new file called `git-command-line-tutorial.md` to the `programming-ide` folder in the root of the repository.
* Create a new folder called `git-command-line-tutorial` in `static/images/programming-ide`.
* Add any images you need to that new directory.
* To refer to an image called `image1.png` in the markdown file, you would use `/images/programming-ide/git-command-line-tutorial/image1.png`.

## Sidebar.json

The `sidebar.json` file in the root of the repository contains JSON definitions of the sidebar / table of contents. Add your tutorial to the relevant section. 

* For `slug` use the name of your markdown file without the `.md` extension
* For `name` usually use the same name as the title / first line of your markdown file (the H1), but if it's longer than 3-5 words then shorten it for hte sidebar title.

## Opening the pull request

See [Using Git for Replit](https://ritza.co/handbook/project-specific-docs/replit/using-git/).






