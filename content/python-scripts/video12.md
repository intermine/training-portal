+++
title = "Tutorial 12"
description = ""
weight = 13
+++
{{< lead >}}
<br/>


Welcome to the twelfth tutorial in the InterMine python tutorial series! This tutorial will cover some more functionalities of a query. Queries are the basis of all research in InterMine. Being able to manage them more effectively is always useful.

First, we create a query object like we saw earlier, and select the gene symbol and organism as the views.

Let’s say that the query is not as simple as a strict cumulative filter and the user wants combinations of constraints. For example, the user wants all genes such that the gene symbol is either ‘eve’ or ‘zen’. This can be incorporated in the following way using set_logic and the pipe operator | to signify OR

Here we can see the output. It returns two symbols which are exactly ‘eve’ and ’zen’.

The query results can be converted into a dictionary using row_to_d() method in the following way: 

Similarly, row.to_l() can be used for conversion of the results into a list.

count() can be used to print the total number of rows in a query: 

So here the result is 2.

to_xml() can be used to return a readable XML serialisation of the query. This can also be copy/pasted and imported into the InterMine user interface. 

clear_view() can be used to clear the output column list, which deletes all entries currently in the view list. It is contrary to add_view().


In these ways, queries can be utilized to a greater extent and produce more fruitful results. 

Next tutorial will tell you about the Query Manager and how it can be utilised to make better use of queries.

Thank you for watching!
