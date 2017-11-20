---
layout: tutorial_page
permalink: /rule_8
title: Rule 8
header1: Workshop Pages for Students
header2: Have a main landing page
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover having a main landing page.
author: Ann Meyer
modified: 2017-11-20
---

# Learning Objectives  

* Set up your main landing page

# Your Main Landing Page

This is the page visitors and students will see when they first head to your website. It needs to be easily navigable with visitors easily finding the content or workshop they are looking for.

Things your page should have:

* navigation to the different sections of your page  
* sections for each year of workshops  
* a way to find out about and/or register for upcoming in-person workshops

Let's revisit and set up the main landing page for our website.  You can do this either on the GitHub website (easiest) or on your desktop.

In GitHub, in your websiter repo, head to `_layouts` and click on `default.html`.  This is where we'll add some navigation buttons.

Change this:

```
      {% if site.github.is_project_page %}
        <a href="{{ site.github.repository_url }}" class="btn">View on GitHub</a>
      {% endif %}
      {% if site.show_downloads %}
        <a href="{{ site.github.zip_url }}" class="btn">Download .zip</a>
        <a href="{{ site.github.tar_url }}" class="btn">Download .tar.gz</a>
      {% endif %}
```

to this:

```
      <a href="#Introduction" class="btn">Introduction</a>
      <a href="#Current" class="btn">Current Workshops</a>
      <a href="#Past" class="btn">Past Workshops</a>
```

Now, in your website repo, click on `index.md`.  We are going to add content to our different sections.

```
---
layout: default
---

# Welcome <a id="Introduction"></a>

Welcome to our awesome workshops! On these pages you'll find links to our workshop contents.  

<a href="made up url" class="btn">Register for our upcoming workshops</a>

---

# Current Workshops <a id="Current"></a>

Here's a list of our current workshops:

<a href="made up url">Current Workshop 1</a>
---

# Past Workshops <a id="Past"></a>

<a href="made up url">Past Workshop 1</a>

---
```

Once you commit these changes, they will appear on your website.
