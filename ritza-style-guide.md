# The Ritza style guide

![](https://i.ritzastatic.com/images/8669ccb26a744f6489d31fb26d6aecb7/writingablog.png)

We have produced hundreds of technical tutorials, articles, and other educational materials. Our goal is always to *teach*. 
This often means helping our readers explain complicated technology, either conceptually or by example.

This is our opinionated style guide. Following it will help you produce work that is valuable and easy to understand.

## Use an appropriate voice and mood

Default to *first person plural* to include the reader in your 'team'

When explaining how to do something, use first person plural (we/us). This means you the author, and the reader. You are doing something together. 

✅ "Next, we'll install the widget factory to create widgets efficiently."

Sometimes it's more efficient to use the imperative mood and "instruct" the reader by telling them what needs to be done. 
This is harsher but often less wordy, so use your judgement

* ⚠️ "We can do this by using our package manager. We'll acheive this by typing `sudo apt-install widget-factory`"
* ✅ "We can do this by using our package manager. Type `sudo apt-install widget-factory`"

As a non-fiction writer, we never want to get in the reader's way - they are not interested in us as people

* ❌ "I wrote this guide after encountering difficulties with the software myself"
* ❌ "Next, I'm going to show you how to install a widget factory"

It's ok to refer to the reader as 'you' in some cases, where the writer is clearly not involved, but in general, default to the 'we' voice wherever possible.

* ⚠️ "As you might remember from the [previous tutorial](#), widget factories create widgets. In this tutorial..."
* ✅ "In the previous tutorial, we saw how widget factories create widgets. In this tutorial..."

## Avoid anything you might find in an encyclopaedia or academic paper

Most people have been taught to write "wrong" at school. You should watch [this video](https://www.youtube.com/watch?v=vtIzMaLkCaM) if you have time, but in short

Don't use anything that you might find at the start of a Wikipedia article or a dictionary. Your reader isn't interested in definitions - or if they are they can easily find these elsewhere. 

If you're writing an article on NER, instead of starting with

❌ "Named Entity Recognition (NER) is the task of categorising key words in a text as specific entities."

Consider something more like 

✅ "If you're analyzing a large amount of text, it's often useful to extract named entities from this - identifying people, places, dates and other entities."

If you've ever tried to learn a new concept, you probably already know that reading a definition doesn't really clarify - but a more specific exmaple does.

## Avoid guessing out loud what the reader wants

It's tempting to start an article with "Are you are a foo who likes to bar but sometimes finds baz?", but in most cases these define a much narrower audience than the actual audience, and you risk alienating anyone who does not fit that identify (and they might stop reading after the first setence, even if the article would have helped them).

## Don't give extraneous context

Often it's tempting to try and give the reader some related context or information. Generally avoid this. The reader isn't here to learn about knowledge in general, but usually on how to achieve a more specific goal.

Instead of

❌ Label Studio is an open source data labeling tool for labeling and exploring multiple types of data. Label Studio can be integrated with machine learning models to supply predictions for labels (pre-labels), or perform continuous active learning. You can use LabelStudio for a variety of labelling and classification tasks for many different data formats but again we will just be focusing on its NER capabilities.

Try something more concise:

✅ We can use Label Studio for manually tagging Named Entities in our dataset. Install it now with `pip install label-studio` if you haven't already.

## Default to active voice

This is often taken as a hard-and-fast rule. It isn't. In many cases, active voice makes it clearer who is doing what and sounds less stuffy. That said, sometimes passive is simply cleaner (often in cases where there isn't a specific subject) - use your judgement.

* ⚠️ The command will be run by the shell.
* ✅ Use the shell to run any commands.

## Avoid telling the reader that something is obvious or easy

Different people find different things difficult. Avoid telling the reader that something should be 'easy', 'obvious' or 'simple'. In the worst case, they find it hard and find it discouraging. In the best case, they do find it easy and they don't gain anything by you telling them that it was easy.

Mostly, `~it's simple~`. You can `~easily~` `~just~` remove the offending words and the sentence keeps its meaning.

* ❌ Obviously, you can terminate the program at any time by hitting `Ctrl+C`
* ✅ You can terminate the program at any time by hitting `Ctrl+C`

Sometimes, you need to reword to avoid implying that something is simple

* ❌ It's easy to add new widgets using Acme's tool. Click `menu` -> `add widget`.
* ✅ To add a new widget using Acme's tool, click `menu` -> `add widget`.

## Structures should be as flat as possible

Articles should using heading 1 (`#` in Markdown) for the title and heading 2 (`##`) to break things down into logical sections. Heading 3 (`###`) can be used where necessary for sub-sections, but in general having a deeply nested structure makes things harder to follow, harder to edit, and harder to reuse. As a writer, your job is to take a complicated graph of interconnected ideas and break them down into a linear structure that can be read from start to end.

You can do this partially (with many nested substructures), which helps readers but still requires them to put in effort, or you can break things down even more cleanly into a single line (harder for the writer, easier for the reader)

![distilling information](/img/distillinginfo.png)


## Avoid nested bullets

❌ Don't nest bullets into several levels

You have several options for adding widgets

* From the menu
    * by clicking on `file` -> `add widget`
    * by clicking on `help` searching for `add widget` and hitting `enter`
* With a keyboard shortcut
    * by pressing `a` and then `w` in command mode
    * by pressing `ctrl + a`

✅ Rather restructure to use separate bullet lists

You can add widgets from the menu
* by clicking on `file` -> `add widget`
* by clicking on `help` searching for `add widget` and hitting `enter`

or with a keyboard shortcut
* by pressing `a` and then `w` in command mode
* by pressing `ctrl + a`

## Avoid 'marketing' speak

Never try to sell something to the reader. Don't say a product makes things easy, that a design is beautiful, or use any text that you might find on a SaaS landing page.

## Link as Much Context as is Useful

Choosing what text to link out to an additional resource is more an art than a science. The main rule is that it should be as clear as possible to the reader what is being linked to, but keep it simple. 

* ❌ "[You can follow the widget guide](#) to learn more"
* ❌ "You can follow the widget [guide](#) to learn more"
* ✅ "You can follow the [widget guide](#) to learn more"

The first example links too much unnecessary wording. In the second example, the link could be to a Wikipedia article explaining what a guide is. The third makes it clear that it is a link to the guide that was mentioned.

## Don't Assume Knowledge

This can be tricky because, of course, you always have to assume _some_ level of knowledge when writing technical content. However, we try avoid assumptions about our reader's skill level. 

* ❌ "Referring back to the server code, it's obvious that we need both a success.html and a cancel.html."
* ✅ "Referring back to the server code, you may notice it requires both a success.html and a cancel.html."

## Include User-friendly Code Samples

We want to tell the reader exactly _what_ code needs to go _where_, and make it easy to repeat what we are doing. Avoid screenshots of code, and rather present code samples in text, between backtick gates with a language description.

**Avoid long code snippets**
Instead of giving an entire file to copy-paste, break down the code into several steps if possible.

**Provide a file, if you must**
If there's a lot of ‘boilerplate’ code, consider providing the file in a repl and instruct the reader to copy the whole thing as a starting point. However, it's preferable to avoid this if you can.

## Annotate screenshots and use context
Screenshots are super helpful tools for tutorials, but using them too often or without clarity may just make it harder for the reader to follow your instructions. 
 
* ✅ Use contextual screenshots to help readers navigate whichever platform you are directing them to.
* ✅ Use a screenshot to demonstrate what your reader should be seeing if they correctly followed your instructions. 
* ✅ Make use of [1], [2], [3] annotations if several things need to be shown from a single shot.
* ✅ Preferably take screenshots using a 4k/retina screen, or consider using a virtual high-res screen through Chrome dev tools as an alternative.
* ✅ For Mac, use CleanShotX if possible

* ❌ Avoid screenshots of large amounts of text. Rather use a caption if you need to present text to your reader. 
* ❌ Avoid screenshots that show too little; for example, just the button they must click. Where is this button in relation to the page? 
* ❌ At the same time, don't include so much in the screenshot that the reader isn't sure what you are trying to illustrate.

## Prefer code blocks to inline code

It's ok to use markdown's single back-tick syntax to highlight a single word like "Notice the `for` statement below". For any code samples, even if only one line, rather use three backticks and have the code on its own line and in its own section.

❌ Now run `python3 app.py`

✅ Now run:

````
```
python3 app.py
```
````



