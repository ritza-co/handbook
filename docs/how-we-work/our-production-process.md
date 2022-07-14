# Our master workflow for producing great writing

To some extent, we customise our workflow to each project. Sometimes we have different roles, people taking on more than one role, or extra pieces. But in general these modified workflows are still based on this one.

## Roles

* Project manager - discusses potential topics with the writer, communicates anything that should definitely be included, and sets a timeline
* Writer-engineer - an engineer who creates any code samples and writes the article
* QA-engineer - a second engineer who follows the article, converts it into markdown + git if necessary, and creates high quality screenshots
* Designer - creates a cover image and designs any in-article graphics or diagrams for the article, matching the brand our customer
* Editor - a language expert improves the flow, fixes any language errors, and gives feedback to the writer, working with the writer on revisions to the text if necessary.
* Publisher - hits the publish button to put the post live
* Distributor - shares the post on various social platforms and aggregators

## Platforms

Articles are generally produced either using Google Docs or Markdown. If we use Markdown, articles are tracked in our GitHub organization in a private fork of our customer's repository where the article will finally be published.

We communicate mainly over Slack, and track an overview of the status of each article in Trello. In the case of articles in Google Docs, some communication may be done through Google Docs comments or edit suggestions. For larger projects with more people involved, we may have status meetings using Zoom, or people may meet 1:1 over Zoom to discuss any problems that arise.

## Git workflow

Imagine a customer named Acme who has a Markdown-based blog called Acme Blog. They have a GitHub repository at `https://github.com/acme/acme-blog`. We have a fork of their repository at `https://github.com/ritza-co/acme-blog`. We are working on a new article called `how-to-foo-your-bar-with-baz`

### Drafting

The writer will have a local copy of our fork on their machine. They will create a new branch for the article, off the `main` branch.

```
git checkout -b add-foo-bar-baz-article 
```

They will then work on the draft of their article using whatever editor they are most comfortable with. If they are not comfortable with git or are not part of our GitHub organization, they will simply work in a markdown file and share this by email or Slack and it will rather be integrated into GitHub at the QA stage.

Once they are done, the writer will share their work in the `#ritza-acme` Slack channel.

### Quality assurance

If the writer did not use GitHub, the QA engineer will create the git branch as described above and add a commit with "original author's work" or similar, before making any changes.

The QA engineer will look at the writer's work and try it out, making sure all example code and commands work as expected. If the writer did not have a 4k or Retina screen while taking any screenshots, the QA engineer will also retake these screenshots, and possibly annotate them. The QA engineer will then commit any changes or improvements with a commit like 'quality assurance updates`. For larger changes, the QA engineer may make a new branch, and merge these changes into the writer's branch.

Once they are done, the QA engineer will share the link again in the `#ritza-acme` Slack channel.

### Editing

The Editor will look at the article and make language changes, often through the GitHub interface. The Editor will then commit these changes into the same `add-foo-bar-baz` branch. For larger changes, they may branch off and then merge back in again.

Once done, the Editor will share the GitHub link showing all the changes made by the edit with the writer, and share in the `#ritza-acme` channel that the edit is complete.

### Publishing

The Publisher will open a pull request from `ritza-co/acme-blog:add-foo-bar-baz` article into `acme/acme-blog:main` or equivalent.

### Distributing

The Distributor will copy the article to dev.to, hashnode, linkedin, Twitter, and possibly post on Hackernews and/or Reddit.












