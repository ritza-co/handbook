# Writing a draft

You've likely been given the task of writing the draft of a technical article. Here are some general guidelines that you should follow. This is generic advice - if you are working on a project with more specific requirements around file formats, project structure, or anything else, then use that instead.

## Use markdown and GitHub

Your draft should be a single markdown file. Any images should be in a subdirectory and relatively linked.

Your file structure will probably look something similar to the following.

```
building-foo-bars-with-a-baz.md
img/
    installing-foo.png
    configuring-bar.png
    ...
```

## Follow our style guide

[Ritza's writing rules](https://styleguide.ritza.co/ritza%27s-writing-rules/Style/) give some general points for your writing to follow. If it's your first article, you don't need to hit every one of these points, but at least read through them before you begin and see which ones you can get right from the start, as this saves us a lot of editing time.

## Screenshots

Screenshots will usually be redone during the quality assurance stage, so you do not need to worry about every detail described in our [screenshots guide](https://styleguide.ritza.co/screenshots/screenshot-guidelines-for-technical-documentation/). However your screenshots should still follow at least these points.

* Use a descriptive name for each screenshot, e.g. `installing-foo.png`, not `screenshot-1.png`
* Name the files in slug form with no spaces, not `Installing Foo.png`. 
* Avoid special characters in screenshot names, not `installing-foo(1).png`
* Make sure the screenshot is high quality enough to be legible.
* Add annotations if you want them. They will be reannotated during QA, but it helps QA follow along if you have added at least some rough annotations.
* Do not include too many screenshots. It's a balance between too few and too many, but think about the reader. If something is obvious, it does not need to be shown graphically. For example, if you are describing a process that has 20 steps, you migh want to include screens of the four most complicated ones.

## Code samples

Use code blocks in three backticks and the language name as described [here](https://styleguide.ritza.co/ritza%27s-writing-rules/Style/#prefer-code-blocks-to-inline-code).

## Check your own work

Although we do QA and editing on all drafts, you should do your own run through and read through before submitting a d raft for QA and Editing. QA and Editing are meant to be a second pair of eyes, not a function to transform unfinished work into the final product.

However you should still ask for early feedback from QA and Editing, as early and as often as possbile, especially if it's your first article. This can help correct misconceptions early in the process and avoid you needing to do rework after submitting a final draft.

