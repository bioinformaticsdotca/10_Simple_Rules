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
* Use metadata with BioSchemas to be FAIR  

# Findable, Accessible, Interoperable, and Reusable

[FAIR guidelines](https://www.nature.com/articles/sdata201618) were designed for scientific data and stewardship but are easily appliable to educational resources.

For your workshop materials to be the most useful, learners need to be able to find them (google, links from other sources), they need to be available to anyone, they need to work on Windows, Mac, and Linux, and the contents need to be adaptable or modifiable.

Having your content on GitHub is a good start for accessibility and adding CC-ShareAlike licenses helps with reusability.  Using metadata tags and [BioSchemas](bioschemas.org) in your page templates will help with findability.

## Metadata Tags and BioSchemas

These are tags that keep the content from being displayed on your site but are machine readable.

In BioSchemas, somethings that you want to include but don't necessarily want displayed are:

* the event type   
* the audience group  
* the learning resource type  
* the license  
* the content author  
* what workshop this is part of  
* the date the content was last modified  
* a description of the content  

Here is the code snippet that should be added to the `<head>` section of your workshop landing and tutorial templates:  

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
						<meta div itemprop="author" itemscope itemtype="http://schema.org/Person">
							<meta span itemprop="name"> {{ page.author }} </span>
						</div>
					</div>
					<meta div>Target audience:
						<meta span itemprop="audience" itemscope itemtype="http://schema.org/Audience">
   							<meta span itemprop="audienceType">Omics</span>
   							<meta span itemprop="genre">Omics</span>
						</span>
					</div>
					<meta div>Material: 
						<meta span itemprop="learningResourceType">text</span>,
						<meta span itemprop="learningResourceType">exercise files</span>, 
						<meta span itemprop="learningResourceType">scripts</span>
					</div>
					<meta div>License:
						<meta span itemprop="license">https://creativecommons.org/licenses/by-sa/4.0/</span>
					</div>
					<meta div> Tutorial as part of workshop
						<meta span itemprop="isPartOf"> {{ page.home }} </span>
					</div>
					<meta div>Last modified:
   						<meta span itemprop="dateModified"> {{ page.modified }} </span>
					</div>
				</div>
```



[Next rule](https://bioinformaticsdotca.github.io/rule_5)
