+++
title = "Tutorial 10"
description = ""
weight = 11
+++
{{< lead >}}
<br/>


Welcome to the tenth tutorial in the InterMine python tutorial series! This tutorial will talk about how you can perform enrichment calculations on lists that you have access to.

‘Enrichment’ means that the feature (GO term, domain) occurs for those genes more than would be expected by chance. It is calculated using the hypergeometric distribution which is described further in the InterMine documentation

Enrichment widgets are useful to find items such as GO Terms or publications which are associated with your gene list more than would be expected by chance.

The InterMine service has various widgets that can perform different functions. These widgets are stored in a dictionary in the Service class. To view all the widgets for an InterMine we can use service.widgets.

Here we can see the output

If you want to view only those widgets that are related to enrichment, you can filter based on the widget type. Here we use a python loop to print all the enrichment related widgets.

Now we can get a list on which we want to perform the analysis using the list manager. The get_list method here returns a list from the service by name, if it exists. 

To perform any enrichment analysis on the list, we can use the calculate_enrichment method. The arguments include the type of enrichment (this has to be one of the widget types shown in the widget list above) and the maximum p value to show. Here we store the results in a variable named “r”. 

Then we iterate through r and view the results. 

In this output, we can see a set of publications for which this gene set is enriched - that is, genes that are over-represented in the publications

In the next tutorial, we will talk about how you can combine two lists easily in InterMine.

Thank you for watching!
