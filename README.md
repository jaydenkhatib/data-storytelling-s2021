Data Storytelling Course Blog
=============================

This lets you author simple stories in [Markdown](https://daringfireball.net/projects/markdown/syntax) and embed javascript and
other things that you cannot on other hosts like WordPress. Your posts will get automatically turned into HTML by the "Jekyll" engine.

## Writing a New Post

### If you *do* feel comfortable with GitHub

1. Fork this repository (you only need to do this once). This will create a copy of this repository in your GitHub account.
2. Use the web UI on GitHub.com to create a new file in the `_posts` folder (follow the file naming convention you see there).
3. Copy the `sample-story` into there and edit to with your story and the related embedded content.
4. Make sure to save ("commit") when you are done.
5. Create a "pull-request" via GitHub. This will let me know that you have some new content for me to pull in.

### If you do *not* feel comfortable with GitHub

1. Checkout the [sample post](_posts/2021-03-11-sample-story.markdown) in this repository.
2. Copy and paste that into a plain text file (or a Google Doc with no fonts or anything).
3. Edit your plain text file to format your post in Markdown and add in any custom HTML or Javascript.
4. Turn in your plain text file, or a link to it, and I will add it here so it will be automatically converted into a webpage.

## Technical Details

This uses [Jekyll](https://jekyllrb.com) to process your markdown and turn it into static HTML files. This makes it very cheap and easy to share on the web, because are no databases involved and no server code that needs to run in the cloud somewhere. That has made Jekyll very popular for cheap and easy distribution of HTML.

GitHub, now owned by Microsoft, is a major backbone of software development practices. They offer free hosting for HTML repositories via GitHub Pages, which we are using here to automatically run Jekyll to turn all the setup files and Markdown content into HTML pages (this happens automatically when new changes are made to the repository.)

### Run this on your own computer

Open up the terminal and do the following:

```
bundle install
jekyll serve
```
