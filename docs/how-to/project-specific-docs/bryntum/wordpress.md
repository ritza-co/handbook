# Cross-posting from GitHub to Bryntum Wordpress guide

The article should be copied from the GitHub by clicking and dragging over the article, rather than clicking on the `copy` button. This is because the `copy` button does not copy the text in markdown format, which we will need later on in the crossposting.

![Copy markdown](https://i.ritzastatic.com/images/dc9b9558164b4bf282dea79c07dd4737/copy-markdown.mp4)

Next the article can be pasted into the Wordpress visual editor.

![WP Visual editor](https://i.ritzastatic.com/images/de362045d5e74d97a231c888229e6524/visual-editor.png)

Here the editor will automatically format the markdown. Not all of the article will be formatted correctly and some adjustments may need to be made.

## Code block syntax highlighting

In the WP `visual editor`, run through the article and check the block type of all of the code snippets. Convert all code snippets to the `code` block type.

![Block type change](https://i.ritzastatic.com/images/e1847978414a4c069fc45e349c3b4997/block-type-change.mp4)

Swicth to the Wordpress `code editor` and run through all of the `<!-- wp:code -->` code blocks. Add the following class to both the `<pre>` and `<code>` tags of these blocks:

```html
class="language-(language-type-here)"
```

Ensure that the appropriate language is added to that class to ensure the code block has the correct syntax highlighting.

This can be made easier by copying the `html` version of the article from Wordpress, pasting into a text editor and using the find functionality (`cmd/ctrl+f`) to locate all of the `<!-- wp:code -->` blocks.

![Using text editor](https://i.ritzastatic.com/images/13cbe24f40c54c0cb60869778e525b8c/text-editor.mp4)

Each code block should be wrapped in a tag that looks something like this:

```html
<!-- wp:code -->
<pre
  class="language-javascript wp-block-code"
><code class="language-javascript">CODE-GOES-HERE</code></pre>
<!-- /wp:code -->
```

## Images

Go through the Wordpress block editor and delete the image blocks one by one and replace with the appropriate image for that section of the article.

![Image upload](https://i.ritzastatic.com/images/8da582080e4a495b90d61aac101560f9/image-upload.mp4)

All video or gif files must be converted to `webm` format. You can use [this website](https://cloudconvert.com/mp4-to-webm) to do the converting.

### Making the header image

To make the header image take the screenshot of the final software demo, or if the article is a comparison between two demos take the screenshots of both software demos, and place these images inside the Bryntum frame found in the Figma project.

![Figma header](https://i.ritzastatic.com/images/c54991ccdeee469782f4c7122dcbb750/figma-header-work.mp4)

Attach the header image in the cover image section.

![Header image](https://i.ritzastatic.com/images/06b95173e7454ba092148e177f96318e/header-image.mp4)

## Final checks

Once you have completed these steps, run through the article to make sure all the formatting has been copied over correctly. Check the headings, lists, bullet-points, images, etc.

Once the article is complete, copy the `html` tex from the Wordpress `code editor`, create a file in the Ritza GitHub repository alongside the original article, and paste the text there. We keep this `html` version in case something corrupts the Wordpress version.

![HTML save](https://i.ritzastatic.com/images/133019c06ad34297bdebcce53ae24565/html-save.mp4)