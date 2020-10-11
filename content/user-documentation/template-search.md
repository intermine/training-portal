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

A pre-defined search which provides a simple form with one or more variables for you to define. It provides a list of terms making the search easier for someone who do not know the right terms to search for and provides default values for each template search.


## How To Get Data Using The Bluegene Template Search


1. Go to bluegenes homepage link  http://bluegenes.apps.intermine.org/
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/home.PNG)


2. At the top of the webpage, you will find a navbar and a dropdown with its default value of “Flymine”. You can click on this dropdown to select a mine of your choice or you can proceed with the Flymine.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/fly.PNG)



3. Proceed to click on “TEMPLATES”.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/template.PNG)

4. Clicking on templates redirects you to a webpage where you see an instruction telling you how to filter your data. You can filter your data in two ways:

## A.Filter By Category:  
 You can click on the buttons to filter the searches. The buttons include:

## a. All : 
To provide you with all information you might want to know

## b. Regulation: 
To filter the data and provide transcription factors information of the mine involved.

## c. Function: 
To filter data by gene functions

## d.Expression:
 To filter data by Dna an Rna Expressions.

## e.Homology: 
To filter data by its gene homologues.

## f.Genes: 
To filter data by gene information.

## g.Interactions: 
To filter by its genetic interactions.

![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/cate.PNG)



## B. Filter By Description: 
You can write the description of the data you want to find and the data automatically pops out.
![alt text](https://raw.githubusercontent.com/LizzyKate/training-portal/lizzy/content/user-documentation/template-img/des.PNG)





## TROUBLESHOOTING

No result found on my template search  - Why?

All templates should return results with the default  values provided, if you find a template that doesn’t, please contact  
<a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a>

If you provided your own values, it may mean that we don’t have the data you are looking for or if it is a complicated search with optional constraints, some of the required data might be there but not all of it resulting in no results.

If you have activated multiple optional constraints, it is often a good idea to turn these on individually to see if one in particular is causing the problem. By default adding a constraint means that the data MUST satisfy that constraint for the search to return results - see <a href="https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin">Outer joins</a> for more details.

Please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> if you require further attention.




{{< childpages >}}