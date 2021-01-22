# The Query Builder

## The Query Builder

The Query Builder is InterMine’s custom query building interface,  allowing you to create and save your own searches. Users usually use this flexible interface to construct their own data mining queries. The QueryBuilder lets you view the data model, apply constraints and select your preferred output. To access the query builder, click on the **Query Builder** tab in the top navigation bar. 

![](../../.gitbook/assets/query-tab.png)

The main query builder page is divided into four main sections: 

{% tabs %}
{% tab title="Model Browser" %}
The **Model browser** helps you find and add your data of interest.

![](../../.gitbook/assets/data-model-edited%20%281%29.png)

1. The class field to browse through available classes. For example, the screenshot shows the **Gene** class with its associated attributes, such as **Length**, **Name**, **Primary Identifier**, etc. 
2. You can click the **Browse** button to be directed to the **Data browser tree** to browse all class names. Clicking on any class name will take you back to the **Model browser** with that class selected in the class field. 
3. You have some controls to manage the selected class's data. You can use **Summary** to summerise the selected class by adding its common attributes, **Expand** to expand the **Model browser tree** to show all selected attributes, **Collapse** to fold the **Model browser tree** to the top level and **Clear** to remove all selected attributes. 
4. Use **checkboxes to** add individual fields - attributes - to your results. 
5.  Expand more fields underneath class a using the➕sign. 
6. Click **Summary** to add a summary of common fields to the results table.  
{% endtab %}

{% tab title="Query Editor" %}
* The **Query Editor** tab allows you to edit your query by adding filters - constraints - or remove selected classes or attributes. 

![](../../.gitbook/assets/editor-window%20%281%29.png)

* The **Manage Columns** tab lets you manage the order of selected columns in your results and sort data in each column alphabetically in ascending or descending order. 

![](../../.gitbook/assets/manage-cols%20%281%29.png)
{% endtab %}

{% tab title="Query Preview" %}
* The **Preview** tab lets you preview how the results of the query under creation will look like. 

![](../../.gitbook/assets/preview-2.png)

* The **XML** tab lets you view and copy queries in XML format to share them with others.  

![](../../.gitbook/assets/xml%20%281%29.png)
{% endtab %}

{% tab title="Query History" %}
* The **Recent Queries** tab displays recent queries you run. 

![](../../.gitbook/assets/recent.png)

* When you successfully save a query, a confirmation message will be shown, and you can view saved queries under the **Saved Queries** tab. 

![](../../.gitbook/assets/save-query-message.png)

* To the right of each saved query, there are some available actions that you can use to Load or run that query, Rename it or Delete it if needed. 

![](../../.gitbook/assets/saved-queries.png)

* You can also import query by pasting the query XML in the input field and click **Upload Query** under the **Import from XML** tab. 

![](../../.gitbook/assets/import-xml-query.png)
{% endtab %}
{% endtabs %}

### Constructing queries

{% hint style="info" %}
To build a query, you must first decide on a starting point - or a class - to start your query. The class to begin a query defaults to **Gene** and can be changed with the dropdown list in the Model Browser. 
{% endhint %}

There are three steps to construct a query, which you can repeat for any additional data required:

1. Navigate the model/data browser to find the class or attribute you need.
2. Add the appropriate constraints - or filters - to selected class/attribute.
3. Decide on the columns you want to view in your results.

 These steps are explained in more detail below. 

### Navigate the data browser

As mentioned earlier, the query builder's left-hand pane is called the model browser, which allows you to navigate through all the data classes from your defined starting point. You must first decide on a starting point - or a class - from which you can start your query. The classes are linked through logical references - for instance, you can navigate from gene to proteins, transcripts and microarray data etc. Classes and references will vary for each InterMine. Every class of data has certain attributes - fields - associated with it. For instance, a gene has a primary identifier, name and symbol, among others. Use the model browser to navigate to the data you are interested in searching. For example, to get to protein domain from **Gene** as the starting point, you would expand the **Protein** class first and then the protein domain class. For each class and attribute in the model browser, there is a **checkbox** that you can use to add - or remove - a given class or attribute from your results.

