---
layout: post
title:  "Creating Header and Footer."
tags: [Introduction, Dime]
last_updated: May 3, 2021
sidebar: blog_sidebar
feature_text: |
  ## Summary
  How to add header and footer to your dime application.
permalink: dime-head-foot.html
toc: true
categories: About Todo Dime
---

## Adding header & footer to DIME application

Headers and footers are useful for including material that we want to appear on every page of a web-application such as application name, company logo, buttons etc. For every web-application a header(i.e., the top margin of a page) , and a footer (i.e., the bottom margin of each page) is very general component.

### Header

Steps:
 - Create a new GUI and name it as Header
 - Inside the body add Top Navigation Bar
 - One can add any gui components as their choice
 - For styling try fixing properties of each components 
 - Save it

{% include image.html file="Header.jpg" caption="An example header GUI model with it's corresponding web-page view." %}

### Footer

Steps:
 - Create a new GUI and name it as Footer
 - Inside the body try adding tour company logo image using 'Image' gui component 
 - For styling try fixing properties of each components 
 - Save it

{% include image.html file="Footer.jpg" caption="An example footer GUI model with it's corresponding web-page view." %}

#### Using header & footer

 - At any page's GUI model right click on diagram editor and choose 'Add Header'
 - Place the header template at GUI top
 - Drag your created header gui from model component views to header template on diagram editor
 - Then again right click on respective GUI's diagram editor and choose 'Add Footer'
 - Place the created footer template at GUI bottom
 - Drag your created footer gui from model component views to footer template on diagram editor
 - Save everything 
 - Generate code and run application

## Video Tutorial 

Please watch this video for better understanding of header & footer creating with dime.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ge9Ryupq_kk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

#### Adding Custom Header to Home Page Only

At the home page the header should so different structure, at it's public area. So here we are discussing about a custom header. 
  - We can create custom header for any page, here we are adding header to the home page.
  - Fo that delete the Header gui from public home page and create a new header to the 'header' template. 

{% include image.html file="customhead.png" caption="An example custom header for home page & the general header" %}

<br>
#### Adding Image/Gif

Adding image/gif file to DIME application includes the following steps

 - Add a Row or Column to GUI body as layout for placing the image
 - Drag Image content from palette to layout
 - Go to Image properties
 - Set Path of the image e.h., asset/image.png
 {% include note.html content="image should be placed at project's asset folder" %} 
<br>
{% include image.html file="Dimege.PNG" caption="An example custom header for home page & the general header" %}

## Video Tutorial 

Complete direction of the above discussion

{% include video.html id="wetniHXL-do" title="Siteleaf tutorial video" caption="How can we create custom header for home page and Add image in DIME application." %}

<!--<iframe width="560" height="315" src="https://www.youtube.com/embed/wetniHXL-do" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>-->

