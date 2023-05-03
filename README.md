# 📓 The Ritza Handbook

## ⚠️ Work in Progress

This is a very early stage, work-in-progress collection of documents that we use to coordinate at https://ritza.co.

If you want to work with Ritza, check out:

* [Writing for Ritza](./writing-for-ritza.md)
* [Our job opening for a Backend Freelance writer](./jobs/backend-freelance-writer.md)
* [Our style guide](./ritza-style-guide.md)


## Contributing to the handbook

To contribute to the handbook, you should set up a local development environment to preview your changes before making a pull request. You'll need a Python development environment locally and you should be comfortable with virtualenv and pip.

1. Clone this repository locally, and change into the handbook repository.

```
git clone git@github.com:ritza-co/handbook.git
cd handbook
```

2. Create and activate a virtual environment

```
python3 -m virtualenv venv
source venv/bin/activate
```

3. Install requirements

```
pip3 install -r requirements.txt
```

4. Preview the site 

```
mkdocs serve
```

5. Visit the local site

Open http://localhost:8000/handbook in your web browser. Any markdown files you edit and save should be automatically rebuilt and previewed in your browser.

Once you've added new markdown files or edited existing ones, add the changes and push them up to a branch. e.g. 

```
git checkout -b add-my-cool-new-page
git add docs/my-cool-new-page.md
git commit -m "Add my cool new page"
git push origin add-my-cool-new-page
```

Git will prompt you to make a pull request on GitHub. Follow the the link and open the PR.













