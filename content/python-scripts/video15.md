# video15

+++ title = "Tutorial 15" description = "" weight = 16 +++    


Welcome to the fifteenth tutorial in the InterMine python tutorial series! This tutorial will help you utilise the module to get details about the data model of various mines. These are additional examples, besides the ones covered here - [http://intermine.org/intermine-ws-python/intermine.html\#module-intermine.model](http://intermine.org/intermine-ws-python/intermine.html#module-intermine.model). Each class \(data type\) has information containing references to other objects in the data model, collections of references or attribute details.

Let's begin by showing all the fields a data type contains \(including all Attributes, References and Collections listed alphabetically\). Each class can have any number of attributes \(which store primitive data, like numbers, dates, and strings\), references to other objects in the database, and collections of other objects in the database.

Here we see the datatype is Gene with the method get\_class.

Then we can see all fields in the gene data type.

Suppose you have a class name, and want to know the details about a particular field it contains, then you can do the following:

Here we only get the gene field from the Protein class.

Note that if you enter a field name that does not belong to the class, then you will receive an error.

Now, suppose you want to find out the nature of the data you retrieved earlier \(i.e. whether it is an 'Attribute' or 'Collection'/'Reference'\), you can easily iterate over the fields we had obtained earlier:

Here, we classify field types as either REFERENCE or ATTRIBUTE and print their names.

Notice that we used make\_path\(\) in the process. This function helps us construct paths and inspect whether it is valid or not, or as in here, utilise it to get more information from the model.

Now let's look at what information we can get regarding 'inheritance' of class'.

The isa function helps us determine whether 'input' belongs to the ancestry\(is a parent class or one of the parents of the parent class or so on\) of a given class.

So here we know Allele is not an ancestor of Protein.

Now let's see how we can retrieve the ancestry of a particular class:

The to\_ancestry method returns the ancestry of the given class.

We can print them here.

This tutorial thus explained how to get information regarding a class such as its attributes and the inheritance it shares without having to retrieve the entire model!

Thanks for watching!

