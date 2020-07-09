+++
title = "Tutorial 2"
description = ""
weight = 3
+++
{{< lead >}}
<br/>


Welcome to the second tutorial in the InterMine python tutorial series! In the previous tutorial we learned how to select the output columns of choice. In this tutorial, we’ll look at adding constraints to our queries to filter the results.

Let’s start with creating a service and query object, like we saw earlier. 

If we want to view all the possible output columns at once, we can pass “*” as a parameter to the select function like this.

If we want to add a constraint to our query, we can use the add_constraint method available in the query class.

For example, we can add the constraint “genus” “=” “Drosophila” In this way, we gives the constraint Organism.genius equals to Drosophila.

Now we can print the results of our query. In this cell, we don’t set limits to output rows. Let’s click it. We can see the output is quite long.

Next, we are going to change the query a little bit. Let’s say we want to extract all the publication information about Drosophilids that have been published since 2010. Let’s click it.

Since we want to get all the information related to each publication, we will add publications dot star as our parameter.

We can add constraints to it. Firstly we want to limit our search to only Drosophilids. Secondly we want to extract only those publications that were published in or after 2010. We use bigger or equals to here. Let’s click it. 

Similarly, we can print the result while limiting the size, and we can see the output.

Now, let’s look at another query. It runs similarly as before.

When querying the database using consecutive add_constraint methods, by default the constraints are “and”. For example, a particular instance will be part of the final result only if it satisfies all the constraints. Here, the constraints are organism.genius = Drosophila and organism.species is one of the two species.  

After we click this cell, we can see the output.

However, we have the option to use “or”.  We create a new query object to show this.

In this cell, we set this constraint to A, this constraint to B, this constraint to C, this constraint to D. 

After we use the set_logic method, the constraints now are A and (B or C) and D.

Similarly, we can print the results.

In the next tutorial, I’ll introduce more about constraints. 

Thank you for watching!
