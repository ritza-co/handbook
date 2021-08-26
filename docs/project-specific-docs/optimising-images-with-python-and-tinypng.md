# Auto optimize images in < 100 lines of code

Sometimes you want to reduce the size of all the images in a directory to fit into a fixed limit. For example, if you have a blog post and some linked images:

```
blog/
    my-awesome-post.md
    images/
        first-image.png (2 MB)
        second-image.png (500 KB)
```

You might want each image to be 

* As good quality as possible
* No more than 100 KB per image

This is a classic tradeoff - you want low cost (size) but high quality, so if the image is too big, you want to reduce it to around 100 KB.

## The two step process

The nicest way to reduce the file size of PNGs is to 