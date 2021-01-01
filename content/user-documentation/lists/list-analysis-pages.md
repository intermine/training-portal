# List analysis pages

## Overview

Every list has an associated list analysis page. A list analysis page is analogous to a gene report page and provides collated information about all the items in your list. If you upload a list you will be automatically taken to it’s list analysis page. To access the list analysis page from lists already in the database, go to the lists tab and click on the ‘View’ sub-tab. Clicking on a list name will display the analysis page. Remember, you must be logged in to view your own lists.

## The list summary

The list summary provides the main identifiers for the objects in your list. The list summary is a [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) and provides all the [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) functionality.

## Converting a list to another type

A list of objects can be converted to a related list of objects through the list analysis pages. For example, if you have a list of genes, you can convert this into the list of corresponding proteins or a list of all the exons or transcripts for that set of genes:

## Open another organisms MOD-intermine via the orthologues of your list

InterMine databases are available for Human, mouse, rat, zebrafish, fly, worm and yeast. See [the InterMOD project](http://intermod.intermine.org/) for more details. It is possible to link to one of these databases with the homologues of the list you are viewing:

## What does enrichment mean and how are the p-values calculated?

‘Enrichment’ means that the feature \(GO term, domain etc\) occurs for those genes more than would be expected by chance. It is calculated using the hypergeometric distribution which is described further in the [InterMine documentation](http://intermine.readthedocs.org/en/latest/embedding/list-widgets/enrichment-widgets/)

The InterMine enrichment widgets also provide the choice of three methods for multiple test correction - Bonferroni, Holm-Bonferroni and Benjamini Hochberg. These are also described further in the [InterMine documentation](http://intermine.readthedocs.org/en/latest/embedding/list-widgets/enrichment-widgets/)

## What does normalise by length mean?

The probability of a given set of genes being hit in a ChIP experiment is amongst other things proportional to their length – very long genes are much more likely to be randomly hit than very short genes are. This is an issue for some widgets – for example, if a given GO term \(such as gene expression regulation\) is associated with very long genes in general, these will be much more likely to be hit in a ChIP experiment than the ones belonging to a GO term with very short genes on average. The p-values should be scaled accordingly to take this into account. There are a number of different implementations of corrections, we have chosen the simplest one. The algorithm was developed by Taher and Ovcharenko \(2009\) for correcting GO enrichment. Corrected probability of observing a given GO term is equal to the original GO probability times the correction coefficient CCGO defined for each GO term.

The correction coefficient is described in the [InterMine documentation](http://intermine.readthedocs.org/en/latest/embedding/list-widgets/enrichment-widgets/)

## Template results on list analysis pages

List analysis pages include a set of [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches). These are found at the bottom of the list analysis page and are a set of searches that are automatically run on your list so you can immediately access the results. The results are presented in [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) and provide the full functionality of [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables).

