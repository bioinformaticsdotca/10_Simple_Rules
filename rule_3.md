---
layout: tutorial_page
permalink: /rule_3
title: Rule 3
header1: Workshop Pages for Students
header2: Create templates and hace a consistent structure
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover creating templates.
author: Ann Meyer
modified: 2017-11-17
---

# Learning Objectives

* Create page templates

# Templates

Templates take care of the tedious bits of your pages.  These are things that need to be on every page and are consistent across pages.  You should have a few different templates (workshop landing page, tutorial page, etc).  

Templates are found in the `_layouts` directory and are written in html.

Currently, there should only be one template, default.html.  This is the template index.md is using.

# Creating a New Template

Let's create the template for the landing page for a 2 day workshop.

In the `_layouts` directory, click "Create new file".

Name the file "2_day_main.html".

Standard things we need are the html tags; the head tags and content; and the body tags.

```
<!DOCTYPE html>
<html lang="{{ site.lang | default: "en-US" }}">
  <head>
    <meta charset="UTF-8">

{% seo %}
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <link href='https://fonts.googleapis.com/css?family=Open+Sans:400,700' rel='stylesheet' type='text/css'>
    <link rel="stylesheet" href="{{ '/assets/css/style.css?v=' | append: site.github.build_revision | relative_url }}">
  </head>
  <body>
  </body>
</html>
```

Within the body tags, we need to define sections that hold our content but we need to be able to modify this content for individual pages.  Content that is modifiable is contained within `{{ }}`.

Things we'd like to modify on each page:



Now, within the body tags, we are going to create our sections.





