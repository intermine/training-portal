# video06

+++ title = "Tutorial 6" description = "" weight = 7 +++    


Welcome to the sixth tutorial in the InterMine python tutorial series! In the previous tutorials we learned how to add filters to limit the query results. However, it is often useful to view the results without filters. This tutorial will show you how to process, sort, and analyse the query results.

Usually, we begin by creating a query object. Our example for this tutorial is going to be related to gene expression, represented in InterMine by the RNA Sequence Result class. Let’s select the result score, expression level, and associated gene as our views.

Then we sort the results in descending order of their expression score.

Now we print the first ten rows.

Note that we have not added any constraints so we have extracted all the possible results.

Now let’s say that we want to sort all the results into three different maps, which we can also call dictionaries. Results with an expressionScore of greater than 25 go into the “high” map, the ones with an expression score greater than 10 but less than 25 into the “medium”, and all the remaining ones into a separate map for low result scores.

We begin by declaring these three dictionaries. high\_dict, medium\_dict, and low\_dict.

Here we add three map conditions to sort the results into each of our three maps

Then we print items stored in high\_dict. We can see the output is quite long.

We can calculate the average score of items with scores over 1000, by adding all scores together and dividing by the number of scores over 1000.

Here we can see the result is around 3018.

If you change your mind about the constraints, you can simply change the “if” condition.

In the next tutorial, we will look at templates, which are like pre-prepared queries you can easily re-use.

Thank you for watching!

