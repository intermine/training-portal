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

## [Regions Search ](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MSmZhKGwlzd16Z8Ca73/content/user-documentation/region-search#troubleshooting)

### 1. I have saved my genomic regions from a query - how do I upload them to the region search?

BlueGenes does not support uploading genomic regions directly from the results of an InterMine search into regions search. You first need to download the regions and then reformat them to one of the accepted formats. 

## [Lists](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/content/user-documentation/lists/lists#troubleshooting)

### 1. I am being told to upgrade my lists - what does this mean?

Every time we make a new release of an InterMine database, it is possible that some of the gene models have changed, which means that some of your identifiers might become outdated. For example, a gene may have been split; in this case, an identifier may now refer to more than one gene. Often a gene model is just updated, and the old identifier becomes a synonym while the gene is assigned a new identifier. When we make a new release, all of the identifiers present in your saved lists will be checked against the new database’s identifiers. When any discrepancies are found \(i.e. if any have now become synonyms or refer to more than one gene\), you will be asked what you want to do about these genes before using your list again. 

A message appears at the top of any page informing you that you have lists that need an update. To update your lists, you must be logged in to your user account. Within the Lists view page, lists that need to be updated will be shown first. The list upgrade system is the same as The Identifier Resolution page you see when you upload a list.

### 1. I have saved my genomic regions from a query - how do I upload them to the region search?

BlueGenes does not support uploading genomic regions directly from the results of an InterMine search into regions search. You first need to download the regions and then reformat them to one of the accepted formats. 

## [The Query Builder](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MSmZhKGwlzd16Z8Ca73/content/user-documentation/the-query-builder#troubleshooting)

### 1. Why do I keep getting “No results” for my search?

Sometimes your search gives “No results” because one part of your search does not yield results. If you have several constraints, try removing only one at a time to see if you will get results. Alternatively, toggle your constraints to an [outer join](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MRV1dETGFXxj_SCpAD8/content/user-documentation/the-query-builder#outer-joins) from your results to see if there is data fulfilling that constraint; you can check [Outer joins](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MRV1dETGFXxj_SCpAD8/content/user-documentation/the-query-builder#outer-joins) for more details. If you still need additional help, please [Contact Us](contact-us.md).

### 2. I am not sure how to start building a search; it looks hard!

Every template search can be displayed in the query builder. Try looking at some of the simple templates in the query builder and see how they have been constructed. Use this as a starting point to try changing a constraint or adjusting what is shown in the results table. If you need any help, please [Contact Us](contact-us.md).

To decide which class to select to begin building a query, think about the data you are trying to return. For example, suppose you want to know about the expression of a set of genes. In that case, you can start your query from Gene, where you can define which genes you are interested in and then navigate to the expression data, where you can determine what expression data you like to see. Similarly, you could construct the same query by defining the expression data. Expression data links to Genes, which allows you to add your gene constraints.

### 3. I can’t find the data I am looking for in the model browser!

The data browser is based on the sequence ontology and follows the logical relationships found in biological data. **For example, Exons are referenced from Gene and Protein domains are referenced from Protein**. Many additional classes and fields have been added that also follow logical biological relationships. So if you are looking for Gene expression data, you will find this referenced from Gene. For details of all the data sources loaded to see the **Data** tab. If you need additional help, please Contact Us.

### 4. I don’t understand what a field/class means.

Some fields have an information icon that provides an additional description of those fields. If you are unsure of a field’s contents, you can add it to your results and run the query. Most queries give results immediately, which allows you to adjust the columns you want to include in your results and fine-tune your query. It is also possible to do this from within the **Results Tables**. If you need additional help, please [Contact Us](contact-us.md). 

### 5. How do I navigate a class I have constrained without going through the model browser again?

Clicking on a class name in the right-hand Summary pane will open the model browser at that class.

