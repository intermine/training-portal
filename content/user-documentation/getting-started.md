# Getting Started

A powerful open source data warehouse system that allows users to integrate diverse data sources with a minimal effort, providing powerful web-services and an elegant web-application with minimal configuration. 

### General Overview

This page is an overview of the InterMine - Bluegenes user interface.

The InterMine query interface provides a variety of ways in which you can view and analyse data, whether you are looking at a single gene, a list of over 1000 genes, transcription factor binding sites or protein interactions, for example. To understand the interface it is useful to understand the following terminology:

Intermine allows you to work with **single items \(objects\)** and **multiple items \(lists\)**:

**Object:** A single item in the database \(this can be anything, a gene, protein or binding site for example\).

**List:** Multiple items of the same type. For example, a list of genes or a list of proteins.

InterMine has four search tools as follows:

* [Keyword Search](https://flymine.readthedocs.io/en/latest/quick-search/Documentationquicksearch.html#quicksearch): A simple search box for looking up names, symbols identifiers or keywords.
* [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches): A pre-defined search which provides a simple form with one or more variables for you to define \(defaults are always provided so you can see exactly what the template does\).
* [The Query Builder](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#querybuilder): An advanced query building tool - you can use this to construct your own searches. You can even turn them into your own template searches.
* [Region Search](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearch): A tool for looking at genomic regions and the features they contain. Allows you to upload a set of regions and search for features mapped to these regions.

To view data resulting from these searches, intermine provides the following interfaces:

* [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages)
* [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage)
* [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables)
* [Region Search Results](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearchresults)

How everything links together:

Although the above tools and interfaces are described separately here, they do of course all interact with each other in various ways. For example, you could run [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) to find all genes regulated by a specific transcription factor. From the resulting results table, you could [Upload a list](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listupload) of these regulated genes. This list could then be analysed using the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage). You could also run further [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) using this list as the input.

Alternatively, you may start by [Upload a list](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listupload) of genes. Through the graphs and tables provided on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage), you may filter this set according to some criteria \(eg expressed in the brain\) to create a smaller list. You may then run a series of [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) or build your own queries using [The Query Builder](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#querybuilder) to find out more about this set of genes. You may also browse the information available on the [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages) for those genes that look most interesting.

You may start by entering a gene identifier for a gene you have picked up in an experiment into the [Keyword Search](https://flymine.readthedocs.io/en/latest/quick-search/Documentationquicksearch.html#quicksearch) box and browsing all the information for this gene on its [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages). From here you learn that this gene has orthologues in fish, mouse and rat. You click the link for the mouse orthologue and this takes you to the report page for this orthologous gene in a related intermine, MouseMine, and so on.

A set of worked use-cases is available in the [cookbook](https://flymine.readthedocs.io/en/latest/cookbook/index.html).

