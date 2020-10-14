+++
title = "User Documentation - Template Search"
description = "This documentation explains how to search the Bluegene database without having to construct your own query or understand the data structure before searching for your own data."
weight = 3
+++

{{< lead >}}

- [User Doc](https://flymine.readthedocs.io/en/latest/)
- Try online on [BlueGenes](http://bluegenes.apps.intermine.org/)
{{< /lead >}}



## How To Search For Genomic Data In Bluegenes Using Template Searches



Bluemine is a query interface that provides variety of ways which you can view and analyse data, whether you are looking at a single gene, a list of over 1000 genes, transcription factor binding sites or protein interactions.

This query interface has provided options to search for this data and it includes:

1. Keyword Search
2. Template Search
3. Query Builder
4. Region Search





## Template Search

A pre-defined query that has been created to search for data which provides a simple form with one or more variables for you to define. It allows you to search for databases without having to construct your own query or understand  the underlying data structure. In other words, it provides a list of terms making the search easier for someone who do not know the right terms to search for and provides default values for each template search.


## How To Get Data Using The Bluegene Template Search


1. Go to bluegenes homepage link  http://bluegenes.apps.intermine.org/
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/home.PNG)


2. At the top of the webpage, you will find a navbar and a dropdown with its default value of “Flymine”. You can click on this dropdown to select a mine of your choice or you can proceed with the Flymine.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/fly.PNG)



3. Proceed to click on “TEMPLATES”.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/template.PNG)

4. Clicking on templates redirects you to a webpage where you see an instruction telling you how to filter your data. You can filter your data in two ways:

## A.Filter By Category:  
 You can click on the buttons to filter the searches by category. The buttons include:

## a. All : 
To provide you with all information you might want to know about any data type.

## b. Regulation: 
To filter the data and provide transcription factors information of the mine involved.

## c. Function: 
To filter data by functions

## d.Expression:
 To filter data by Expressions.

## e.Homology: 
To filter data by homologues.

## f.Genes: 
To filter data by information.

## g.Interactions: 
To filter data by interactions.

![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/cate.PNG)



## B. Filter By Keywords: 
You can write the keyword of the data you want to find and the datatype automatically pops out.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/des.PNG)


## Description Of Each Templates
Each template has a short name and a description. The short name is provided so that users can quickly scan the available searches and provide the one that they need. The description will provide you with more details of the search and any limitations to the values you can enter.

## Short Name
![alt text]()

## Description
![alt text]()

## Details Of A Template Search
A template search provides you with a form, with one or more keywords to set. Some will require you to enter a value, while others will provide drop-down lists for you to select from. Some templates provide optional constraints. These constraints can be turned on or off depending on your wish. Once you are have provided the options you want to chose so as to minimize your data search, results based on those options are provided with a button signalling you to click to show more results. 

## Dropdowns
![alt text]()

## Optional Constraints
![alt text]()

## Results
![alt text]()

## View More Results
![alt text]()

## TROUBLESHOOTING

No result found on my template search  - Why?

All templates should return results with the default  values provided, if you find a template that doesn’t, please contact  
<a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a>

If you provided your own values, it may mean that we don’t have the data you are looking for or if it is a complicated search with optional constraints, some of the required data might be there but not all of it resulting in no results.

If you have activated multiple optional constraints, it is often a good idea to turn these on individually to see if one in particular is causing the problem. By default adding a constraint means that the data MUST satisfy that constraint for the search to return results - see <a href="https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin">Outer joins</a> for more details.

Please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> if you require further attention.




{{< childpages >}}