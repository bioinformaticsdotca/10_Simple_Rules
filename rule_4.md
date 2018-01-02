---
layout: tutorial_page
permalink: /rule_4
title: Rule 4
header1: Workshop Pages for Students
header2: Be FAIR
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover using metadata to be FAIR.
author: Ann Meyer
modified: 2017-11-17
---

# Learning Objectives

Be able to:

* Know what is FAIR  
* Use metadata with BioSchemas to be FAIR  

# Findable, Accessible, Interoperable, and Reusable

[FAIR guidelines](https://www.nature.com/articles/sdata201618) were designed for scientific data and stewardship but are easily appliable to educational resources.

For your workshop materials to be the most useful, learners need to be able to find them (google, links from other sources), they need to be available to anyone, they need to work on Windows, Mac, and Linux, and the contents need to be adaptable or modifiable.

Having your content on GitHub is a good start for accessibility and adding CC-ShareAlike licenses helps with reusability.  Using metadata tags and [BioSchemas](bioschemas.org) in your page templates will help with findability.

## Metadata Tags and BioSchemas

Metadata tags are tags that keep the content from being displayed on your site but are machine readable.

In BioSchemas, somethings that you want to include but don't necessarily want displayed are:

* the event type   
* the audience group  
* the learning resource type  
* the license  
* the content author  
* what workshop this is part of  
* the date the content was last modified  
* a description of the content  

Several groups, including [GOBLET's Standards Committee](https://www.mygoblet.org/content/standards), are working on best practices for using BioSchemas to tag educational content from in-person and online workshops.  

[Here](https://raw.githubusercontent.com/bioinformaticsdotca/10_Simple_Rules/master/bioschemas.txt) is the code snippet that we will add to the `<head>` section of our workshop landing and tutorial templates that we created in [rule 3](https://bioinformaticsdotca.github.io/rule_3). Paste this code right before the `</head>` tag in the 2 layouts.  Remember to include this code in any new layouts you create!    

[Next rule](https://bioinformaticsdotca.github.io/rule_5)
