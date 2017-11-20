---
layout: tutorial_page
permalink: /rule_10
title: Rule 10
header1: Workshop Pages for Students
header2: Use teams
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover adding Google tracking to your website.
author: Ann Meyer
modified: 2017-11-20
---

# Learning Objectives  

* Add Google tracking to your website

# Google Analytics

Ever wondered how many people visit your website, how long they spend on each page, what they are looking at, and where they are coming from?  [Google Analytics](https://www.google.ca/analytics/#?modal_active=none) can provide these answers and many more. 

To use Google Analytics, you need to have a Google account. This tutorial **will not** cover setting up a [Google Account](https://accounts.google.com/SignUp?hl=en), getting a [tracking code](https://support.google.com/analytics/answer/1008015?hl=en), or analysing the analytics.  It will cover adding a tracking code to your GitHub website.

# Adding Google Analytics to Your Site

The Analytics code should be added to every single page you want tracked. We can make this easy by using templates and `_config.yml` file.

Conveniently, the site theme we are using already has a code snippet for Google Analytics so we just need to add in our tracking code to the config.yml file.

The code snippet in the templates looks like this:

```
    {% if site.google_analytics %}
      <script type="text/javascript">
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
        })(window,document,'script','//www.google-analytics.com/analytics.js','ga');
        ga('create', '{{ site.google_analytics }}', 'auto');
        ga('send', 'pageview');
      </script>
    {% endif %}
```

Make sure that is copied to the bottom of all of your page templates.

In the `_config.yml` file in the website repo:

```
google_analytics: place tracking code here
```

It might take some time before you have enough data in Google Analytics to actually track but you should have enough data after your first workshop.
