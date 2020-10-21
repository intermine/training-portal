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



Bluegene is a query interface that provides variety of ways which you can view and analyse data, whether you are looking at a single gene, a list of over 1000 genes, transcription factor binding sites or protein interactions.

This query interface has provided options to search for this data and it includes:

1. Keyword Search
2. Template Search
3. Query Builder
4. Region Search





## Template Search

A pre-defined query that has been created to search for data which provides a simple form with one or more variables for you to define. It allows you to search for data without having to construct your own query or understand  the underlying data structure. In other words, it provides a list of terms making the search easier for someone who do not know the right terms to search for and provides default values for each template search.


## How To Get Data Using The Bluegene Template Search


1. Go to bluegenes homepage link  http://bluegenes.apps.intermine.org/
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/home.PNG?raw=true)


2. At the top of the webpage, you will find a navbar and a dropdown with its default value of “Flymine”. You can click on this dropdown to select a mine of your choice or you can proceed with the Flymine.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/fly.PNG?raw=true)
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/drop.PNG?raw=true)




3. Proceed to click on “TEMPLATES”.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/template.PNG?raw=true)

4. Clicking on templates redirects you to a webpage where you see an instruction telling you how to filter your data. You can filter your data in two ways:

## A.Filter By Category:  
 You can click on the buttons to filter the searches by category for example regulation, function, expression, homology, genes and interaction
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/cate.PNG?raw=true)

## B. Filter By Keywords: 
You can write the keyword of the data you want to find and the datatype automatically pops out.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/describe.PNG?raw=true)

## Description Of Each Templates
Each template has a short name and a description. The short name is provided so that users can quickly scan the available searches and find the one that they need. The description will provide you with more details of the search and any limitations to the values you can enter.

## Short Name
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/short.PNG?raw=true)

## Description
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/keyword.PNG?raw=true)

## Details Of A Template Search
A template search provides you with a form, with one or more keywords to set. Some will require you to enter a value, while others will provide drop-down lists for you to select from. Some templates provide optional constraints. These constraints can be turned on or off depending on your wish. Once you are have provided the options you want to chose so as to minimize your data search, results based on those options are provided with a button signalling you to click to show more results. 

## Dropdowns
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/down.PNG?raw=true)


## Optional Constraints
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Optional.PNG?raw=true)


## Results
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Result.PNG?raw=true)


## View More Results
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/view.PNG?raw=true)


## Result Tables
Any search that is being looked upon,  from a template search will give you a results table. 
Results tables are also used to save your template search on the public list page.
Results tables not only display your results but also allows you to summarise, filter, add or remove columns, create and download data.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/table.PNG?raw=true)

## Understanding your result table
On the middle section, immediately below the clickable buttons found in the result table, you will see a dropdown that siginifies how may rows of data you want to see per page.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/rows.PNG?raw=true) 
Towards the right of the row dropdown, you will see a the following symbols "Backward, Lesser, Greater and Forward" that allows you to navigate to any page you want data from. You will also see a text indicating the numbering of the rows that are going to show in the result tables.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Symbols.PNG?raw=trues)
Below the rows and the page symbols section are the "Column Headings". These give the field name for the data shown and in some cases the class the data is from. 
For examples, in the following result table, the column headers are :
1. Gene Secondary Identifier
2. Gene Symbol
3. Chromosome DB Identifier
4. Chromosome Location Start
5. Chromosome Location End 
6. Chromosome Location Strand

![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/head.PNG?raw=true)

## Column Summaries
 A summary of the data can be accessed by clicking on the graph in the column header. You can read more in the <a href="https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables">Results Table Section Of the Intermine Documention</a>.
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/graph.PNG?raw=true)


 You can also filter the results in the column summary either by selecting the checkboxes or enter some text in the filter fields. You can use the sliders in the numerical data to select a range of data you wish to view. You can read more in the <a href="https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables">Results Table Section Of the Intermine Documention</a>.
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/filtered.PNG?raw=true)
 
 You can remove a column header by clicking on the "X" Symbol.
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/remove.PNG?raw=true)

 You can sort the data in an alphabetical order using the "Up Arrow" symbol for ascending alphabetical Order or the "Down Arrow" symbol for descending alphabetical order.
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/arrange.PNG?raw=true)

 ## Finding Out More Links
 Below the column headers and in the rows are object identifiers or symbols which are links to the "Report Pages". These identifiers also give a pop-up summary of the object.
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/object.PNG?raw=true)

 ## Report Pages
 The Report pages give you details of that particular data depending on what query that data was built upon. You can read more in the <a href="https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages">Report Pages Of The Intermine Documentation</a>
 ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Report.PNG?raw=true)


## Features Of The Result Table

1. Recent Queries: This is seen at the top left of the result table to show the templates that have been searched for and when each of the template in the recent query is clicked, it gives information about that particular template search. 
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/recent.PNG?raw=true)

2. Modification buttons: On the middle-top section of the webpage, you will buttons that enable you modify your template search and add more data to the results.
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/query.PNG?raw=true)
The functions of these buttons include: 

a. Add Columns: To add a new column header that gives data result based on the field name of that header.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/columns.PNG?raw=true) -->

b. Manage FIlter: To adjust the filter so that the data can be changed to your satifaction.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/filter.PNG?raw=true) -->

c. Manage Relationships: If you want your query to be required or optional, you can determine that in this section.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Relate.PNG?raw=true) -->

d. Save List: You can save your template search in the public lists for it to be viewed later if selected from the List section. Your query  can only be added to the public list if you sign up and login into that particular "Mine". You can edit the name you want your query to be called in this list thus creating your own data.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/save.PNG?raw=true) -->

e. Export: You can download your results with this button.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/export.PNG?raw=true) -->

f. Javascript: Developers can use this button to choose the programming language and alsoto download the source code of this result.
<!-- ![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/lang.PNG?raw=true) -->

g. Undo: You can click on this button to reverse all the changes you have made and remove all the query data you have added.

3. Enrichment
This section is found at the right part of the result table webpage. This section allows to enrich the data of your query by increasing or decreasing your "Max p-value", changing your "Test Correction" inputing your query data in "Filter Enrichment Results". You can also click on the default enrichment values provided instead of making your own query data yourself. Thus providing more information for your result table. Any enrichment that is clicked on adds a new template search to the previous searches on the "Recent Query" Section.
<a href="https://intermine.readthedocs.io/en/latest/embedding/list-widgets/enrichment-widgets/">You can find out how Enrichment is calculated here</a> 
![alt text](https://github.com/LizzyKate/training-portal/blob/lizzy/content/user-documentation/template-img/Enrichment.PNG?raw=true)




## TROUBLESHOOTING

No result found on my template search  - Why?

All templates should return results with the default  values provided, if you find a template that doesn’t, please contact  
<a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a>

If you provided your own values, it may mean that we don’t have the data you are looking for or if it is a complicated search with optional constraints, some of the required data might be there but not all of it resulting in no results.

If you have activated multiple optional constraints, it is often a good idea to turn these on individually to see if one in particular is causing the problem. By default adding a constraint means that the data MUST satisfy that constraint for the search to return results - see <a href="https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin">Outer joins</a> for more details.

Please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> if you require further attention.




{{< childpages >}}