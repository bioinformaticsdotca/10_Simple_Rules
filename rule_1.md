---
layout: tutorial_page
permalink: /rule_1
title: Rule 1
header1: Workshop Pages for Students
header2: Put thought into your user or organisation name
image: /site_images/CBW_bigdata_icon.jpg
home: https://bioinformaticsdotca.github.io/GOBLET_GitHub_2017
description: This rule will cover choosing a user or organisation name and creating your site repo.
author: Ann Meyer
modified: 2017-11-15
---
# Learning Objectives

* Difference between individual or organisation account  
* Create site repo

# Different Account Types

## Individual Accounts

* All users have individual accounts.  This is **your** identity on GitHub     
* Include unlimited *public* repos and unlimited collaborators
* Can pay for private repos

## Organisation Accounts

* Shared accounts with **owners, administrators, and members** with different levels of privileges and access  
* Include unlimited *public* repos and unlimited collaborators  
* Have the ability to assign teams
* Can require all organisation members to use two-factor authentication 
* Can pay for private repos, apply for education discount, or request a not-for-profit account for free private repos  

### Getting a Not-For-Profit Organisation Account

These accounts include unlimited private repos and unlimited users, free of charge.

Available to official nonprofit organizations and charities that are nongovernment, nonacademic, noncommercial, nonpolitical in nature, and have no religious affiliation.

To request a not-for-profit account, visit https://github.com/nonprofit.  

Special accounts are also available to [academic institutions](https://education.github.com/).  

# Create Your Site Repo on GitHub

Your site repo will contain all the materials for **creating** your website (style sheets, layouts, etc.).  

In an internet browser, go to github.com and log into your account or your organisation account.

To create a new repo, at the top of the page in the black navigation bar, click on "+" and select "New repository".

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/new_repo.png?raw=true" alt="New Repo" width="450" align="middle" />

Under "Owner", ensure that the correct owner is selected in the dropdown since you might be an owner of an individual account and several organisations.

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/Owner.png?raw=true" alt="Owner" width="450" align="middle" />

Under Repository Name, in the textbox, enter the name of your site.  This is where the name of your individual account or organisation account becomes **very** important.  The format of the name is username.github.io *or* organisation.github.io (where username is your GitHub username and organisation is your GitHub organisation name).  Your repo will not render as a website if you do not use this format.

<img src="https://github.com/bioinformaticsdotca/10_Simple_Rules/blob/master/img/site_name.png?raw=true" alt="Site Name" width="650" align="middle" />

Decide whether the repo will be *public* (anyone on the internet can view it but only those you choose can change it) or *private* (only you and those you choose can view it and change it).   

It isn't necessary to initialize with a README or license.

Hit the green "Create repository" button.

# Pull Your Repo to Your Computer

Switch over to a terminal on your computer.

Create a new directory to store your website files.

```
mkdir GitHub
cd GitHub
```

You will need to clone your newly created repo to your computer.  To do this, type:

```
git clone https://github.com/username/username.github.io
```

Remember to change *username* to your user or organisation name.

Next, you will need to move into your repo, initialize it as a git repo (for version control), add a README, and add the remote.  To do this, type:

```
cd username.github.io
git init
echo "# mygobletorg.github.io" >> README.md
git add .
git commit -m "first commit"
git remote add origin https://github.com/username/username.github.io.git
git push -u origin master
```
And that's it! You've created the repo for your site.


[Next rule](https://bioinformaticsdotca.github.io/rule_2)
