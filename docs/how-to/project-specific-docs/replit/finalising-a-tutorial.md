# Finalising Replit tutorials

Writers provide tutorials in different formats, both in terms of code and the write up. You need to convert them so that the write up exists as a branch of [our fork of their docs](https://github.com/ritza-co/replit.github.io/) and the code exists as a repl on our team account. All screenshots of progress showing the repl should be taken using this version so that the Replit user appears as "Ritza".

![](https://cln.sh/JjlIbW+) 

## Adding the example Replit embed

Add the example Replit embed at the *end* of the tutorial. In the team plan, the "share" button doesn't offer the HTML, but you can grab the latest version of the Embed code by clicking "Share" on a personal repl and then switching out the src URL to refer to the example (team) repl. This currently looks as follows but might be updated in the future.

```html
<iframe height="400px" width="100%" src="https://replit.com/@GarethDwyer1/WelltodoElatedLoops?lite=true" scrolling="no" frameborder="no" allowtransparency="true" allowfullscreen="true" sandbox="allow-forms allow-pointer-lock allow-popups allow-same-origin allow-scripts allow-modals"></iframe>
```

## Adding it to the sidebar
Add the tutorial to the appropriate place in sidebar.json as part of the pull request.



