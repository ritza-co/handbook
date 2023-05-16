# Meta descritions

Metadescriptions are used by search engines like Google to show a summary of the article. e.g. 

![](https://i.ritzastatic.com/images/031c2f1ec4924b84a047991936b6cabd/example-meta.png).

Google doesn't always take exactly the metadescription that you give, but if the meta description is good, then Google is more likely to use it.

## Good meta descriptions

* Always < 160 characters 
* Should give the reader as much value as possible from the
* Not click-baity or trying to make the read the article - if you can give them everythign they want just from the metadescription then that is fine.
* Don't use phrases like "read on for more" etc. You only have two sentences - try to give the reader the main takeaway of the article. 

## How to set metadescriptions

In editors like Wordpress and Medium, the meta description is often set up automatically with automatic summarization of the article draft. It's still good to manually write your own one rather.

In HTML, you use the `<metadescription>` tag in the `<head>` section.

In many static site generators, you use YAML front-matter, e.g

```
---
title: This is my article
description: This is an article about foo bar baz
---
```

But this will depend on exactly which [Static Site Generator (SSG)](../ssgs) you are using.



