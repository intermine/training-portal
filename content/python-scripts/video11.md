+++
title = "Tutorial 11"
description = ""
weight = 12
+++
{{< lead >}}
<br/>


Welcome to the eleventh tutorial in the InterMine python tutorial series! This tutorial will talk about how you can combine two lists easily in InterMine.

Like previous tutorials, this tutorial will require you to login into your InterMine account so that the lists that you will combine can be saved. 

To make things easier, I use a test account here. Don’t forget to enter your username and password, execute it and then proceed with the rest of the tutorial. 

We begin by declaring a list manager object which will help us in combining various lists together.

Let's say that you want to combine all the most enriched genes in the adult Fly brain and in the adult Fly hindgut. These are present as two separate lists currently on Flymine. So we begin by extracting both the lists first, storing them in variables called l1 and l2.

We use get_list method here. This method returns a list from the service by name.

There are a couple of ways by which you combine the two lists, for example, union of the two lists. 

The first method is shown below - using the addition operator automatically combines both the lists. 

Here we delete the list with the name “combination-1” in case there is already a list named combination-1 on the server which will cause an error. Then we set the name of variable l3 to “combination-1”.

Then we can print all genes in l3.

Here we can see the output

The second way of combining two lists is to first declare a Python List object with the lists that you want to combine. I've called this temporary list "y". You can then use the union method present in list manager to take the set union and give a name to the list in one step. This has been shown below. 

Similarly, if you want to find the intersection of two lists, you can use the intersect method that is present in the list manager class. You can combine lists and queries in the same way. 

Next tutorial will cover some more functionalities of a query. 

Thank you for watching!

