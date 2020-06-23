+++
title = "Tutorial 3"
description = ""
weight = 4
+++
{{< lead >}}
<br/>


Welcome to the third tutorial in the InterMine python tutorial series! In the previous tutorial, we learned about adding constraints to our query so that we could filter the results. In this tutorial we will take a look at some more different types of constraints.

First, let’s create a query object like we saw earlier.

The first type of constraint we will look at is Unary Constraint. A unary constraint is one that does not take any value but can be used to check if a particular attribute is absent or present. The unary constraints are IS NULL and IS NOT NULL. Let’s look at a small example.

We add constraint IS NOT NULL here. This means that primaryIdentifier must have some value.

Let’s click it and see the output.

The next type of constraint is a Binary Constraint. This refers to constraints that take a value. Binary constraints are the largest group of constraints. Binary operators are =, <=, >=, <, >, and !=.

Let’s look at this example. We add the constraint length >= 12000 here. That means genes’ length should be longer than 12000 in this query object.

We can see the output here.

Now we look at Ternary constraints. A ternary constraint is a type of constraint which has one required value and one optional value. InterMine currently supports only one such type of operator, LOOKUP, which searches through all the fields in a particular class for the value specified by the user. 

In the example below, it will search through the entire gene class to find if any of the fields has an occurance of “zen”. The advantage of this is that you do not need to remember if zen is a symbol or a name or a primaryIdentifier. However, this may lead to ambiguous results and so you can use the optional extra_value parameter to limit the search to the type of object - for example, you might want to limit it by organism.

We can see in this example the constraint is Gene LOOKUP zen IN D.melanogaster.

Then we can see the output.

The next constraint type we will look at is Multi-Value constraints. This allows the constraint to take multiple values. Two operators that are allowed are ONE OF and NONE OF.

Here, we set the constraint is Gene.symbol NONE OF [‘zen’,’eve’].

We can see the output now.

Let’s look at List Constraints now. List Constraints allow users to create a named list of objects and then use the operators IN and NOT IN to use those named lists in queries. 
Let’s show it in this example.

Now the constraint is GENE IN the list  PL FlyAtlas_brain_top.

We can see the output.


Next, let’s look at Sub-Class constraints. These constraints allow you to specify a sub-class of a class to constrain a path to. 

In this example, the constraint now is Gene.ontologyAnnotations IS A GOAnnotation

We can see the output.

Next, we look at Loop Constraints. Loop constraints assert that two paths refer to the same object. The valid operators are IS and IS NOT. The Path and LoopPath in such a query must always be a Class(for example - Gene is a valid path). Also, the operators IS and IS NOT map to “=” and “!=”. The example below is an application of a Loop Constraint.

Firstly, we add list constraints here.

Then we add a loop constraint.

Then we can see the output.

Finally, let’s look at range constraints. They are used for testing where a value lies relative to a set of ranges. These constraints require that the value of the path they constrain should lie in relationship to the set of values passed according to the specific operator. Valid operators are OVERLAPS, DOES NOT OVERLAP, WITHIN, OUTSIDE, CONTAINS and DOES NOT CONTAIN. Here is an example of Range Constraint.

Here we set the constraint OVERLAPS this range. 

Now we can see the output.

This tutorial summed up some of the important constraint types. In the next tutorial we will look at some of the other features of a query.

Thank you for watching!