---
layout: tutorial_page
permalink: /rule_2
title: Rule 2
header1: Workshop Pages for Students
header2: Choose a site theme that sends your message
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover choosing a site theme.
author: Ann Meyer
modified: 2017-11-17
---
# Learning Objectives

Be able to:

* Choose a theme for your site    
* Upload your theme to your GitHub repo  
* Make changes to the configuration and index files  

# Finding Themes

Themes are the template of what your website looks like.  Somethings are simple to change (colours, fonts) while others are more complex (overall layout, menus).  

3 ways to find a theme:  
1. Choose one of the [GitHub supported themes](https://pages.github.com/themes/)  
2. Find a site that uses GitHub pages and borrow their theme  
3. Create your own theme  

# Working with GitHub Supported Themes

For this example, we'll work with the [Cayman theme](https://pages-themes.github.io/cayman/).  

Download the theme by clicking on [Download .zip](https://github.com/pages-themes/cayman/zipball/master).  

Find where the file was downloaded on your computer and unzip the file on your computer. This folder contains all the supporting materials to make your website.   

## 2 Ways to Install the Theme

### Drag and Drop

Select all the files in the theme directory and drag them into the GitHub repo.

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/drag_and_drop.png?raw=true" alt="Drag and Drop" width="450" align="middle" />

Write a commit message and hit the commit button.

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/commit_theme.png?raw=true" alt="Commit Theme" width="450" align="middle" />

You can pull the changes to your local computer in your website repo within a terminal using:

```
git pull origin master
```

### Terminal

Move all files in the theme directory to your site directory on your computer and push them to GitHub.

In your site directory on your computer:

```
cp <path to theme files> .
git add .
git commit -m "Add site theme files"
git push origin master
```

# Making the Theme a Little Bit Yours

After installing the theme, if you visit yourname.github.io, it should look like the Cayman download page (it might take a few minutes for your site to actually render.  Be patient and refresh until you see the site. Remember to replace *yourname* with your GitHub username or organisation name).

To make the site yours, you need to edit a few documents.  To edit files within GitHub, click on the file name and then click on the pencil icon.

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/Edit_pencil.png?raw=true" alt="Edit Pencil" width="450" align="middle" />

## config.yml

This configuration file is for settings that affect your whole site, things that appear on every page like your email address or twitter handle, that you set up once and would rarely change.

Within this file, we need to change the title and description.  We will also add social media (twitter, github) and specify our markdown type.

```
title: My Site
description: An awesome sauce workshop site.
show_downloads: true
theme: jekyll-theme-cayman
url: bioinformaticsdotca.github.io

# Social Media

twitter_username: Bioinfodotca
github_username:  bioinformatics-ca

# Build settings
markdown: kramdown

# Google Services

google_analytics:
```

Reloading our site now should show these changes.

## Index.md

This file is the actual content of your landing page - the page the visitors to your site see first when they reach your site.

When we open this to edit, we see the page header section:

```
---
layout: default
---
```

We'll ignore this for now.

Let's delete everything after this section and type something else like "Site under construction".

Reload your site until you see the updates.

Let's pull all our changes to our local computer.  On your local computer in your website repo type:

```
git pull origin master
```

# New Commands Used in This Rule

`git pull` - brings changes made on different branches (ie the remote GitHub branch) to your current branch (ie the branch on your computer)  
`cp` - copy files from an origin location to destination



[Next rule](https://bioinformaticsdotca.github.io/rule_3)


