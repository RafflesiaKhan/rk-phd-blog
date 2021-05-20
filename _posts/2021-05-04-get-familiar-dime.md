---
layout: post
title:  "Getting Familiar with DIME Models."
tags: [Introduction, Dime]
last_updated: May 3, 2021
sidebar: blog_sidebar
summary: Brief description of DIME Models.
permalink: get-familiar-dime.html
datatable: true
toc: true
categories: about toto dime
---
## Model Types and Concrete Models


The main model types, model elements and models of a general DIME application.

### Data Model 
The data model of DIME application, representing both the concrete and abstract data. It contains both unidirectional and bidirectional relations such as association and inheritance. 

{% include image.html file="datamodel.png" caption="The four data model that DIME includes." %}


### Graphical User Interface Models
In DIME, the GUI model type represents the structure (layout and contents) of a DIME app's individual web pages. A collection of GUI models defined, therefore the abstract and concrete ``look" of the presentation layer of a DIME application. Every GUI models of a DIME app is created using components from DIME palette. The GUI models call process models to execute an operation. These GUI models are also reusable.

{% include image.html file="guiintro.jpg" caption="An example GUI model with it's corresponding web-page view." %}


### Native DSLs
In DIME, the actions and services are collected in domain specific palettes that are basically a service or component oriented DSL. The DSL elements correspond to (calls to) individual functionalities that are either directly implemented or provided by an external service provider, like e.g. the database. The individual functionalities are modelled as special native types called SIBs, for service-independent building blocks, where service-independent means that they are widely reusable across applications. 

These Native SIBs enable interoperability on a structural level. 


### Data-flow
In DIME data flow is explicitly modelled within the process models. The input/output ports of SIBs can either be connected directly with each other or used to read and write from/to variables placed in a dedicated container representing the data context [More Details](https://link.springer.com/chapter/10.1007/978-3-319-47169-3_60).


### Process models
Process models express the business logic in a fashion roughly similar to Activity Diagrams, but with a clean formal semantics. There are several process types: basic, interactable and interaction processes. Each process type follows certain rules regarding which kind of SIBs they contain and the kind of tasks they express. The graphical syntax and general handling are the same for all the types of SIBs and processes. 

The collection of process models together with the connected GUI, actions and data flow expresses the behaviour of the application in terms of its operation. 

Process models can also be of different type such as
#### Basic Processes
Basic Processes consist of native SIBs and built-in SIBs, and express the smallest processes of the application's business logic. In a DIME app, basic processes models are the CRUD (i.e., create, read, update, and delete) operations and data operations.

#### Interactable Processes
Interactable Processes work as interfaces between the front-end layer and the backend of the application. They are similar to  Basic processes, but are restricted to non-native type. The StartUp process is a interactable process in a general DIME app. This process includes operation of successful login of user with different role. 

#### Interaction Processes
Interaction Processes are used to define the immediate interaction between user and application, accordingly they can be seen as a sitemap. Where interactable SIBs communicate with the backend, interaction SIBs establish a new hierarchy level with the frontend. 


#### Security Processes
Security Processes realize the (role based) access control with a predefined interface.  

{% include image.html file="Process.jpg" caption="An example DIME Process Model with other processes, data-flow, branches and guard process." %}