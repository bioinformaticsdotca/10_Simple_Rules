---
layout: tutorial_page
permalink: /rule_7
title: Rule 7
header1: Workshop Pages for Students
header2: Use submodules
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover using submodules to pull your content into the website repo.
author: Ann Meyer
modified: 2017-11-20
---

# Learning Objectives

* Setting up submodules  
* Updating submodules  

# Why Submodules

You've created your workshop in a repo that isn't your website repo so how do you get the two repos together so that your workshop content is part of your website??? To do this, we'll use submodules.  Submodules are a little tricky since you need to actively update your main repo to pull in changes that are made in the submodules.  It's advantageous since what is in the main website repo *should* be the last working version of any workshop - changes only get pulled into the website repo if things are working. 

# Setting Up and Adding New Submodules

On your computer, in terminal, make sure that both your website repo and workshop repo are on the master branch.

```
cd <path_to_website_repo>
git pull origin master
cd <path_to_workshop_repo>
git pull origin master
```

Change to your website repo and add the workshop repo as a submodule:

```
git submodule add <path_to_workshop_repo>.git
```

You should now have a `.gitmodules` file.

```
cat .gitmodules
```

To push these changes to GitHub (and have them appear on your website):

```
git status
git commit -m "Add submodule <workshop name>"
git push origin master
```

Now when you go to your website repo, you should see your workshop repo followed by an `@` and then some letters and numbers (this hash refers to the version of the workshop repo that was pulled).  Your workshop content should also now be available through your website (be a patient if it doesn't appear right away, it might take a couple of minutes to render). 

# Updating Submodules

When you make changes to your workshop repo, you will need to update the submodule path in your website repo so that the hash reference gets updated.  This process is similar to adding a submodule.

I prefer to update the original workshop repo at the same time I update the submodule.

```
cd <path_to_workshop_repo>
git pull origin master
cd <path_to_submodule_in_website_repo>
git pull origin master
cd ..
git add <submodule>
git commit -m "update submodule path"
git push origin master
```

Any changes you've made to your workshop repo should now be visible on your website.



[Next rule](https://bioinformaticsdotca.github.io/rule_8)
