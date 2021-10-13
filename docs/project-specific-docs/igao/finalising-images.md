# Finalising images

Before sending the images we should optimize them to try get them close to 100KB. For the internal images (not the CS), we also need to manually set the dimensions.

## Using imagemagick to set the dimensions

They want the images to be 3200, so with [ImageMagick](https://imagemagick.org/index.php) you can use the following command.

```
convert -resize 3200x Maps-02.png Maps-02.png
```

Note:

* The `convert` command is part of ImageMagick - not sure how easy this is to set up on Windows
* The `3200x` width specifies one dimension and then the other is set automatically to maintain the aspect ratio
* By passing in the same file name twice, we overwrite our original file - be careful!

This only needs to be done for the internal images, not the cheatsheet.

## Optimizing the images

Once it's resized, you can go to [tinypng](https://tinypng.com) and upload all the images (including the cheatsheet). This reduces the colour variation to optimize the file size without further reducing the dimensions.

## Adding the images to the Google doc

Finally, delete any sketches in the Google doc and replace them with the optimized designed images. Also delete the cheatsheet table, and replace it with the optimized cheatsheet.

Then share all of the images and link to the doc on Slack so Gareth or Sarah can send off.




