---
layout: tutorial_page
permalink: /rule_5
title: Rule 5
header1: Workshop Pages for Students
header2: Put important information in the page header
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover using the header section.
author: Ann Meyer
modified: 2017-11-20
---

# Learning Objectives

To be able to:

* Use page headers

# Page Headers

Now that you have templates for each of your content types, you can start creating new pages.  Headers at the top of each one of your pages will allow you to put important information (like the BioSchemas info) in one spot.  This information will then be populated into your page in the spots indicated in your page template.

Page headers are placed at the top of each page between dashes:

```
---
---
```

The header for our example workshop's landing page should look like this:

```
---
layout: 2_day_main
permalink: /awesome_workshop_1
title: Awesome Workshop 1
header1: Awesome Sauce Workshops
header2: Awesome GitHub Workshop
description: Instructions to create GitHub websites
author: CBW
modified: 2017-11-20
home: https://annmeyer.github.io
---
```

And the header for the tutorial page should look like this:

```
---
layout: tutorial
permalink: /awesome_tutorial_1
title: Tutorial 1
header1: Awesome Sauce Workshops
header2: Amazing Tutorial 1
home: https://annmeyer.github.io/awesome_workshop_1
description: First tutorial on creating github pages
author: CBW
modified: 2017-11-20
---
```

Copy these headers into text documents.



[Next rule](https://bioinformaticsdotca.github.io/rule_6)
