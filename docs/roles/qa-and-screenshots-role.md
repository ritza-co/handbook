# The Quality Assurance role and high res screenshots

All Ritza tutorials should 

* Be easy to follow - each step should be correct and clear
* Have high quality graphics - screenshots should be taken on a retina or 4k monitor

As each of these steps requires a full "run through" the tutorial, they are often done together. The QA engineer should place themselves 'in the reader's shoes'
and work through the tutorial from start to end, making sure that each step is clear, unambiguous, and correct. As they go, the QA engineer also re-takes any 
screenshots that are not high resolution, and adds screenshots for clarity if required. This usually includes adding a screenshot to the introduction section to 
demonstrate what the app or project will look like once the reader has finished working through the tutorial.

We use CleanShotX for all of our screenshots. Ask for a license key if you do not have one.

## Making changes

The QA engineer should submit several pull requests, depending on what is needed.

* One pull request to include a version of the author's tutorial and code **exactly as they provided it**. This step can be skipped if the author already made a pull request to the correct place, but often the author works in a different format or on their own GitHub. This should be in a branch called something like `add-first-draft-chat-bot-tutorial`. This is exactly the author's work.
* A second pull request for text and/or code changes. If anything isn't clear or the QA engineer finds something confusing, they should submit suggested changes, as a separate pull request (to the version in our GitHub, not to the author's original version. If necessary, they can ask clarifying questions to the author, but in general they should aim to use their judgement so we can keep moving forwards without reverting back to the author.
* A third pull request to add and update the images.

## Adding captions and alt text

All screenshots should have relevant alt text that can help with accessibility - e.g. blind people have these read to them by screenreaders. In markdown, alt-text 
can be added within the first set of (square) brackets `![A graph showing that x increases as y decreases](/path/to/image.png)`

## Choosing the correct cropping

Showing how much context to show is important. Many people will simply screenshot the entire screen. It is better to crop the screenshot as much as possible, 
showing only the relevant panel or section of an interface **but** making sure it is clear what the context is. The user needs to be able to find the section in 
the screenshot - if it might be difficult, rather include more context for the reader to orientate.

## Annotations

We use numbers, arrows, and rectangles to call the readers attention to specific areas of a screenshot. In some cases, a short amount of text (preferably one word) 
can be added, but this is generally undesirable. Rather keep any text to captions or paragraphs above/below the image.

## Gifs
Sometimes it's clearer to show something in a gif than in a static image. Gifs should in general be 2-5 seconds long (any longer and the reader is annoyed by 
having to wait for it to start again if they miss the start).
