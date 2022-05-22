# MVC

## What exactly is Azure DevOps?

Azure DevOps is a fully integrated set of services that together provide you with all the tools necessary for building and maintaining a backlog, hosting your source code repositories, implementing continuous integration, along with delivery and testing workflows for your products before releasing them. In this course you will become familiar with Azure DevOps (formerly known as VSTS and before that, VSO) and explore the five services that make up Azure DevOps:

* Azure Boards
* Azure Repos
* Azure Pipelines
* Azure Test Plans
* Azure Artifacts

## Choose Azure DevOps Services
Choose Azure DevOps Services when you want the following outcomes:

* Quick set-up
* Maintenance-free operations
* Easy collaboration across domains
* Elastic scale
* Rock-solid security

## MVC
 is a design pattern or architecture which helps in developing the web application in a most efficient way when compared with the traditional ASP.NET Web Application.


## The Model View Controller 

(MVC) design pattern specifies that an application consist of a data model, presentation information, and control information. The pattern requires that each of these be separated into different objects.
MVC is more of an architectural pattern, but not for complete application. MVC mostly relates to the UI / interaction layer of an application. You’re still going to need business logic layer, maybe some service layer and data access layer.

![th (20)](https://user-images.githubusercontent.com/98957434/169713268-3b675bbb-f7d3-4d53-947b-ae70cb0b7115.jpg)


## What are Tag Helpers?

Advantages over HTML Helper
In our view we need some controls are html elements like form controls are heading element that help us to build View. Tag helpers help us to create that Html elements, we can extend existing html elements or we can have our own custom tags, Tag Helpers enable server-side code to participate in creating and rendering HTML elements in Razor files.

### Example of tag helper is,

Anchor tag : <a asp-action=”ActionName” asp-controller=”ControllerName” class=”customCssClass”>


## We can say that there different types of Tag Helper

1. Tag helper that extend exsiting html tag
We have already used anchor tag that takes asp-action and asp-controller as atribute and we render link according to provided attributes.

2. Custom tag helper
Later in this, we will define a custom tage helper that render a list of objects. We will use custom tag helper for that, which take list of string as parameter.

3. Tag helper that helps to do some operations seemless and update some exsisting tags or their attributes.
These tag helper are link environment , in the environment tag we can have group of files that need to be included on the base of environment like if environment is development get local javascript file but in case of production get files from CDN.
