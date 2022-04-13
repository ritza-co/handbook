# Updating MakeJSGames.com

Our [makejsgames.com](https://makejsgames.com) site consists of several pieces.

* Each article, which lives on [docs.replit.com](https://docs.replit.com)
* The website, which links to the individual articles.
* The ebook, which has its own GitHub repository and is built using LeanPub.

This explains how to update each component.

## Updating the book

To add a new chapter:

1. Copy the markdown content from the version in the [GitHub docs repository](https://github.com/replit/replit.github.io)
2. Create a new markdown file in the `manuscript` folder of the [Book's GitHub Repository](https://github.com/ritza-co/make-javascript-games-book), following the naming convention of the other chapters, and add the markdown copied in step 1.
3. Fix the images. You need to add the full URL to the path on the Replit docs. See the existing chapters for exmaples.
4. Replace any gifs or mp4s (animated images) with a single frame png file. See [How to extract PNGs from GIF or MP4](../../how-to/how-to-extract-pngs-from-gif-or-mp4).
5. Add the pngs to the `resources` folder and reference them in the Markdown file using a relative reference (see the existing chapters for examples).
6. Add a footnote and a link to the gif/mp4 file online (see the existing chapters for examples)
7. Open a pull request to the GitHub repository.
8. Send a message in #ritza-replit on Slack to indicate you've done it.

