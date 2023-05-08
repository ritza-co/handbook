# Prepare and cross-post Bryntum articles

We prepare Bryntum drafts in markdown, but later prepare different formats of the same article. We should always treat the markdown version in GitHub as the canonical version, so any changes made later to other versions should always be backported to the markdown version.

## Overview of formats and versions

* The markdown version in GitHub - https://github.com/ritza-co/bryntum
* A wordpress version for their blog. This we prepare as a **draft** on their **staging server**, and they publish it to live from there
* A medium version for their Medium.com account
* A dev.to version for the Dev.to account
* [for migration guides] - a markdown version in their docs repository. Their docs are in a mono-repo with their source code which they are very protective over, so we have a [bryntum-docs](https://github.com/ritza-co/bryntum-docs) repository that mirrors the same structure as their main repo, but only including the docs we are working on.

## Overview of process

* Once an article has gone thorugh drafting, QA, and editing, it can be uploaded to wordpress. Create a draft (guide below) on wordpress and add a header image.
* Copy the HTML version of the wordpress version and craete a PR with this back to our main Bryntum GitHub repository. This is because WordPress can be janky and once all the finicky formatting is done we don't want to lose that work
* Once the article has been live on their WordPress blog for a couple of weeks, create a Medium.com and Dev.to version [guide to be created].

## Steps for creating a WordPress draft

The article should be copied from the GitHub by clicking and dragging over the article, rather than clicking on the `copy` button. This is because the `copy` button does not copy the text in markdown format, which we will need later on in the crossposting.

<video controls width="100%">
  <source src="https://i.ritzastatic.com/images/dc9b9558164b4bf282dea79c07dd4737/copy-markdown.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Next the article can be pasted into the Wordpress visual editor.

![WP Visual editor](https://i.ritzastatic.com/images/de362045d5e74d97a231c888229e6524/visual-editor.png)

Here the editor will automatically format the markdown. Not all of the article will be formatted correctly and some adjustments may need to be made.

## Code block syntax highlighting

In the WP `visual editor`, run through the article and check the block type of all of the code snippets. Convert all code snippets to the `code` block type.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/e1847978414a4c069fc45e349c3b4997/block-type-change.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

Swicth to the Wordpress `code editor` and run through all of the `<!-- wp:code -->` code blocks. Add the following class to both the `<pre>` and `<code>` tags of these blocks:

```html
class="language-(language-type-here)"
```

Ensure that the appropriate language is added to that class to ensure the code block has the correct syntax highlighting.

This can be made easier by copying the `html` version of the article from Wordpress, pasting into a text editor and using the find functionality (`cmd/ctrl+f`) to locate all of the `<!-- wp:code -->` blocks.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/13cbe24f40c54c0cb60869778e525b8c/text-editor.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

Each code block should be wrapped in a tag that looks something like this:

```html
<!-- wp:code -->
<pre
  class="language-javascript wp-block-code"
><code class="language-javascript">CODE-GOES-HERE</code></pre>
<!-- /wp:code -->
```

For HTML syntax use `markup` as the language in the class:

```html
<!-- wp:code -->
<pre
  class="language-javascript wp-block-code"
><code class="language-javascript">CODE-GOES-HERE</code></pre>
<!-- /wp:code -->
```

## Images, gifs, and videos

Go through the Wordpress block editor and delete the image blocks one by one and replace with the appropriate image for that section of the article.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/8da582080e4a495b90d61aac101560f9/image-upload.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

All video or gif files must be converted to `webm` format. You can use [this website](https://cloudconvert.com/mp4-to-webm) to do the converting.

### Making the header image

To make the header image take the screenshot of the final software demo, or if the article is a comparison between two demos take the screenshots of both software demos, and place these images inside the Bryntum frame found in the Figma project.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/c54991ccdeee469782f4c7122dcbb750/figma-header-work.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

Attach the header image in the cover image section.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/06b95173e7454ba092148e177f96318e/header-image.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

## Final checks

Once you have completed these steps, run through the article to make sure all the formatting has been copied over correctly. Check the headings, lists, bullet-points, images, etc.

### Changing the Ritza GitHub links

Any links to a Ritza GitHub repo in the article should be sent to Bryntum to fork, that Bryntum repository should replace any Ritza repository links in the article. Please check the article and let Bryntum know if they need to fork all branches of the repository.

### Pick an article category

Make sure to pick a category for the article from the Wordpress sidebar. The category should match the category of similar articles previously posted, which can be checked inside Wordpress.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/cd19003d415841ccb99519de38c34199/wordpress-article-category.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>

### Save HTML version of article

Once the article is complete, copy the `html` text from the Wordpress `code editor`, create a file in the Ritza GitHub repository alongside the original article, and paste the text there. We keep this `html` version in case something corrupts the Wordpress version.

<video controls width="100%">
    <source src="https://i.ritzastatic.com/images/133019c06ad34297bdebcce53ae24565/html-save.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
