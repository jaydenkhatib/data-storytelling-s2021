Data Storytelling Course Blog
=============================

This lets you author simple stories in [Markdown](https://daringfireball.net/projects/markdown/syntax) and embed javascript and
other things that you cannot on other hosts like WordPress. Your posts will get automatically turned into HTML by the "Jekyll" engine.

## Writing a New Post

1. Fork this repository (you only need to do this once). This will create a copy of this repository in your GitHub account.
2. Use the web UI on GitHub.com to create a new file in the `_posts` folder (follow the file naming convention you see there).
3. Copy the `sample-story` into there and edit to with your story and the related embedded content.
4. Make sure to save ("commit") when you are done.
5. Create a "pull-request" via GitHub. This will let me know that you have some new content for me to pull in.

## Technical Details

This uses Jekyll to process your markdown and turn it into static HTML files. This makes it very cheap and easy to share on the web, because are no databases involved and no server code that needs to run in the cloud somewhere.

### Run this on your own computer

Open up the terminal and do the following:

```
bundle install
jekyll serve
```
