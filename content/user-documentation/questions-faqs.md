# Frequently Asked Questions

Welcome to our Frequently Asked Questions \(FAQs\) page. 

{% hint style="info" %}
Got a question? We want to help! If you have a question that isn't answered here, please [contact us](contact-us.md).
{% endhint %}

## [Template Searches](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/keyword-search)

### 1. My template returns no results - why?

All templates should return results with the default values provided. Please [Contact Us](contact-us.md) if you find any template that doesn’t.

* If you have entered your desired values and the template returns No Results in the results preview window, this means the data you are looking for is not available.
* For more complex searches with optional constraints, the way the search is constructed may affect the results - some of the required data might be missing resulting in no results. If you have activated multiple optional constraints, it is often a good idea to turn these On individually to see if one of them is causing the problem. By default adding a constraint means that the data **MUST** satisfy that constraint for the search to return results - take a look at [Outer Joins](https://flymine.readthedocs.io/en/latest/query-builder/Documentationquerybuilder.html#outerjoin) for more details about how constraints and joins can limit your results. 

## [Regions Search ](region-search.md)

### 1. I have saved my genomic regions from a query - how do I upload them to the region search?

BlueGenes does not support uploading genomic regions directly from the results of an InterMine search into regions search. You first need to download the regions, and then reformat them to one of the accepted formats. 

## [Lists](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/content/user-documentation/lists/lists)

### 1. I am being told to upgrade my lists - what does this mean?

Every time we make a new release of an InterMine database, it is possible that some of the gene models have changed, which means that some of your identifiers might become outdated. For example, a gene may have been split; in this case, an identifier may now refer to more than one gene. Often a gene model is just updated, and the old identifier becomes a synonym while the gene is assigned a new identifier. When we make a new release, all of the identifiers present in your saved lists will be checked against the new database’s identifiers. When any discrepancies are found \(i.e. if any have now become synonyms or refer to more than one gene\), you will be asked what you want to do about these genes before using your list again. 

A message appears at the top of any page informing you that you have lists that need an update. To update your lists, you must be logged in to your user account. Within the Lists view page, lists that need to be updated will be shown first. The list upgrade system is the same as The Identifier Resolution page you see when you upload a list.

