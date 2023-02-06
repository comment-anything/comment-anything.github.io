# Comment Anywhere Developer Website

The website is available at: https://comment-anything.github.io/

The Comment Anywhere project repo website was generated using Jekyll and the [Just The Docs theme](https://just-the-docs.github.io/just-the-docs/).


When we want to customize the theme, we should reference the [Github documentation](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll).


# How to Add a Post

You need to have [Ruby](https://www.ruby-lang.org/en/downloads/) installed to test the site locally. 

- clone your fork locally if you don't have it with `git clone https://github.com/your-name/comment-anything.github.io.git`.
- create a branch if necessary with `git branch yourname`
    - if you have a branch, go to it on GitHub and sync it with master
- checkout to your branch with `git checkout yourname`
- Make sure your branch is updated locally with `git pull`.
- Create a new markdown (*.md) file in the _posts folder. The name of the file should be `YYYY-MM-DD-title.md` where YYYY-MM-DD is the date and title is the name of the post.
- Add [YAML front matter](https://assemble.io/docs/YAML-front-matter.html) to the top of your .md file. It should include values for layout, author, and title. For example: 

```yaml
---
layout: post
author: karl
title: Weekly Presentation Report
---
```
- Create the post content. It uses standard [markdown formatting](https://www.markdownguide.org/cheat-sheet/). 
- Your post may need to link additional files or images. Add them in the appropriate subfolder of assets and link them like so:
```markdown
![my image alt text for accesibility]({{site.url}}/assets/images/My_New_Image.PNG)
```
- Similarily, you can add PDFs as links.
```markdown
[my new pdf]({{site.url}}/assets/pdfs/MyInterestingPdf.pdf)
```

- Test your post by running `bundle exec jekyll serve` to launch your page locally. Ensure good formatting and that the post is free from typos and errors, that all links work, and that all images load. If they do, it's time to push it to github.
- Run `git add *` to stage all the changes you have made.
- Run `git commit -m "message"` but replace message with a sentence summarizing the changes that were made.
- Run `git push` to push your commit to the fork. 
- Go to github, navigate to your forked repository, and open a pull request to merge your changes into the main branch.
- Karl will check the pull request and merge it if it is error-free.
