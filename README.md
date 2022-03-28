# Adie Hub

An Adie-organized space for sharing resources across adie cohorts.

Check out the [repo on github](https://github.com/adie-hub/adie-hub.github.io), or [go to the site itself](https://adie-hub.github.io/).

## Contributing to the Adie Hub

We are using [Hugo](https://gohugo.io/) to build the site. This means all of the content lives in simple markdown files under the [content/post](https://github.com/adie-hub/adie-hub.github.io/tree/main/content/post) folder!

If you just want to correct a typo or add something small to an already existing page, you can skip steps 1, 3, and 4.

If you want to add a new page, please follow the steps below:

### 1. Install Hugo

If you are on a mac, the easiest way to install hugo is through homebrew:

```sh
brew install hugo
```

Otherwise, checkout [Hugo's install documentation](https://gohugo.io/getting-started/installing/).

### 2. Fork and clone the repository

Fork this repository to your own github account, then clone it to your local machine with:

```sh
git clone --recurse-submodules https://github.com/<YOUR_USERNAME_HERE>/adie-hub.github.io.git
```

Open it up in your favorite text editor (VS Code works great!).

### 3. Create a new page

Making a new page is very simple. Navigate to the repository in your terminal and run:

```sh
hugo new post/my-new-post.md
```

Replace "my-new-post" with the name of the page you want to create.

This should create a file at `content/post/my-new-post.md`. Open that file up in your text editor. It should like something like this:

```yaml
---
title: "My New Post"
date: 2022-03-03T18:21:19-08:00
draft: true
toc: true
tags:
  -
---
```

This is some metadata that will help Hugo build the page correctly. The title will be set automatically based on the name of the file, and the date will also be created automatically.

`toc: true` will add a table of contents to your post. If your post does not need a table of contents, you can change this value to `false`.

Make sure to add the tag(s) that are relevant. See [Tags](#Tags) below for examples.

Now you can write out the content you would like the page to have! If you don't know markdown, check out this [cheatsheet](https://commonmark.org/help/) to get started.
The theme we are using has some additional options; if you would like to use those, you can see examples of what they look like and how to use them on the theme's [demo site](https://cupper-hugo-theme.netlify.app/cupper-shortcodes/).

### 4. Test your changes

You can test the changes to see what they will look like by running:

```sh
hugo server -D
```

from the root of the repository on your computer. Then, you can open `localhost:1313` in your browser to see the site. You should be able to navigate to your page with the "All Pages" button or the "tags" button if you set tags up.

### 5. Submit a pull request

Once you are happy with your changes, go back to the yaml metadata and change `draft: true` to false. If you do not do this, your page will not be created by hugo when you submit it.

Then you can commit your changes and push them up to your repository. Then you can submit a pull request for review!

## Tags

You can add one or more tags to a page to denote what it relates to.
Suggested tags include:

- C16 (or C17, C18, etc)
  - use this to denote that information is applicable to a specific cohort
- internship
- general

You aren't limited to only these tags. Check the tags page of the site for more possible ideas, but feel free to come up with your own. However, if there is a tag that already means something very similar to your new idea, please use the pre-existing tag.

To set tags in the post, just add them to the list at the top of your page. For example, a page that has the C16 and internship tags would look like this at the top:

```yaml
---
title: "My New Post"
date: 2022-03-03T18:21:19-08:00
draft: true
toc: true
tags:
  - C16
  - internship
---
```

## Questions

If you have any questions, please feel free to reach out in one of these ways:

1. Join the [discord server](https://discord.gg/U8qBJXn2GM)
   - Current students and alumni, please direct your questions to the #ada-hub channel.
   - Alternatively, you can reach out directly to Jesse (discord username: jesse (they/them)#2656) or Lux (discord username: knox#2169)
2. Open an [issue on github](https://github.com/adie-hub/adie-hub.github.io/issues)
