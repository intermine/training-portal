# video05

+++ title = "Tutorial 5" description = "" weight = 6 +++    


Welcome to the fifth tutorial in the InterMine python tutorial series! This tutorial will talk about dealing with the results of our query. You can either store the results into a file \(using a library like csv\) or you can process the results immediately after you extract them.

Now we write a short query for genes, and add all views for publications associated with that gene, then explore the results.

Here we constrain the query to show the gene “zen” in fruit flies.

Once we have added our constraints and views, we are ready to look at the results. The results can be accessed in either a dictionary form, or a list, or a ResultRow object, or a list of strings \(CSV or TSV\).

Here we can see the output

And here we print all the genes.

You may have wondered what the difference was - and actually, iterating through query.results \(we set rows = “rr” here\) and iterating through query.rows\(\) are equivalent. Feel free to use whichever you feel comfortable with.

Let’s say you want to extract column 2 and 3 in this example.

We use the command print\(gene\[1\], gene\[2\]\) here and we can see the output. \(because the count starts from 0, gene\[1\] means the second gene and gene\[2\] means the third gene\)

If we want to print only those rows where publications.doi is not None then we can add an if condition as shown below.

We use the command if row\[1\] != None\(!= means not equals to\) here to achieve this goal.

Then we can see the output.

You can pass two more parameters, start and size, while passing query.results\(\). Start represents the row number that you want to start processing from. By default this is set to 0 \(the first row\). Size represents the number of rows that you want to print. Let’s say we want to print row 10 and 11 only.

So here we set size equals to 2, and start equals to 10. We can see the output is only two rows

If you prefer dealing with lists of strings, for example csv and tsv objects, you can use them too. First, we need to import the csv library. Then we create a csv reader object. This has been shown below. query.results\(row = “csv”\) means that this object reads query.results. delimiter refers to the character used to separate values \(or fields\) in the CSV file. Here we set the character to comma. quotechar refers to the single character string that will be used to quote values if special characters \(like delimiter\) appears inside the field. Here this single character is quote.

Here we print the first row, row\[0\]. We can see the output.

The last thing that we look at in this tutorial is the summarize method. This method is useful when we want some basic statistics regarding a particular column.

Here we look at the statistics of the length of genes present in the list of the most enriched genes in the adult fly brain.

First we create a query.

Then we add views to show the gene and organism for each gene, and constraint the query to be in the list called “PL FlyAtlas\_brain\_top”.

We then print out the first 10 rows of results.

Next we can look at the summary of the length of each gene. This contains some useful information such as the average length and the maximum and minimum length.

We can see the output.

Also, we can print genes’ id.

In the next tutorial we will focus on further management of results.

Thank you for watching!

