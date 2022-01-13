# Creating Leanpub Books

The following is a guide on how to create a book in pdf, mobi and epub format on Leanpub. 

## Getting Started

First create a GitHub repository which will house the markdown content for your book. In the root folder of the repository, create a `manuscript` folder to contain the `md` files for the chapters your book will have. 

## Adding Book Chapters

Each book chapter will have its own `md` file. When naming the `md` files, start with a number that denotes the chapter number followed by the chapter title for example, the `md` file for the first chapter might be named `1-first-chapter-title.md`. 

## Adding Images

To render images you can add them to the repository and link to them relatively in the `md` files or you can provide an absolute url to where they are hosted on the internet. 

### Adding Local Images  

Create a `resources` folder inside the `manuscript` folder and add the images there. The names of the images should start with a number denoting for which chapter they are for followed by what the image depicts. For example, an image showing a login form for the first chapter might be named `1-login-form.png`. Use the syntax below to link to it in the `md` file:

```md
![Login form](1-login-form.png)
```

### Adding External Images 

To render an image that's hosted elsewhere on the internet, use the syntax below:

```md
![Login form](absolute-url-to-where-image-is-hosted)
```

## Dealing with Gifs 

Leanpub can't render gifs in pdfs so to get around this, take a screenshot of the most important frame in the gif and add it to the `resources` folder in the repository. Link to the screenshot image in place of where the gif was and provide a link to open the gif below the image like so:

```md
![Login process](1-login-process-important-frame.png)
[*click to open gif*](absolute-url-to-where-gif-is-hosted)
```

## Add a `Book.txt` File

When you have finished adding the `md` files for the book chapters the last step will be to create a file named `Book.txt` inside the `manuscript` folder. This file tells Leanpub how to compile your book and in which order to arrange the chapters. List the file names of the `md` files starting with the first and ending with the last like so:

```txt
1-first-chapter-title.md
2-second-chapter-title.md
.
.
.
10-tenth-chapter-title.md
```

## Create Unbranded Exports on LeanPub

After actioning the above steps Leanpub will now be able to generate exports for your book. Generate *unbranded* epub, mobi and pdf versions of your book and upload them to the Digital Ocean Space with the permissions set to publicly readable.