![](../../.gitbook/assets/navigate-the-data-model.png)

### Add a constraint - filter - to your query

Once you have navigated to the data you want to search, you can now add a constraint to filter your results and only return the data you are interested in. For example, if you want to return all genes which code for proteins with homeo domains, you would add a constraint to the ‘name’ attribute of the protein domain class. The type of constraint you can add depends on the class and attribute selected. For some, you may have to add some text; while others may require you to select from a drop-down list. Some will allow you to choose a list of saved objects, e.g. a list of genes. You can add as many constraints as you wish to build up your query. The set of constraints you add is shown in the right-hand pane of the Query Builder - specifically under the **Query Editor** and **XML** tabs. 

Remember that you are building a query from scratch so you may need to put in constraints to limit the organism or the set of genes. For example, the following screenshot shows a query under construction - without any constraints, the expected results are 232429 rows. 

![](../../.gitbook/assets/query-filter-0.png)

Adding one constraint to lookup the **PPARG** gene in the previous query limits the search results to only three rows. 

![](../../.gitbook/assets/query-filter-1.png)

Constraints are also shown in the query's XML format as follows

```text
<query model="genomic" view="Gene.symbol 
Gene.primaryIdentifier Gene.name 
Gene.secondaryIdentifier 
Gene.length" constraintLogic="(A)" sortOrder="">
   <constraint path="Gene" value="PPARG" 
    op="LOOKUP" code="A"/>
</query>
```

{% hint style="info" %}
To navigate back to a place in the model browser, click on the class name in the right-hand pane. 
{% endhint %}

### Choose the data you want in your results.

Every attribute has a **checkbox** on the left that you can tick✅to add that attribute to your query output. All selected attributes will become columns in your results table when you run your search. 

{% hint style="info" %}
Columns are shown - and can be removed - under the Query Editor tab. 
{% endhint %}

### Run your search

Once you are happy with your query and the attributes you have selected for your results, press **Show All Rows** to run your search. Your results will be displayed in our [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables). 

## Advanced features of the query builder

### Subclasses

Some classes have subclasses, which are more specialised sets of the main class. For example, the **UTRs class** in HumanMine has two subclasses **Five Prime UTR** and **Three Prime UTR**. To constrain a class to its subclass, click on the class name and select the subclass from the drop-down list. Classes which have subclasses are indicated as shown below. 

![](../../.gitbook/assets/subclasses.png)

### Outer joins

When adding a constraint to a query, you also need to consider whether you want this constraint to limit your results to just those items with that information or if you want your results to show all the items and the new feature if it exists. For example, if you are adding a constraint to the protein domain class for homeobox, and selecting to show genes and proteins in your results, do you want your results to show:

1. Only genes and proteins which contain a homeobox \(inner join\)
2. All genes and proteins and indicate which contain a homeobox. \(outer join\)

The default constraint is always A \(inner join\). i.e. the record you are searching must have information in the field the path describes. However, you can change the logic to B using the outer-join. To do this, add your constraint in the usual way. The outer-join icon is found in the right-hand pane next to your constraint. Click on this to change the logic of your constraint:

Note that the column summary and filtering still applies to the results table as a whole

### Loop queries

Coming soon. 

### Constraint logic

You can set the constraint logic for your query under **Query Editor** tab. Each constraint is assigned a letter - which can be found under **Query Editor** tab. The constraint logic accepts: **AND** and **OR** and **NOT** logic.

### Sorting

By default, results are sorted on the contents of the first column. However, sorting and reordering columns can be changed under the **Manage Columns** tab. Check the **Query Editor** tab at the top of this page for more details about sorting and ordering columns. 

### Saving and exporting your query

