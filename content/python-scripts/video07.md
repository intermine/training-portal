# video07

+++ title = "Tutorial 7" description = "" weight = 8 +++    


In this tutorial we will look at templates, which are like pre-prepared queries you can easily re-use. Templates can do everything that a query can do. Everything that you can do with a query - add new constraints, add new views, process the results using the results iterator can be done with templates as well.

While writing queries of your own, you would have probably realized that there is a lot of duplication of effort. So we use templates which can be run numerous times and certain values can also be changed easily.

Let’s begin with a simple example. Let's say you want to extract the publication information about various Genes related to an organism. There is already a set template for this process.

We begin by importing the Service class and then create a template object. The parameter that we pass to the get\_template method is the name of the template.

To check the columns that our results will have we can use template.views. If you want to add a column use the add\_view/add\_views method.

Here we can see the output.

To look at the current constraints, use template.constraint\_dict. There is only one constraint which is editable. For example, you can change the value or operator if you want. However, even for editable constraints you are not allowed to change the path of the constraint.

To view the results we can use the results iterator as we learned previously.

We can see the output.

If you want to extract information for Drosophila Erecta and not Drosophila melanogaster, you can edit the query while calling the results method. In the code shown below, A refers to the code of the constraint. This code can be viewed using template.constraint\_dict as shown above. Here the constraint means all the information should be of Drosophila erecta.

This is how you can use a predefined query and modify it to work for you. You can visit the flymine website and take a look at some of the templates that have been defined there. Try running them using Python and change the constraints and views.

While exploring through templates you may come across templates that can be switched on or off. To switch off a constraint that is already turned on you can use the following code: template.get\_constraints\('B'\).switch\_off , where B is the code of the constraint in the constraint dictionary. In our example, the code is A since there is only one constraint.

To check if a particular constraint is switchable use the get\_switchable\_status method. This method can return three possible values - locked, on or off. Locked means that the particular constraint is fixed and cannot be switched on or off. If a particular constraint is switchable, it will return on or off depending on its current status.

So here we know A’s constraint is locked - can’t be switched on or off.

Naturally, if you try to switch off a constraint that is "locked" or not switchable, you will get an error.

It is also possible to modify constraints on the templates, as discussed above. Both the operator and value maybe altered. Here is an example from the Gene Intron template-

Firstly we see the status of the constraints on this template.

Here we get A’s constraint is editable and current constraint is on. B’s constraint is editable and current constraint is on too.

Now we modify constraint A, such that it only contains output data with secondary identifier CG10023. Then we print the results.

Here we can see the output.

Thus the output only contains results as per the applied constraints.

This tutorial focus on how templates help in automating commonly used queries and can make extremely efficient workflows. In the next tutorial, we will talk about how to access your saved templates and lists if you have your login information \(username and password\).

