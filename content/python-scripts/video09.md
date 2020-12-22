# video09

+++ title = "Tutorial 9" description = "" weight = 10 +++    


Welcome to the ninth tutorial in the InterMine python tutorial series! This tutorial will talk about how you can create and save lists in your account. You will need to provide your login information while creating a service object like in the previous tutorial.

You can either provide a list of identifiers \(for example, gene symbols\) and the InterMine Server will try to match them with objects in the database, or you can provide a query that specifies exactly what you want.

Here I use my username and password to show how it works. Don’t forget to enter your own login information when you try to run it.

We will look at three methods in this tutorial. Let’s say you want to upload a list of strings \(Gene Symbols\). We begin by declaring a python list variable, which I called symbols.

Note that you can use other identifiers, known in InterMine as secondary identifiers or DB identifiers, if you are more comfortable with that. So you can change symbols to \["CG2328","zen","rudimentary"\] or \["eve","FBgn0004053","rudimentary"\] - both of these lists work with FlyMine and contain the same three genes. InterMine would be able to resolve it for you, so long as it has this identifier set in its database.

To create a list in the InterMine server, you need to declare a list manager object. We then use the create\_list method as shown below. Remember to define a name for the list, otherwise the list will be lost once the session will be terminated.

delete\_lists method here delete the given lists from the webserver. create\_list has three parameters. content means the source of the identifiers for this list. Here the source is symbols we created before. list\_type means the type of objects to include in the list, for example “Gene” or “Protein”. Since this is a list of genes, of course we want to include Gene in this list. name is the list name of your choice, so here, the name is “my list”.

We will now look at how you can save a list from a query. Suppose that you want to extract only the information regarding the gene symbol “eve” stored in the previous list that we uploaded. You can do it as shown below. We create a query, restrict it to genes in the intermine list named “my list”, then add the constraint that symbol is eve, and then add a second intermine list named “my list 2” to store the query results.

If you visit BlueGenes or FlyMine.org and go to the lists page, then click on the view tab, you should be able to see the two lists you created.

Finally, let's say that you have a file with a list of gene identifiers stored on your machine which you want to upload as a list. Change the string stored to match the path location of your file. Uncomment the lines of code and run it. Files generally need to be plain text and have comma, \(,\) semicolon, \(;\) or new line separators between genes.

If you want to view the names of all the lists available on the InterMine server, use get\_all\_list\_names:

Here we can see the output.

In the next tutorial, we will talk about how you can perform enrichment calculations on lists that you have access to.

Thank you for watching!

