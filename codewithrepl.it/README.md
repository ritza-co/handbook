# Updating the codewithrepl.it site and book

We have 

- https://codewithrepl.it - a site for people looking for coding projects and tutorials
- https://leanpub.com/coding-with-replit/overview - the tutorials in book form on LeanPub

The book chapters are slightly different from the articles - they refer to 'the next chapter' and 'the previous chapter' and gifs are replaced by screenshots where possible and linked to separately.

## Updating the website

* [here is a commit](https://github.com/ritza-co/code-with-replit-articles/commit/dd5c6d11bef5de8496b17ddca7efcaa7e6273ee0#diff-747a8f398395dde8e524d9f983784bd8441c5cfe4307b5a079be5412ee65c314) which shows adding a new article to the site. Cover images are created with Canva.

To add a new article, create a similar pull request to https://github.com/ritza-co/code-with-replit-articles (in the 'website' subdirectory). The site is manually deployed, so ping Gareth once you're done so he can push it live.

Note that we have been editing the .css and .html files directly instead of following the original NodeJS build process.

## Updating the book

Each article is also copied into https://github.com/ritza-co/code-with-replit-book/. These are *almost* the same as the online versions, but 

* We add a paragraph at the end of each chapter to introduce the next chapter
* Gifs are replaced by a single PNG and include a link for the reader to open the .gif if they are reading the book online. If the gif is not that important for following the tutorial, you can simply replace it with a .png and skip adding a link to the full gif 

![image](https://user-images.githubusercontent.com/2641205/114161514-73794100-9928-11eb-8555-eb14f731602f.png)

Merge the changes into the GitHub repository and then regenerate the book on LeanPub. Download the *unbranded* epub, mobi and pdfs and upload them to the Digital Ocean space.


