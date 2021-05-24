---
layout: post
title:  "Data types of dime and their use!"
tags: [Introduction, Dime, Data]
last_updated: 2017-03-09T14:25:52-05:00
sidebar: blog_sidebar
feature_text: |
  ## Summary
  Brief description of DIME Data types.How we can user them to store and view data.
permalink: dime-data-flow.html
toc: true
categories: about type dime
---
## DIME Data

From [DIME WIKI](https://scce.gitlab.io/dime/content/user-guide/advanced/docs.html#data-flow "A link") we learn the life-cycle of a GUI model starts with a rendering, including the injection of initially specified data. Similar to the process models, the GUI models take usage of a data context as well, which can be used analogous. In contrast to the processes the GUI models cannot receive data from output ports of a start node. The initially needed data has to be specified as an input in the properties of a variable in the data context. Every variable, which is specified as an input, will result in an Input Port of the corresponding GUI SIB.


For accessing data between Process model DIME includes

  -``PrimitiveInputPort`` i.e., branch output, receives data from GUI model and

  -``PrimitiveOutputPort`` i.e., GUI input, view/shows data to GUI model

{% include image.html file="dataflow.png" caption="Data variables in a Process model." %}
<br>
For accessing data between GUI model DIME includes

  -``PrimitiveVariable`` i.e., data context's attribute , receives data from GUI model and stores to application

 

{% include image.html file="dataflow2.png" caption="Data variables in a GUI model." %}

## Video Tutorial 

Complete direction of the above discussion
<br>

{% include video.html id="N4vPQcYig4U" title="Siteleaf tutorial video" caption="How to enter data in a dime application. What are the possible data type." %}