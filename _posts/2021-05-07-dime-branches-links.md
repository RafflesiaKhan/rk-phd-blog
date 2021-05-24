---
layout: post
title:  "Branches and Links."
tags: [Introduction, Dime]
last_updated: May 7, 2021
sidebar: blog_sidebar
feature_text: |
  ## Summary
  Creation and use of links and branches in DIME.
permalink: dime-branches-links.html
toc: true
categories: About Dime
---

## DIME Branches 

In Dime Buttons works as branches. All Buttons of a GUI are corresponding to a branch of the related GUI-SIB in a parent Interaction Process. The Branches and Buttons are matched by the label.

1. Button label works as method/operation link.
2. Button display label shows button name. 
3. Buttons are the branch to GUI model. 
4. Every branch should lead to some operation (GUI/Process).

{% include image.html file="BranchLink.png" caption="An example GUI model with branches and link process." %}

```
UploadData,EntryData and AnalyseData are the 3 branches here and home is a link process.
```

## DIME Links 

In Dime Link processes works as page link. Steps of using a process as a link
- Create a process.
- Drag the process to app.dad file and place it as ProcessComponent
- Set a url name
- Use the link from Link section of model component view. 

## Video Tutorial 

Complete direction of the above discussion
<br>

{% include video.html id="-v-flWrD1rk" title="Siteleaf tutorial video" caption="How dime branches and links works." %}
