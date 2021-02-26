# Getting Started

This quick guide will walk you through the key functions of the InterMine - BlueGenes application UI. 

You can use this guide to:

* Take a general overview of the BlueGenes interface.
* Take a closer look at the key sections of the homepage.
* Understand the basics of using InterMine and its main sections 

{% hint style="info" %}
This concise overview is geared mainly for new users. For more information about a particular topic, see the relevant section in the documentation. 
{% endhint %}

### The Basics

The InterMine query interface provides various ways to view and analyse data. Whether you are looking at a single gene, a list of genes, transcription factor binding sites, or protein interactions, it is useful to understand the following terminology to understand the interface. 

Intermine allows you to work with **single items \(objects\)** and **multiple items \(lists\)**:

* **Object:** A single item in the database. This can be anything, a gene, protein or binding site.
* **List:** Multiple items of the same type. For example, a list of genes or a list of proteins.

{% hint style="info" %}
This user guide demonstrates the workflow in all sections using HumanMine as a reference.
{% endhint %}

### Homepage

Below is a quick description of different sections and their associated functionalities of the BlueGenes homepage: 

![The BlueGenes UI Homepage](../../.gitbook/assets/homepage%20%282%29.png)

* \*\*\*\*[**Home**](http://bluegenes.apps.intermine.org/humanmine): the homepage of the interface offers a search feature for any term, access to popular queries, documentation, the InterMine blog, external tools, and more.
* \*\*\*\*[**Upload**](lists/upload-a-list.md): to upload a new list as a free text or from an existing file. 
* \*\*\*\*[**Lists**](lists/): a list in InterMine refers to multiple items of the same type - for example, a list of genes or a list of binding sites. 
* \*\*\*\*[**Templates**](template-search.md): a pre-defined query which offers a simple form with one or more variables for you to define; defaults are always provided so you can see exactly how the template works.
* \*\*\*\*[**Regions**](region-search.md): a tool for looking at genomic regions and the features they contain, allowing you to upload a set of regions and search for features mapped to these regions.
* \*\*\*\*[**Query Builder**](the-query-builder.md): an advanced query building tool - you can use this to construct your own searches. You can even turn them into your own template searches.
* \*\*\*\*[**Keyword Search**](keyword-search.md): a search box appears on the menu bar of all pages and the home page. You can search for any identifier, name, symbol or keyword.
* \*\*\*\*[**HumanMine**](http://bluegenes.apps.intermine.org/humanmine): an integrated database of Homo sapiens genomic data. You can change HumanMine to a different InterMine instance. Check this [registry](http://registry.intermine.org/) for available instances.   
* \*\*\*\*[**Account**](account.md): your personal InterMine account where you can manage your lists, queries, templates, etc.  

### InterMine search tools

* [Keyword Search](keyword-search.md)
* [Template Searches](template-search.md)
* [The Query Builder](the-query-builder.md)
* [Regions Search](region-search.md)

### Viewing search results

To view data resulting from these searches, intermine provides the following interfaces:

* [Report Pages](report-pages.md):  a report page can be viewed for any object, such as gene or protein, allowing you to view all information available for that particular object and providing links to related objects. 
* [List analysis pages](lists/list-analysis-pages.md): every list has an associated list analysis page. A list analysis page is analogous to a gene report page and provides collated information about all the items in your list.
* [Results Tables](results-tables.md): results tables are not only for displaying your search results but are also powerful analysis tools, allowing you to summarise, filter, add or remove columns, create lists and download data.
* [Regions Search Results](region-search.md): regions search provides results in a tabular format. The resulting table displays each of your regions in turn with all features found and their genomic location. 

### How everything links together

Although the above tools and interfaces are described separately; they all interact together in various ways. 

For example, you could run [Template Searches](template-search.md) to find all genes regulated by a specific transcription factor. Using the resulting [Results Table](results-tables.md), you could [Upload a list](lists/upload-a-list.md) of these regulated genes. This list could then be analysed using the [List analysis pages](lists/list-analysis-pages.md). You could also run further [Template Searches ](template-search.md)using this list as the input.

Alternatively, you may start by [Uploading a list](lists/upload-a-list.md) of genes. Through the graphs and tables provided on the [List analysis pages](lists/list-analysis-pages.md), you may filter this list according to particular criteria \(e.g. expressed in the brain\) to create a smaller list. You may then run a series of [Template Searches](template-search.md) or build your own queries using [The Query Builder](the-query-builder.md) to find out more about this set of genes. You may also browse the information available on the [Report Pages](report-pages.md) for any genes that may seem interesting to you! 

Likewise, you may start by entering a gene identifier for a gene you have picked up in an experiment into the [Keyword Search](keyword-search.md) box and browse all the information for this gene on its [Report Pages](report-pages.md). From here, you learn that this gene has orthologues in fish, mouse and rat. You click the link for the mouse orthologue and, this takes you to the report page for this orthologous gene in a related intermine, MouseMine, and so on.

