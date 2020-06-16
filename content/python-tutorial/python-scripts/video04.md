+++
title = "Tutorial 4"
description = ""
weight = 5
+++
{{< lead >}}
<br/>


Welcome to the fourth tutorial in the InterMine python tutorial series! In the previous tutorials we learned about the basic backbone of a query - views and constraints. This short tutorial will talk about another feature of an InterMine query - Outer and Inner Joins.

When we add a path to a query, even if it is in the view, then by default there is a constraint involved. Our query will consist of only those records that have information in the fields or attributes that are described by the path.

Here, we’ll try to get genes involved in a biosynthetic process and any publications on them. If a particular gene has publication information available, then we want to view the general information about that gene.

By default, InterMine is designed to give you an Inner Join, which basically means that no partial matches will be part of the result. However, for the example we are discussing here, we would require something known as an Outer Join. An outer Join on Gene.publications would help in solving the problem for us.

Here is a comparison table of Inner Join and Outer Join:





| Inner Join | Outer Join |
| -------- | -------- |
|  default behavior        |   optional behavior       |
|implicitly constrains the values of that path to be non-null          |allows null values in the joined path          |
|no data will be returned if any one gene has not matched attributes described by the path     |query will continue even if some genes don’t have matched attributes described by the path     |

<br/>

Screenshot of the same query with Inner Join and Outer Join:

#### With Outer Join:

<img src="https://i.imgur.com/av7Jggf.png" width="900" height="400" />


#### With Inner Join:

<img src="https://i.imgur.com/vXuoN3Q.png" width="900" height="600" />

*PS: in the first second screenshot, results for 0610009B22Rik takes up three rows, which is the same as the SINGLE row with three publications in the second screenshot.*


Let’s start by creating a new query object like we saw earlier. We're selecting the primaryIdentifier and symbol for each gene, as well as the year, first author, and title of any associated publications.

Here we add the constraint like this, which constrains ontology terms to be any term that contains “biosynthetic process”. The *s in the constraint are a wildcard, meaning that any additional text can come before or after the phrase “biosynthetic process”. 

Then, we add an outer join using the query.outerjoin method, asserting that all genes should be returned, and if publication information is available we will return it as well.

Here we can see the output.

Another query feature that InterMine has is the ability to define shorter column names. This can be done using the add_path_description method.

This helps us when we want to print our tables into a file and want the column names to be in a readable format. 

In this example, we use Ontology Term to represent ontologyAnnotations.ontologyTerm and Pub. to represent publications.

In the next tutorial, we will look at dealing with the results that are returned by our queries.

Thank you for watching!