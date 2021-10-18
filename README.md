# Whitney Young Robotics Website

Welcome to the source of https://www.wyrobotics.org, our website for the Robotics Club at Whitney Young and its two FTC Teams:
- 3216 Robophins
- 15659 Young Droids

This website is built with [Hugo](https://gohugo.io) and uses the [Wowchemy](https://wowchemy.com) template manager. It's also deployed on [Netlify](https://www.netlify.com).

The website was created as a rework of the old Google sites website at https://sites.google.com/view/wyrobotics/. Under the impression that it wasn't optimal for customizing and inserting blog posts, it was decided that we recreated the website without a UI-based website builder. 

## For Members

Here's a rundown on how the website is organized and how to insert your blog posts appropriately.
Folders and files that are self-explanatory or not necessary to be understood will be left out.
The most important directories for adding blog posts have been **bolded**.


📁 archetypes - includes templates for pages -- don't worry about it

📁 assets
- 📁 media - media used in front matter or config
    - 📁 cover-img - images used as the cover of pages

📁 config - website config
- 📁 _default
  - 📄 config.yaml - main website config
  - 📄 menus.yaml - edit the navigation bar
  - 📄 params.yaml - personalize the site

📁 content
- 📁 authors - user profiles
  - 📁 `someone`
    - 📄 _index.md - your user profile
    - 📄 avatar.jpg - photo of yourself or delete to not show any photo
- 📁 home - the homepage
- 📁 about - the about page
- 📁 gallery - the gallery page
- 📁 info - the for team members page
- 📁 **post - list of blog posts**
  - 📁 robophins 
    - 📄 `post-date-1`.md
    - 📄 `post-date-2`.md
    - 📄 _index.md - an archive of blog posts for Robophins
  - 📁 young-droids
    - 📄 `post-date-1`.md 
    - 📄 `post-date-2`.md
    - 📄 _index.md - an archive of blog posts for Young Droids

📁 data - font and theme info

📁 layouts - edits to the default template theme

📁 static - files that won't change
- 📁 img - static image files
  - 📁 gallery - photos included in our Gallery page of the website
  - 📁 home - photos used on the homepage
  - 📁 **posts - photos used in blog posts**
    - 📁 `date` - contains photos used in that day's journal entry
    - 📁 unsorted - temporary place for photos to live

### Creating Blog Posts

Use markdown to write all journal entries. For a brief overview of what you can do, please refer to this [article](https://wowchemy.com/docs/content/writing-markdown-latex/).

Use the template at [content/post/template.md](content/post/template.md) to start writing a blog.

There are two main sections: the front matter and the body

The front matter is anything between the set of `---` and it includes all metadata that is used for your post.

The body is anything after the front matter and can include markdown text, html, images, LaTeX and other features.

### Adding Blog Posts

[Commit](https://github.com/git-guides/git-commit) and [push](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository) your post to the `drafts` branch of the [GitHub repository](https://github.com/texguy360/wyrobotics).

Then submit a [pull request](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) to merge your post to the `main` branch, which is the branch that is deployed.

Please refer to this [Git article](https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository) to learn more on the basics of using git.