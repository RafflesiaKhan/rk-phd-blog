---
layout: post
title:  "Test DIME new application"
tags: [Introduction, Dime, Run]
last_updated: May 2, 2021
sidebar: blog_sidebar
feature_text: |
  ## Summary
  This describes 'How to create and run a new dime application'
permalink: new-app-run.html
toc: true
categories: about dime
---

## Test a new application with DIME

Follow these instructions to create and run a new DIME Application.

### 1. Creating new App

For creating a new DIME application

- Right click on DIME explorer and choose 'New DIME App' from the following options
- Select 'Create a new application form starch'
- Leave the project name as it is
- And his 'Finish'

```
Create a new application form starch - will create a simple DIME app
Initialize the project with an Example App - provides you options to select an existing example DIME project architecture

```
<img src="images/createnewapp.png" style="width: 650px;"/>


### 2. Running new App

For running a new DIME application, here we will follow the docker option. For more information please visit [APP Development] (https://scce.gitlab.io/dime/content/user-guide/development-with-docker.html#requirements)

I found [this video](https://www.youtube.com/watch?v=YH3sutAsxEM) really helpful for Docker-Compose installation in Windows 10 Home Edition

How to run you DIME app:

- Expand you 'NewApp' at DIME  project explorer
- Open app.dad
- Hit G for generating the application code

{% include note.html content="You must keep the 'app.dad' file open for code generation" %}

```yaml
NewApp
- dimemodels
  - app.dad
```        

<img src="images/newAppG.png" style="width: 650px;"/>

- After successful code generation go to 'target' folder

```yaml
NewApp
- target
```  

- Open two command window , you can also use Git BASH
- Run this command in one window : docker-compose up
- When the first command comes to 'Started Services' Run this command an another: docker-compose up --detach --build webapp dywa-app 
- Wait for the second command finish running successful 
- GO to 'http://127.0.0.1:8080/'
- Your app is running on local port 8080

## Video Tutorial

### Part One- Create and Run 'New DIME APP'

This video shows the steps for creating and running a new application with dime:

<iframe width="560" height="315" src="https://www.youtube.com/embed/sOSDdggSuJg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


### Part Two- What's Already Tthere

This video describes what is already created for you in the 'NewApp': General thoughts about GUI and Process :

<iframe width="560" height="315" src="https://www.youtube.com/embed/9mZ__OA2pkU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


