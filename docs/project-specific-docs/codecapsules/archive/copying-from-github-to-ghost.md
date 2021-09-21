# Copying from GitHub to Ghost

All of our content lives primarily in GitHub. This is important so that we can track changes and keep it up to date.

However, some of our customers use Ghost as a CMS, which does not have an easy integration with markdown on GitHub.

Therefore, we have to manually copy across content from GitHub to Ghost. 

Any changes made need to be updated in GitHub and then transferred to Ghost so that GitHub always has the main and most updated copy.

## Copying procedure

The Ghost editor handles formatting quite well. You can preview the markdown file in GitHub (not 'raw' mode), select all the content, and copy it to Ghost.

The things that break are

- Code samples - for each code sample, you need to type three backticks into the Ghost editor and press `Enter`. This will create a Code block and then you can enter the language in the prompt to get the correct highlighting. See the gif at https://cln.sh/jNSIC2.
- Links - some links are prefixed with https://github.com... and then the final version is broken.


