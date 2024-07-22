This is a template DREAM project site. You can start with this and modify it in any way you like, so long as it is still hosted in a git repository.

## Quick Start

### Step 1) Get a GitHub account

Go to github.com and sign up for a free account. Let's assume you sign up for an account with username "myname".

### Step 2) Copy this site to your GitHub account

Sign into your github account.

From this repo, click the "Fork" button at the top right hand of the window.
A copy of this repository will be made in your own github account.

### Step 3) Rename the repository

In "myname/dreamprojecttemplate", click on "Settings" near the top right hand of the window. Change the repository name from "dreamprojecttemplate" to to "myname.github.io". ("myname" must match your GitHub user name exactly.)

Scroll down til you see "GitHub pages" and choose "Master" instead of "None".

If you already have a GitHub site, then you can make this a project site rather than your personal site.

### Step 4) Customize and view your site

Set up your site name, description, avatar and many other options by editing the _config.yml file. 

To edit, click on the file link and then click on the little pencil icon in the top right. When you are done, scroll down and click "Commit".

To add your own image, do the following:
* upload your image into the "images" directory, by going to the "images" directory and clicking the "Upload File" button. Let's say you upload "yourimage.png". Don't forget to Commit!
* modify the avatar line in _config.yml to say "https://myname.github.io/images/yourimage.png". Don't forget to Commit!

Your site will typically be viewable within 5 minutes at <https://myname.github.io>.

Making a change to _config.yml (or any file in your repository) will force GitHub Pages to rebuild your site with jekyll. Your rebuilt site will be viewable within 5 minutes at <https://myname.github.io>.

> There are 3 different ways that you can make changes to your site:

> 1. Edit files within your repository in the browser at GitHub.com.
> 2. Use a third party GitHub content editor, like [Prose by Development Seed](http://prose.io). It's optimized for use with Jekyll making markdown editing, writing drafts, and uploading images really easy.
> 3. Clone down your repository and make updates locally, then push them to your GitHub repository. For more on how to "clone down", see [Github pointers](https://help.github.com/en/github/getting-started-with-github).

### Step 5) Publish your first blog post

Edit `/_posts/2020-06-01-week1.md` to publish your first blog post. This [Markdown Cheatsheet](http://www.jekyllnow.com/Markdown-Style-Guide/) might come in handy.

> You can add additional posts in the browser on GitHub.com too! Just hit the + icon in `/_posts/` to create new content. Just make sure to include the [front-matter](http://jekyllrb.com/docs/frontmatter/) block at the top of each new blog post and make sure the post's filename is in this format: year-month-day-title.md.

## Modify the Style

You can modify the look and feel of your site by modifying style.scss.

## Local Development

If you want to edit your website on your own computer rather than at GitHub.com, follow these instructions.

1. Install Jekyll and plug-ins in one fell swoop. `gem install github-pages` This mirrors the plug-ins used by GitHub Pages on your local machine including Jekyll, Sass, etc.
2. Clone down your fork: `git clone https://github.com/myname/myname.github.io.git`.
3. Serve the site locally on your computer: `jekyll serve`.
4. View your website at http://127.0.0.1:4000/.
5. Commit any changes and push everything to the master branch of your GitHub user repository: `git commit -m "message here"`; then `git push -u origin master`. GitHub Pages will then rebuild and serve your website publicly.

## Additional Tips and Help

- [GitHub pointers](https://help.github.com/en/github/getting-started-with-github)
- [GitHub pages](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site#creating-your-site)
- [Markdown](https://www.markdownguide.org/basic-syntax#links)
- [Jekyll](https://jekyllrb.com)
- [Jekyll tips](https://devhints.io/jekyll)

This site is based on [Jekyll Now](https://github.com/barryclark/jekyll-now).
