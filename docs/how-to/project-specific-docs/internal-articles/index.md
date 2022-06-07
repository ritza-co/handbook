# Working on 'internal' articles

Most of the content we create is used by other companies to get exposure and brand awareness. We also [dogfood](https://en.wikipedia.org/wiki/Eating_your_own_dog_food) our own service by creating articles for Ritza.

These serve different purposes, including 

* Giving our writers practice
* Supporting the Ritza.co domain which helps our main page rank better and people to discover us
* So we can experiment with SEO and see what kinds of things help an article to rank well on search engines
* A potential source of future monetization - we could add company-specific ads to these articles where relevant, or a general advert for Ritza.

## Creating an internal article

We have a repository of internal articles at [https://github.com/ritza-co/internal-articles](https://github.com/ritza-co/internal-articles). To create one, simply add a markdown file to the `docs` folder. Note the points below.

### Hiding the Navigation sidebar

* You should prefix the document with some YAML to hide the navigation (this stops all articles being listed on every article, as they are only loosely related). You should do this by adding the four lines right at the top of the markdown file, followed by an empty line, followed by the title as a heading one, as in the example below.

```
---
hide:
  - navigation
---

# Better Google Trends graphs using Python and seaborn
```

### Choosing a good URL / title

The URL will be built from the first heading in your file, the title. This URL (e.g. https://ritza.co/articles/kubernetes-vs-docker-vs-openshift-vs-ecs-vs-jenkins-vs-terraform) is important for ranking well, so try to include a phrase that people are likely to search for in this first heading.

### Adding images or other assets

If you need to link to images or other assets, create a folder inside the `docs/assets` folder using the same name as your markdown file name. All images and assets should be stored there, unless they are too large for GitHub. If your article is called 'working-on-internal-articles.md`, then you should create a folder called `working-on-internal-articles` in the assets folder. You can use these files in markdown in the following examples

```markdown
A file download
[Download the .zip file](../assets/working-on-internal-articles/my-zip-file.zip)

An image
![How to download a zip file](../assets/working-on-internal-articles/how-to-download-zip.png)
```

