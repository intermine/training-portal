+++
title = "Tutorial 1"
description = ""
weight = 2
+++
{{< lead >}}
<br/>


Welcome to the first intermine python tutorial! In this tutorial, we will go through the basics of intermine python queries and how to write your first query. To get started, you would want to ‘pip install intermine’ in your terminal first. 

Let’s look at cells. We start by importing the service class from InterMine’s webservice module. Let’s click it.

Then let’s create a query object. The “new query” method can help us do this. Let’s click it.

A query object defines what we want from the intermine database. In this query object, we query the Flymine database to extract the symbol, primaryIdentifier and length of all genes. Then we can see the output.

Next, I’ll show you how to print the results of our query. In this cell, we use’ for row in query.rows(start = 0, size = 10) print(row)’ command to print the results. Size = 10 means it will print ten results. We can see the output.

The query has another way it could be written. We can see this cell. Let’s click it. Yes, it gives the same output.

Next, let’s try to write a new query which returns all organisms in the database. Let’s click it. It creates a new query object.

Then we select organism names. In this way, this object gets all organisms in the database.

If we want to add another column to our final output, we can use the add_view method. Let’s click it.

Then let’s try to print the results from the beginning. Of course, the size is too big. So we set size = 10. We can see the output, which is organisms’ information.

By default, the result will be sorted according to the first column you defined. We can use the addsort_order method of the query class to change the sorting order to another column. 

Then we reprint it. We can see this time the output is in the order of name.

In this tutorial, we learned how to get organisms from the database and how to set rows of output results. In the next video, I’ll show you how to add constraints to a query.

Thank you for watching!
