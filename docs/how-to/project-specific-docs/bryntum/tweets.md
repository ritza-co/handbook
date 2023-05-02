# Bryntum tweets guide

Every week, early in the week, we need 7 tweets complete in the [`External doc`](https://docs.google.com/document/d/1EnolV69AqvR76GA9kTwmSCGjPgKnl-lIPrj8E7aHm0M/edit#), ready to be posted for the following week.

Every week needs:

- 4 tweets about Bryntum products (Mon, Wed, Sat, Sun)
- 1 tweet about an interesting story in tech preferably webdev news (Tues)
- 1 tweet with a codepen demonstrating something cool or useful for the frontend (Thurs)
- 1 Fun Friday tweet with meme (Fri)

## Bryntum Product tweets

Every week we right four tweets about the features of these six Bryntum products:

- Gantt - https://bryntum.com/products/gantt/examples/
- Calendar - https://bryntum.com/products/calendar/examples/
- TaskBoard - https://bryntum.com/products/taskboard/examples/
- Scheduler- https://bryntum.com/products/scheduler/examples/
- Scheduler Pro - https://bryntum.com/products/schedulerpro/examples/
- Grid - https://bryntum.com/products/grid/examples/

Each tweet needs:

- A description of a Bryntum Products feature, with some emojis
- A link to the described Bryntum product feature (see the links above)
- A 16:9 video demonstrating the use of that feature, recorded in the Bryntum banner maker
- These hashtags: #react #vue #angular #js

Here is an example tweet (please note the header is not included in the tweet):

```
# TaskBoard Columns demo
📚🔀 Manage your team's workflow like a pro with Bryntum's TaskBoard Columns feature! Discover how easy it is to manipulate columns and customize your project's layout.

Demo link below ⬇️
https://bryntum.com/products/taskboard/examples/columns/

[IMAGE](https://i.ritzastatic.com/images/9a37b36dbcaf4261928f3b3afb49b0c3/tb-col.mp4)
#react #vue #angular #js
```

All Bryntum product tweets should follow this format. Please make sure to use a descriptive header for the tweet so that you will be able to easily search the tweets document and find out if you have tweeted about this feature before.

Each product should be tweeted about evenly, ensuring not to tweet about the same product twice in the same week, and ensuring, if possible, that you have not tweeted about any product feature before.

### Recording in 16:9 aspect ratio with CleanShot

Every video uploaded for a tweet must be recorded in a 16:9 aspect ratio. To do this in the CleanShot application, open the application and select `Record Screen`:

![Record Screen](https://i.ritzastatic.com/images/9c2999e18a8847c9b562a38babea74e0/rec-screen.png)

Once the record screen menu is open you will see the aspect ratio symbol, click that symbol and choose the 16:9 aspect ratio setting:

![Choose aspect ratio](https://i.ritzastatic.com/images/f2bf1c20edcd4c6c838dfd8b3d80e02d/sixteen-nine.png)

Then align this recording area over the area you wish to record.

### Recording with the banner maker

The banner maker software, found [here](), needs some setup before use.

- The `Show bryntum logo` option should be selected
- The appropriate demo title should be put into the `Title` option (e.g. TaskBoard Columns demo)
- The `Framework` option should be set to `Javascript`
- The `Size` option should be set to `LinkedIn 1200x675`

![Banner maker settings](https://i.ritzastatic.com/images/2f261694531241d397c8992fc1b45c1a/banner-maker-settings.mp4)

The people at Bryntum are proud of their product and so they them to be shown in their best possible form. However, the banner maker software provided does not always do a good job of displaying the Bryntum products.

Sometimes it is enough to put the link to the demo (e.g. https://bryntum.com/products/taskboard/examples/columns/) in the `iframe` found by enetering the developer tools with (`command + option + i`).

![Open banner maker dev tools](https://i.ritzastatic.com/images/5732f1a545ce4d9085824b579e2fe750/banner-dev.mp4)

Then you can demonstrate using the product while recording the banner at 16:9 aspect ratio.

![Record the product feature](https://i.ritzastatic.com/images/0c146a9114aa4cfab271dea586e02c3c/record-feature.mp4)

But sometimes the UI can be squished by the banner maker, making the product look bad. As you can see in the video above, The TaskBoard's tasks are squished and so you cannot read the text within them. Keep an eye out for this.

If the UI is squished, just adjust the font size % in the settings of the banner-maker until the UI looks good:

![Adjust font size](https://i.ritzastatic.com/images/d71217c8fcbd43a488a6b9d121b0f25e/font-size-zoom.mp4)

## Codepen tweets

The codepen tweets also need to link to the codepen and have a recording of the codepen being used along side some of the code. This video must be recorded in the browser at 16:9 as well.

Here is an example tweet (Again, the heading is not a part of the tweet):

```
# Colorful Button Animations Pen

Brighten up your website with these vibrant button animations in multiple colors! 🌈✨ Add some zest to your user experience with these eye-catching designs.

Demo link below ⬇️
https://codepen.io/bryntum-snippets/pen/NWOKqqm?editors=1100

[IMAGE](https://i.ritzastatic.com/images/5a173b2cd5664781b458a80aedf00576/but-pen.mp4)
#html #css #ux
```

All videos and images must be run through the `upload.py` script, the link returned from that script is then used to link to an online version of the image in the [`External doc`](https://docs.google.com/document/d/1EnolV69AqvR76GA9kTwmSCGjPgKnl-lIPrj8E7aHm0M/edit#).

Make sure to have these tweets ready early in the week before they will be tweeted, in order to allow for proofreading, checks, and adjustments.

## Tech News of the week tweets

Once a week we tweet about an interesting tech news story. The story should be related to frontend dev in some way.

Here is an example tweet:

```
# News 📰

Visual Studio Code 1.77 introduces a preview of deeper GitHub Copilot integration, offering inline suggestions and chat capabilities for an all-new coding experience. 🛠️💬

Read more here:
https://www.infoworld.com/article/3692530/visual-studio-code-177-previews-github-copilot-chat.html

#VisualStudioCode #GitHubCopilot #coding
```

## Fun Friday tweets

On fridays we tweet a meme along with a short reaction, either some text and emojis or just emojis.

The memes are usually sourced from [Reddit](https://www.reddit.com/r/ProgrammerHumor/) but of course you can source them from other places.

Please make sure the meme is high quality, that you have multiple choices for the people at Bryntum to choose from, and that you have not used the same meme in the past.

Here is an example tweet:

```
# Fun Friday

🤣🤣

[IMAGE](https://i.ritzastatic.com/images/aa87382a6c384e90a7eaa15a81f32916/wot.jpg)
```
