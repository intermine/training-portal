# Lists

### Overview

A **list** in InterMine refers to multiple items of the same type - for example, a list of genes or a list of binding sites. A list can not contain a mixture of types - e.g. genes and proteins.

### What is a public list? 🌍  

A public list is a list that has been created by the InterMine developers and is ready to be used. For example, FlyMine has public lists for sets of transcription factors in _Drosophila_. You can use these publicly available lists for analysis or to run a particular search. If you wish to modify a public list, you need to first make your own copy of that list. Please check **How do I copy a list?** section for more details on copying a list.

### How do I make a list?

Lists can be created internally - for example from [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) or the [Region Search](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearch), or they can be uploaded from an external source: [Upload a list](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listupload). **NOTE**: Remember to create a [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account if you want to permanently store your list.

### How do I view my list?

To find a list, navigate to the lists tab and click on the **view** sub tab. All your lists and the public lists will be shown here. **NOTE**: remember to login to view previously stored lists. You can also manage your lists through your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account.

### Managing your lists

You can manage your lists through your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account. Here you can delete, rename and upgrade lists \(if your identifiers have become outdated\).

### Using lists in searches

You can run searches on a list - for example a template search or a search you have built yourself using the query builder. For example, you may want to run a search to find all the GO terms for a list of genes. You can do this from the template form \(see [How do I run a template search with one of my lists or a public list?](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearchelists)\).

### List Analysis

All lists have an associated [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage), which provide a summary of your list and several analysis tools. In addition it is possible to carry out powerful analysis using the list operations: union, intersect, subtract and asymmetric difference \(see [List Set operations:]()\).

### List Set operations:

Sets of lists can be analysed using the union, intersect, subtract and asymmetric difference functions. These set operations are available on both the lists view \([How do I view my list?]()\) page and the lists page within your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account. To use any of these functions:

> 1. Select the lists you wish to analyse.
> 2. Select the function
> 3. Provide a name for your resulting list
> 4. Click **save**: Your results will appear as a list at the top of the page.

{% hint style="info" %}
If you are on your myMine list page, you provide a name for your new list and then select the function you wish to use.

* **Subtract:** This function creates a list that contains the unique entries from **both** lists provided: i.e it is like the opposite of an intersect: if an object is in both lists it will not be in the resulting list, but if it appears in either one, but not the other it will be in the resulting list.
* **Asymmetric difference:** This is more of a traditional ‘subtract’ function, in that the resulting list will contain objects that are in one of the lists only. For example if you have lists A and B and you want to find those unique to list B, use the asymmetric difference function. Note that this function gives you the option to perform the subtraction either way - ie, A-B or B-A.
{% endhint %}

### How do I copy a list?

You can copy a list either in the lists tab of your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account or from the lists **view** \([How do I view my list?]()\) page. Select your list and click on **copy**. A new list will be created with the same name and an underscore number. You should see a message at the top of the page informing you of the new list that has been created.

### How do I delete a list?

You can delete a list either in the lists tab of your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account or from the lists **view** \([How do I view my list?]()\) page. Select your list and click on **delete**, your list will be deleted straight away.

### How do I rename a list?

To rename a list you must be in your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account. Click on the rename icon next to the list name to provide the new name:

### I am being told to upgrade my lists - what does this mean?

Every time we make a new release of an InterMine database it is possible that some of the gene models will have changed. This means that some of your identifiers may now be out of date. For example, a gene may have been split, in which case an identifier may now refer to more than one gene. Often a gene model is just updated and the old identifier becomes a synonym and the gene is assigned a new identifier. When we make a new release, all the identifiers in your saved lists will be checked against the identifiers in the new database. If any discrepancies are found \(i.e if any have now become synonyms, or refer to more than one gene\) then you will be asked what you want to do about these genes before you are able to use your list again.

A message appears at the top of any page informing you that you have lists that need updating. To update your lists you must be in your [MyMine](https://flymine.readthedocs.io/en/latest/mymine/DocumentationMyMine.html#mymine) account. Within your lists page, the lists that need updating will be shown first. The list upgrade system is the same as the [The Identifier Resolution page](https://flymine.readthedocs.io/en/latest/lists/upload/Documentationlistupload.html#listconfirmationpage) that you see when you upload a list.

