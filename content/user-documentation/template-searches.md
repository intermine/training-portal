+++
title = "Template Searches"
description = ""
weight = 6
+++
{{< lead >}}


##### _What is a template search_
----
<div class="text-justify">
<p>Template searches are pre-defined queries that have been created and are ready
to use. They allow users to search the database without constructing their
queries from scratch or understanding the underlying data structure. A library
of template searches covering a full range of data is available.</p>
<p>A template search has a simple form with one or more entry fields.
Users can fill in these fields or select a value from the available options.
Each template uses default values for all required fields, allowing users to
immediately run the query and view whether it returns the data they want.</p>

Each template has a short name and an extended description underneath.
The title helps users to scan available searches and find the one they
need quickly. The narrative provides users with further details and mentions
any restrictions on the values users can enter.<br/>

To access the template library, click on the Templates tab in the main menu bar.


<p align="center">
  <img src="https://i.imgur.com/bKsRSsb.png" class ="shadow" alt="template tab"
  width=90% height=90% />
</p>
<br/>

##### _Finding the template search that you want_
----
There is a long list of predefined searches, and checking all available templates can be time-consuming. So, to help users find the template they want, they can filter the list either by keyword/description or by data category.

<p align="center">
<img src="https://i.imgur.com/rbI8FGw.png" class ="shadow" alt="filter by term or category"
width=90% height=90% />
</p>

If you are not sure about which category to use as a filter, category tags are shown at the bottom right corner of each template preview.   
<p align="center">
<img src="https://i.imgur.com/y2FKjxO.png" class ="shadow" alt="category tags"
width=90% height=90% />
</p>
<br/>

##### _Can’t find what you want - let us know!_
----
If you can’t find a template search that you want or there is one available that doesn’t entirely return everything you need, please do not hesitate to reach out. We can create a custom template or modify an existing one and make it available to you immediately, assuming the data is available in the database. Let us know using the [Contact Us](https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact) form found on all InterMine pages or send us an email at support@flymine.org.

##### _Running a template search_
----
A template search provides users with a fillable form with one or more fields to set. Some may require entering a value; others have a set of available choices in a drop-down list. Some templates offer optional search constraints that users can turn on or off as desired. Once everything looks good, the user can click **view >>** to further expand the template and view the results preview and constraints window.
<p align="center">
<img src="https://i.imgur.com/buzvPow.png" class ="shadow" alt="preview"
width=90% height=90% />
</p>

To see all of the search results, users can click **view rows**
<p align="center">
<img src="https://i.imgur.com/s0rtEjl.png" class ="shadow" alt="view rows window"
width=90% height=90% />
</p>
<br/>

<p align="center">
<img src="https://i.imgur.com/fV91PQg.png" class ="shadow" alt="results table"
width=90% height=90% />
</p>


##### _How do I run a template search with one of my lists or a public list_
----
First, remember to **log in** so that you can view and use your saved lists. Users can run templates to search for a keyword in relevant [Lists](https://flymine.readthedocs.io/en/latest/lists/overview/Documentationlists.html#overview) of objects by selecting the **In List** option.

<p align="center">
<img src="https://i.imgur.com/XDJ0Q2L.png" class ="shadow" alt="in list option"
width=90% height=90% />
</p>

If a user has a list of the correct type (e.g. a list of genes) or a public one that matches their needs exists, they can choose their preferred list from the shown drop-down set.

<p align="center">
<img src="https://i.imgur.com/ooLSAzD.png" class ="shadow" alt="choosing a list"
width=90% height=90% />
</p>


##### _Understanding your results_
----
The template search returns results in a tabular format. Besides displaying query results, results tables are also a powerful analysis tool. Check the [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) section for more details on how to save or download search results.

##### _Modifying a template search_
----

Still under construction...
<br/>

##### _Building your own template search_
----
 Coming Soon...
 <br/>

##### _Troubleshooting_
----
**Q: Why don’t I see any results after running a template search?** <br/>

**A:** All templates should return results with the default values provided. Please [Contact Us](https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact) if you find any template that doesn’t.

* If you have entered your desired values and the template returns No Results in the results preview window, meaning the data you are looking for is not available.
* For more complex searches with optional constraints, the way the search is constructed may affect the results - some of the required data might be missing resulting in no results. If you have activated multiple optional constraints, it is often a good idea to turn these on individually to see if one of them is causing the problem. By default adding a constraint means that the data MUST satisfy that constraint for the search to return results - take a look at [Outer Joins](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin) for more details. Please [Contact Us](https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact) if you require further assistance.






</div>