If you are logged in you can save a query you have constructed permanently under your **Saved Queries** tab. The ‘Save Query’ option is found at the bottom of the **Query Builder** and **Manage Columns** tabs. You can also export your query as XML under the **XML** tab. You can share exported queries with your colleagues or with the [InterMine team](contact-us.md) if you have any problems.  Queries can be imported in XML under the **Import from XML** tab and also be used in [**GET**](https://www.w3schools.com/tags/ref_httpmethods.asp) ****and [**POST**](https://www.w3schools.com/tags/ref_httpmethods.asp) requests used by the [web services](http://iodocs.labs.intermine.org/). See the **Query Editor** tab at the top of the page for more information on saving and exporting queries. 

### The difference between NULL and NOT EQUALS

Searching Null vs NOT EQUALS

When using a “negative” search such as !=, it is important to understand the difference between a NULL value and an empty value. NUll means a value that is unknown or not applicable. Empty means known but not present. This has implications for the way you may construct a query.

For Example: If you try a query such as “Give me all genes where the gene name doesn’t equal something \(e.g. ACXE\)” it excludes all the null values from the results too. In such a case you probably want the query to return all genes where the name does not equal “ACXE” AND those that do not have a name. For those that do not have a name, the field is NULL \(which is different to empty\).

For example, try this query in FlyMine:

It returns 7627 genes. So from the total fly genes, it has not returned the one gene that has the name ACXE AND all the genes which are “NULL” for gene name.

Now, if we add an additional constraint:

\(NOTE: also change the constraint logic to C or B\)

We now get 18, 059 rows - this is all the genes which do not have name ACXE and all genes which have a NULL name.

Note: To add the “NULL” constraint, select “Filter query results on this field having any value or not” and select the “Has no value” checkbox:

## Troubleshooting

### Why do I keep getting “No results” for my search?

Sometimes your search gives “No results” because one part of your search does not yield results. If you have several constraints, try removing only one at a time to see if you will get results. Alternatively, toggle your constraints to an [outer join](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MRV1dETGFXxj_SCpAD8/content/user-documentation/the-query-builder#outer-joins) from your results to see if there is data fulfilling that constraint; you can check [Outer joins](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MRV1dETGFXxj_SCpAD8/content/user-documentation/the-query-builder#outer-joins) for more details. If you still need additional help, please [Contact Us](contact-us.md).

### I am not sure how to start building a search; it looks hard!

Every template search can be displayed in the query builder. Try looking at some of the simple templates in the query builder and see how they have been constructed. Use this as a starting point to try changing a constraint or adjusting what is shown in the results table. If you need any help, please [Contact Us](contact-us.md).

To decide which class to select to begin building a query, think about the data you are trying to return. For example, suppose you want to know about the expression of a set of genes. In that case, you can start your query from Gene, where you can define which genes you are interested in and then navigate to the expression data, where you can determine what expression data you like to see. Similarly, you could construct the same query by defining the expression data. Expression data links to Genes, which allows you to add your gene constraints.

### I can’t find the data I am looking for in the model browser!

The data browser is based on the sequence ontology and follows the logical relationships found in biological data. **For example, Exons are referenced from Gene and Protein domains are referenced from Protein**. Many additional classes and fields have been added that also follow logical biological relationships. So if you are looking for Gene expression data, you will find this referenced from Gene. For details of all the data sources loaded to see the **Data** tab. If you need additional help, please Contact Us.

### I don’t understand what a field/class means.

Some fields have an information icon which provides an additional description of those fields. If you are unsure of a field’s contents, you can add it to your results and run the query. Most queries give results immediately, which allows you to adjust the columns you want to include in your results and fine-tune your query. It is also possible to do this from within the **Results Tables**. If you need additional help, please [Contact Us](contact-us.md). 

### How do I navigate to a class I have constrained without having to go through the model?

### Browser again?

Clicking on a class name in the right-hand Summary pane will open the model browser at that class.

