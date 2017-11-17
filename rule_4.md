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

* Know what is FAIR  
* Use metadata to be FAIR  

# Findable, Accessible, Interoperable, and Reusable

[FAIR guidelines](https://www.nature.com/articles/sdata201618) were designed for scientific data and stewardship but are easily appliable to educational resources.

For your workshop materials to be the most useful, learners need to be able to find them (google, links from other sources), they need to be available to anyone, they need to work on Windows, Mac, and Linux, and the contents need to be adaptable or modifiable.

Having your content on GitHub is a good start for accessibility and adding CC-ShareAlike licenses helps with reusability.  Using metadata tags in your page templates will help with Findability.

## Metadata Tags

These are tags that keep the content from being displayed on your site but are machine readable.  

```
			<!-- BioSchemas -->
				<div itemscope itemtype="http://schema.org/creativeWork">
					<meta itemprop="genre" content="trainingMaterial">
					<meta div itemprop="name"> {{ page.header2 }} </div>
					<meta div itemprop="description"> {{ page.description }} </div>
					<meta div>Event type: 
						<meta span itemprop="eventType">Workshops and courses</span>
					</div>
					<meta div>Author: 
						<div itemprop="author" itemscope itemtype="http://schema.org/Person">
							<span itemprop="name"> {{ page.author }} </span>
						</div>
					</div>
					<div>Target audience:
						<span itemprop="audience" itemscope itemtype="http://schema.org/Audience">
   							<span itemprop="audienceType">Omics</span>
   							<span itemprop="genre">Omics</span>
						</span>
					</div>
					<div>Material: 
						<span itemprop="learningResourceType">text</span>,
						<span itemprop="learningResourceType">exercise files</span>, 
						<span itemprop="learningResourceType">scripts</span>
					</div>
					<div>License:
						<span itemprop="license">https://creativecommons.org/licenses/by-sa/4.0/</span>
					</div>
					<div> Tutorial as part of workshop
						<span itemprop="isPartOf"> {{ page.home }} </span>
					</div>
					<div>Last modified:
   						<span itemprop="dateModified"> {{ page.modified }} </span>
					</div>
				</div>
```
