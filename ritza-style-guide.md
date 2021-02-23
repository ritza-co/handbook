# The Ritza style guide

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

## Default to active voice

Today's readers often scan a page instead of reading it. Aim to use active voice rather than passive, as it means the reader can pick up more info from a quick scan over the content. 

* ⚠️ The command will be run by the shell.
* ✅ Use the shell to run any commands.

## Link as much context as useful

Choosing what text to link out to an additional resource is more an art than a science. The main rule is that it should be as clear as possible to the reader
what is being linked to

* ❌ You can follow the widget [guide](#) to learn more
* ✅ You can follow the [widget guide](#) to learn more

In the first example, the link could be to a Wikipedia article explaining what a guide is. The second makes it clear that it is a link to the guide that was mentioned.

## Avoid telling the reader that something is obvious or easy

Different people find different things difficult. Avoid telling the reader that something should be 'easy', 'obvious' or 'simple'. In the worst case, they find it hard and find it discouraging. In the best case, they do find it easy and they don't gain anything by you telling them that it was easy.

Mostly, `~it's simple~`. you can `~easily~` `~just~` remove the offending words and the sentence keeps its meaning.

* ❌ Obviously, you can terminate the program at any time by hitting `Ctrl+C`
* ✅ You can terminate the program at any time by hitting `Ctrl+C`

Sometimes, you need to reword to avoid implying that something is simple

* ❌ It's easy to add new widgets using Acme's tool. Click `menu` -> `add widget`.
* ✅ To add a new widget using Acme's tool, click `menu` -> `add widget`.

## Structures should be as flat as possible

Articles should using heading 1 (`#` in Markdown) for the title and heading 2 (`##`) to break things down into logical sections. Heading 3 (`###`) can be used where necessary for sub-sections, but in general having a deeply nested structure makes things harder to follow, harder to edit, and harder to reuse. As a writer, your job is to take a complicated graph of interconnected ideas and break them down into a linear structure that can be read from start to end.

You can do this partially (with many nested substructures), which helps readers but still requires them to put in effort, or you can break things down even more cleanly into a single line (harder for the writer, easier for the reader)

![distilling information](https://i.ritzastatic.com/images/6ac86cae2c3a46bcbfcdf5db66d6b0c7/distilling-information.png)


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




