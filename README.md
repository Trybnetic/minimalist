# Minimalist

[![Build Status](https://travis-ci.org/Trybnetic/minimalist.svg?branch=master)](https://travis-ci.org/Trybnetic/minimalist)
[![License](https://img.shields.io/github/license/Trybnetic/minimalist.svg)](https://github.com/Trybnetic/minimalist/blob/master/LICENSE.txt)  

Minimalist is a simple and light weighted [jekyll](http://jekyllrb.com/) theme. It focuses on a minimalistic design but still providing all functionality for a personal blog.

## Installation
To install Open Recipes you have to install [jekyll](https://jekyllrb.com). After successfully installing jekyll you have to clone this repository to your computer:
```
git clone https://github.com/Trybnetic/minimalist.git
```
Then switch into the directory and start jekyll:
```
cd minimalist
bundle exec jekyll serve
```
The last command starts a webserver on your local machine. Now you should have a copy of the site running at `http://127.0.0.1:4000/`. Open this url with your webbrowser and explore the site.  
By changing some of the files (except of the `config.yml`) the changes will be displayed immediately.

## Usage
After you successfully installed the theme on your computer you can add additional blog posts by creating new files in the `_posts` directory. The new files have to follow the name convention `year-month-day-title.md`.


## Post structure
**Example:**
```
---
layout: post
title:  "Lorem ipsum"
date:   2017-09-06 01:03:29 +0200
categories: lorem ipsum
---

Eius ut fugiat omnis. Autem nihil dignissimos deserunt eum. In adipisci ipsum
natus saepe facere. Aspernatur velit autem sed. Rerum provident non incidunt id
expedita aliquam non. Eum sit saepe autem nam aut voluptatem non et.

<!--more-->

Sequi et ut consequatur et incidunt expedita provident. Iste ipsa eaque qui.
Totam vitae quasi nulla aut aliquam harum. Quibusdam et deserunt possimus
dolores voluptate facilis corrupti vero.

```

Each post consits of a header and a body. In the header defined by the `---`, you have to make basic definitions concerning the blog post.   
In the first line of the example the layout is specified. This should be `layout: post` for all blog post except you want to add a custom layout for a certain media type. In the second line the title of the blog post is specified. In the third line you have to add the date of publication which will be displayed on top of the blog post on the website. In the fourth and last line of the header you can add categories so your blog posts gets displayed at the categories site `/categories/<category>/`. The existing categories can be found in the `categories/` folder.  
Finally, you can add `<!--more-->` in your text to indicate that the text till this delimiter should be used as a preview at the homepage.

## Categories
This theme supports using categories. If you want to add custom categories you need to add a `<your category name>.md` file to the `categories/` folder, where `<your category name>` denotes the name of the category you want to add.  
Your `<your category name>.md` needs to contain the following lines:
```
---
layout: category
category: <your category name>
permalink: /categories/<your category name>/
---
```
The first line specifies that the layout of the rendered site is category. In the second line you have to specify the name of the category you want to add. And finally, you have to specify the link scheme to your category site.

## Host your own blog
The simplest way to host your own blog with the [Minimalist](https://trybnetic.github.io/minimalist/) theme is to fork [the repository](https://github.com/Trybnetic/minimalist/) and use the [gh-pages](https://pages.github.com/) functionality provided by [GitHub](https://github.com/).

## License
This jekyll theme is [licensed under the MIT license](https://github.com/Trybnetic/minimalist/blob/master/LICENSE.txt). Check the license on whether and how you are allowed to use, modify and distribute this theme.
