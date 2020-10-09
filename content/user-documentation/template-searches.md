+++
title = "Template Searches"
description = ""
weight = 3
+++


### What is a template search
A template search is a pre-defined query that we have created for you. A template search allows you to search the database without having to construct your own query or understand the underlying data structure. A library of template searches covering the full range of data is available.

A template search consists of a simple form with one or more options for you to enter or select. Default values are always provided so you can immediately run them and see if they return the data you are after.

Each template has a short name and a longer description. We provide a short name so you can quickly scan the available searches and find the one that you need. The longer description will provide you with more details and any limitations to the values you can enter.

### Steps to finding a template search
We use <a href="https://www.flymine.org/flymine/begin.do">Flymine</a> as an example.
1. Click on the templates tab in the main menu bar.

<img src="https://i.imgur.com/bp7Vp3Q.png">
<br/>
<br/>

2. Filter the list using either keywords or data categories

<img src="https://i.imgur.com/0cex0ax.png" >
<br/>

### Can’t find what you want?
If you can’t find a template search that you want or if there is one available but it doesn’t quite return everything you are after please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us.</a>  Template searches can be created or modified and made available to you immediately, providing the data is available in the database. 

### Running a template search
1. Once you have choosen your intended search, you will be provided with a form with one or more variables to set
2. Enter a value,  in this case there is an auto-suggest function. **OR**
3. Choose choose from the drop-down lists if provided
4. Some constraints are optional: you can choose whether to filter on the pathway data source by turning the constraints on or off
5. Click **Show Results** to run the search.

<img src="https://i.imgur.com/nD1HyHA.png">
<br/>
<br/>

### Running a template search with one of my lists or a public list
1. Log-in so that your own lists can be viewed. 
2. Every template can be run on relevant Lists of objects - if you have lists of the correct type (e.g. a list of genes) or if there is a suitable public list, you will be able to select the one you require from a drop-down list. 
3.  select the checkbox to access this.

<img src="https://i.imgur.com/DnVYso5.png">
<br/>
<br/>

### Understanding your results
Your template will return a results tables. As well as displaying your results, the results tables are a powerful analysis tool as well. See the <a href="https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables">Results Tables</a> for more details and for information on how to save or download your results.

### Modifying a template search
Sometimes you may find a template does not return everything you want in your results. Templates can also be a good starting point for building more complex searches. To modify a template using the The Query Builder:

1. Click on the **Edit query** (4) button from the image above to display the template in the query builder. You need to understand how to use the query builder to modify your template - please see the <a href="https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#querybuilder">The Query Builder documentation.</a> Remember, if you do not want to invest the time learning how to use the query builder you can <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> the InterMine team who will be happy to help construct the search you require.
2. Edit from image below and when done click **Show results**

<img src="https://i.imgur.com/RtjozHu.png">
<br/>
<br/>

### Building your own template search
Coming soon……

### TroubleShooting
My template returns no results - why?

All templates should return results with the default values provided (please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> if you find one that doesn’t). If you have provided your own values, in most cases it will mean we don’t have the data you are looking for. In some cases, however, particularly for more complicated searches with optional constraints, it may be because of the way the search is constructed - some of the required data may be there but not all of it, resulting in no results. If you have activated multiple optional constraints, it is often a good idea to turn these on individually to see if one in particular is causing the problem. By default adding a constraint means that the data MUST satisfy that constraint for the search to return results - see <a href="https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin">Outer joins</a> for more details. Please <a href="https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact">Contact Us</a> if you require further assistance.



{{< childpages >}}