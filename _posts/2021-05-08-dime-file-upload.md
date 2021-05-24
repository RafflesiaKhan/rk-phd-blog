---
layout: post
title:  "Uploading file in dime"
tags: [Introduction, Dime]
last_updated: May 8, 2021
sidebar: blog_sidebar
feature_text: |
  ## Summary
  How to create process, gui and link for uploading a file.
permalink: dime-file-upload.html
toc: true
categories: About Dime
---

## Files in DIME

The File Component can be used to Download a File. First the file name is displayed followed by a button with the specified label. The file to download can be specified by a file guard process. But, for uploading a file we can use the 'Field' component. Here we will talk about uploading a small csv file

Steps for uploading file

 - Create a process and a gui model. GUI model need the upload layout and Process need the operations.
 - Inside the GUI add a Form component. In dime Form is used for data collection of entry.
 - ADD a Field component to the Form.
 - Set Properties InputType as SampleFIle and a label
 - Create a primitive variable e.g., file
 - Set Properties DataType as File and a label/name
 - Drag 'FromSubmit' edge from file variable to Field component   
 - Drag 'AddPrimtivetoSubmission' edge from file variable to Submit button. This submits the file.
 - Add a Text component to the for setting successful message after file upload. 
 - Drag 'IF' edge from file variable to Text component 
 - Drag ConcreteUser from model view Data section.
 - Add an 'IF' edge from current uer to From. This identifies the user, who is uploading.   



 {% include image.html file="GUIFileU.png" caption="An example GUI model for file uploading task." %} 


## Video Tutorial 

Complete direction of the above discussion
<br>

{% include video.html id="VNQF_7kjgX0" title="Siteleaf tutorial video" caption="How to upload file on a dime application ." %}