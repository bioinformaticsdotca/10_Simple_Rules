---
layout: tutorial_page
permalink: /rule_6
title: Rule 6
header1: Workshop Pages for Students
header2: Individual repos for each workshop
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover having individual repos for each workshop.
author: Ann Meyer
modified: 2017-11-20
---

# Learning Objectives

Be able to:

* Understand the importance of individual repos for each workshop  
* Set up your workshop repo  
* Create content for your workshop

# Why Using Individual Repos for Each Workshop is Important  

You may offer the same workshop every year (or multiple times a year) and the content for that workshop might change subtly (eg a different instructor but the same content) or the content might change drastically (eg shift to different software or pipeline).  In both cases, you want past students to be able to access the content they were taught but you also want new students to access the most up-to-date content.  You could simply create a new directory in your repo for each time you offer a workshop but this gets very messy very quickly and when students download or clone your repo it's difficult for them to determine which workshop they might have taken.  The size of your repo also becomes rather large if you offer multiple workshops a year.  

Creating a separate repo each time you offer a workshop:

* keeps repo sizes small (for cloning and downloading)  
* keeps students from downloading unnecessary content (from previous workshops or unrelated workshops)  
* reduces student confusion  
* allows students to access content from past workshops they attended   
* allows you to give credit to present and past instructors  
* keeps things organized  

# Setting Up Your Workshop 

Let's set up our workshop.  

## Step One: Create a New Repo

Follow the instructions in [rule 1](bioinformaticsdotca.github.io/rule_1) for creating a new repo.  Let's call this repo **GOBLET_AGM_2017**.  The naming structure here is important since you want the workshop name (GOBLET AGM) as well as when it was offered (2017) to be readily apparent.  If you offer this workshop multiple times a year, you might also want to include the month or location in the name.

## Step Two: Create the Landing Page for the Workshop  

In the workshop repo (GOBLET_AGM_2017), click "Create New File".  Name the file "main_GOBLET_AGM_2017.md". The .md extension means that this file is written in [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet). 

Paste in the header section we created in [rule 5](https://bioinformaticsdotca.github.io/rule_5).

Below the header section, you can add any content you wish, such as:

```
Welcome to GOBLET AGM 2017.
```

## Step Three: Create the Tutorial Page for the Workshop  

In the workshop repo (GOBLET_AGM_2017), click "Create New File".  Name the file "tutorial1_GOBLET_AGM_2017.md". 

Paste in the header section we created in [rule 5](https://bioinformaticsdotca.github.io/rule_5).

Below the header section, you can add any content you wish, such as:

```
This is the first tutorial for GOBLET AGM 2017.
```

## Step Four: Link the Tutorial Page to the Landing Page

Back in "main_GOBLET_AGM_2017.md", we can now put a link to our tutorial file. Links in markdown are created with square brackets for the text followed by curvy brackets for the link without space between the two sets of brackets.

```
[Tutorial 1](<link to tutorial 1>)
```
Remember to replace `<link to tutorial 1>` with the actual link to your tutorial page.

[Next rule](https://bioinformaticsdotca.github.io/rule_7)
