# Getting Started

Welcome to InterMine! This quick guide will walk you through the features and functions of the InterMine - BlueGenes UI. 

You can use this guide to:

* Take a general overview of the BlueGenes interface.
* Explore the main sections of the homepage
* Understand the basics of using InterMine and its main features

{% hint style="info" %}
This concise overview is geared mainly for new users. For more information about a particular topic, see the relevant section in the documentation. 
{% endhint %}

### The Basics

The InterMine query interface provides various ways to view and analyse data. Whether you are looking at a single gene, a list of genes, transcription factor binding sites, or protein interactions, it is useful to understand the following terminology to understand the interface. 

Intermine allows you to work with **single items \(objects\)** and **multiple items \(lists\)**:

* **Object:** A single item in the database. This can be anything, a gene, protein or binding site.
* **List:** Multiple items of the same type. For example, a list of genes or a list of proteins.

### Homepage sections

Below is a quick description of different sections in the BlueGenes homepage

![The BlueGenes UI Homepage](../../.gitbook/assets/homepage.png)

* **Home**: the main page of the interface, which offers search for any term, access to popular queries, documentation, the InterMine blog, external tools, and more.  
* **Upload**: to upload a new list as a free text or from an existing file. 
* **Lists**: A list in InterMine refers to multiple items of the same type - for example, a list of genes or a list of binding sites. 
* \*\*\*\*[**Templates**](keyword-search.md): A pre-defined query which offers a simple form with one or more variables for you to define; defaults are always provided so you can see exactly how the template works.
* **Regions**: A tool for looking at genomic regions and the features they contain. Allows you to upload a set of regions and search for features mapped to these regions.
* **Query Builder**: An advanced query building tool - you can use this to construct your own searches. You can even turn them into your own template searches.
* **Keyword Search**: A simple search box for looking up names, symbols identifiers or keywords.
* **HumanMine**: An integrated database of Homo sapiens genomic data. You can change HumanMine to a different InterMine instance. Check this [registry](http://registry.intermine.org/) for available instances.   
* **Account - MyMine**: MyMine is your personal InterMine account where you can manage your lists, queries, templates etc.  

### InterMine search tools

* [Keyword Search](https://flymine.readthedocs.io/en/latest/quick-search/Documentationquicksearch.html#quicksearch): A simple search box for looking up names, symbols identifiers or keywords.
* [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches): A pre-defined search which provides a simple form with one or more variables for you to define \(defaults are always provided so you can see exactly what the template does\).
* [The Query Builder](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#querybuilder): An advanced query building tool - you can use this to construct your own searches. You can even turn them into your own template searches.
* [Region Search](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearch): A tool for looking at genomic regions and the features they contain. Allows you to upload a set of regions and search for features mapped to these regions.

### Viewing search results

To view data resulting from these searches, intermine provides the following interfaces:

* [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages)
* [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage)
* [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables)
* [Region Search Results](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearchresults)

### How everything links together:

Although the above tools and interfaces are described separately here, they do of course, all interact with each other in various ways. For example, you could run [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) to find all genes regulated by a specific transcription factor. From the resulting results table, you could [Upload a list](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listupload) of these regulated genes. This list could then be analysed using the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage). You could also run further [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) using this list as the input.

Alternatively, you may start by [Upload a list](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listupload) of genes. Through the graphs and tables provided on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage), you may filter this set according to some criteria \(e.g. expressed in the brain\) to create a smaller list. You may then run a series of [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) or build your own queries using [The Query Builder](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#querybuilder) to find out more about this set of genes. You may also browse the information available on the [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages) for those genes that look most interesting.

You may start by entering a gene identifier for a gene you have picked up in an experiment into the [Keyword Search](https://flymine.readthedocs.io/en/latest/quick-search/Documentationquicksearch.html#quicksearch) box and browsing all the information for this gene on its [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages). From here, you learn that this gene has orthologues in fish, mouse and rat. You click the link for the mouse orthologue and, this takes you to the report page for this orthologous gene in a related intermine, MouseMine, and so on.

A set of worked use-cases is available in the [cookbook](https://flymine.readthedocs.io/en/latest/cookbook/index.html).

