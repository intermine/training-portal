# Lists

### Overview

A **list** in InterMine refers to multiple items of the same type - for example, a list of genes or a list of binding sites. A list cannot contain a mixture of types - e.g. genes and proteins. To access the lists library, click on the **Lists** tab in the main menu bar. 

![Lists tab](../../../.gitbook/assets/lists-w-border.png)

The following list is a breakdown of what each key item in your **Lists** tab means: 

1. You need to be logged in to your InterMine account![](../../../.gitbook/assets/61205.png)to have access to your stored lists and to accomplish certain tasks that are not available to guests, including copying, editing and deleting lists. 
2. You can filter lists by typing in any keyword in the search field.
3. You can analyse your lists using the given set operations. These operations are inactive by default, and you need two or more lists to activate them. Please check [List set operations](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#list-set-operations) ****for more details.
4. You can control the number of rows shown per page to 20, 50, or 100
5. You can sort lists by date, type, tags, etc. 
6. This icon![](../../../.gitbook/assets/download-removebg-preview.png)represents a public list. 
7. Controls to copy, move or delete a given list or a group of lists

### Public lists![](../../../.gitbook/assets/download-removebg-preview.png) 

A public list is a list that has been created by InterMine developers and is ready for use. For example, FlyMine has public lists for sets of transcription factors in _Drosophila_. You can use these publicly available lists for analysis or run a particular search. 

![Public list](../../../.gitbook/assets/public-list.png)

{% hint style="info" %}
You cannot modify a public list. You need to make your own copy of a particular public list before you can edit it. Please check [How do I copy a list?](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#how-do-i-copy-a-list) for more details.
{% endhint %}

### Creating lists

Lists can be created internally - for example, from [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) or [Region Search](https://flymine.readthedocs.io/en/latest/region-search/Documentationregionsearch.html#regionsearch). They also can be uploaded from an external source via [Upload a list](upload-a-list.md). 

{% hint style="info" %}
Remember that you need to have an account prior to copying or storing any lists.
{% endhint %}

### Viewing lists

By default, when you click on the **Lists** tab, all of your lists will be shown.  Just remember, you need to be logged in to view your private lists. To filter your lists, you can use one of the available filtering options, such as date, tags, etc., shown in the next screenshot. 

![](../../../.gitbook/assets/filter-0.png)

For example, you can select to only view your private lists, public lists, lists saved in a particular folder first, or all of your lists at once by using the dropdown menu shown in the following screenshot. Check the Creating folders section for more details about how to make new folders. 

![](../../../.gitbook/assets/view-lists-edited.png)

![Viewing private lists only](../../../.gitbook/assets/private-lists-only.png)

{% hint style="info" %}
remember to log in to your account to view and manage your private lists
{% endhint %}

### Managing lists

You can manage your lists through the **Lists** view page. While logged in to your account, you can delete, rename, and upgrade a list, if your identifiers have become outdated.

### List tags

Tags can be used to organise your lists into categories. You can add your preferred tags to your saved lists by clicking on the **Edit list** icon✏in the **Lists** view page. 

![](../../../.gitbook/assets/edit-lists-0-1.png)

![](../../../.gitbook/assets/new-tag-cut.png)

![Adding tags](../../../.gitbook/assets/mytag-cut.png)

You can then filter your lists by one of the available tags in the **Lists** view page. 

![](../../../.gitbook/assets/filter-by-tag-1.png)

![Filter lists by tags](../../../.gitbook/assets/filter-by-tag-2.png)

### Using lists in searches

You can run searches on a list, such as a [template search](../template-search.md) or a search you have built using the query builder. For example, you may want to run a search to find all the GO terms for a list of genes. You can use lists in your searches in the template form - in list option. Check [How do I run a template search with one of my lists or a public list?](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/template-search#how-do-i-run-a-template-search-with-one-of-my-lists-or-a-public-list) for more information.

### List analysis

All lists have an associated [List analysis pages](list-analysis-pages.md), which provide a summary of your lists and several analysis tools. Besides, it is possible to carry out powerful analysis using lists' set operations, including union, intersect, subtract and symmetric difference. Please see [List set operations](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#list-set-operations) for more details.

### List set operations

Sets of lists can be analysed using the **Combine**, **Intersect**, **Subtract** and **Difference** functions. These set operations are available in the Lists view page. 

![Set operations](../../../.gitbook/assets/lists-set-functions-2.png)

To use any of these functions:

> 1. Select two or more lists you wish to analyse
> 2. Select one of the functions
> 3. Provide a name for your resulting list
> 4. Click Save New List
> 5. Your results will appear as a new list at the top of the Lists view page

For example, you can combine two lists and save the new list as **My\_New\_List**. 

![](../../../.gitbook/assets/combine-lists-edited.png)

![Combining lists](../../../.gitbook/assets/new-list-edited.png)

The BlueGenes interface offers four operations on sets for constructing new lists from given lists

{% hint style="success" %}
**Combine lists**: this is more of a traditional ‘**add**’ function, in that the resulting list will contain **all objects** from all selected lists. For example, if you have list A and list B, you can use the Combine function to create a new list containing all items in both lists - i.e. A + B.
{% endhint %}

{% hint style="success" %}
**Intersect lists**: this function creates a list that includes only items **common** to all given lists. For example, if you have list A and list B, you can use the Intersect function to create a new list containing only elements that exist in both A and B.
{% endhint %}

{% hint style="success" %}
* **Difference lists**: this function performs a [**mathematical symmetric difference**](https://en.wikipedia.org/wiki/Symmetric_difference) ****on all selected lists, and the resulting list will contain only items unique to each of those lists. It is more like the opposite of an intersection operation. For example, if you have list A and list B, you can use the Difference function to create a new list that includes objects only appearing in either A or B.
{% endhint %}

{% hint style="success" %}
* **Subtract lists:** this is more of a traditional ‘**subtract**’ function, in that the resulting list will contain objects that exist in one \(_**or group**_\) of the lists only. For example, if you have list A and list B, you can use the Subtract function to find unique items in list B. Note that this function gives you the option to perform the subtraction either way - i.e., A-B or B-A.
{% endhint %}

### Copying lists

You can copy a list from the **Lists** view \([How do I view my list?](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#how-do-i-view-my-lists)\) page. 

1. You can select one list and click on the copy ****icon![](../../../.gitbook/assets/download-1-.png)at the right of each list.
2. You can also use the checkboxes on the left of each list to select multiple lists at once
3. You can copy several lists using the **Copy All** option shown in the menu at the bottom of the page.

![](../../../.gitbook/assets/copy-list-0-edited.png)

You can click **Copy List\(s\)** to make a copy of the list or click **Cancel** to return to the **Lists** view page. Please note that lists can also be copied to a particular folder. Check the Creating folders section for more details about how to make new folders. 

![](../../../.gitbook/assets/copy-list-1-edited.png)

 A new list will be created with the same name and an underscore number. You should see a message at the top of the page informing you of the new list that has been created, and the copied list will show at the top of the **Lists** view page. You can then change the given name of the copied list to any preferred name; please see [How do I rename a list?](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#how-do-i-rename-a-list) for more details. 

![](../../../.gitbook/assets/copy-list-2-edited.png)

{% hint style="info" %}
remember to log in to your account to copy any list\(s\)
{% endhint %}

### Renaming a lists

To rename a list, you must be logged in to your user account. Click on the Edit list ✏ icon on the far right of the list's name. 

![](../../../.gitbook/assets/edit-list-0.png)

A fillable form will be shown that you can use to change the title - the name of the list,  provide a description, and to add any tag\(s\). 

![Rename a list](../../../.gitbook/assets/rename-a-list.png)

### Downloading lists

Lists can be downloaded from the **Lists** view page. You can select any particular list, and you will be taken to the list's detailed results table page. 

![](../../../.gitbook/assets/download-list.png)

You can click the **Export** button on the right of the resulting table to download the results to your device. You can export the results ****in different formats, such as tsv, csv, or fasta.  

![](../../../.gitbook/assets/download-list-2.png)

### Deleting lists

You can delete a list from the **Lists** **view** page. 

![](../../../.gitbook/assets/delete-a-list.png)

Select any list you want to delete and click on the **delete** icon to delete that list permanently.

![Deleting a list](../../../.gitbook/assets/delete-a-list-1-edited.png)

{% hint style="danger" %}
Please note that deleting a list is an irreversible action, and it only applies to your own lists!
{% endhint %}

### Creating folders

All public and private lists are shown in the **Lists** view page, and no folders exist by default. 

![](../../../.gitbook/assets/create-folder-1%20%281%29.png)

You can create new folders as part of [copying](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MQlo5xE8fGV8IneUfjG/content/user-documentation/lists/lists#copying-lists) a list. For example, you can select any list that you want to copy into a folder, and click on the copy ****icon![](../../../.gitbook/assets/download-1-.png)at the right of that list. You can then type any preferred folder name in the **Choose folder** input field and enter to create a new folder. 

![](../../../.gitbook/assets/create-folder-2.png)

Click on **Copy List\(s\)** to make a copy of the list inside the new folder, **My Folder**. 

{% hint style="info" %}
Click the arrow⬆icon to cancel copying the list into the new folder, and delete the newly created folder.  
{% endhint %}

![](../../../.gitbook/assets/create-folder-3.png)

The new folder will be shown at the top of the Lists view page. 

![](../../../.gitbook/assets/create-folder-4.png)

To view the contents of any folder, click on the folder's name or the➕icon to the left of that folder. The contents of any folder are usually displayed between light blue lines. 

![](../../../.gitbook/assets/create-folder-6.png)

New folders can also be created when moving a list or a group of lists. For example, you can use the checkboxes to select multiple lists and then copy or move the selected lists to a new folder using the **Copy All - Move All** options shown in the menu at the bottom of the page. Then follow the same previous steps to create the new folder. 

![](../../../.gitbook/assets/move-lists.png)

{% hint style="info" %}
Please see the [Copying lists](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/~/drafts/-MQlo5xE8fGV8IneUfjG/content/user-documentation/lists/lists#copying-lists) section for more information about making a copy of a given list
{% endhint %}

### TroubleShooting

#### I am being told to upgrade my lists - what does this mean?

Every time we make a new release of an InterMine database, it is possible that some of the gene models have changed, which means that some of your identifiers might become outdated. For example, a gene may have been split; in this case, an identifier may now refer to more than one gene. Often a gene model is just updated, and the old identifier becomes a synonym while the gene is assigned a new identifier. When we make a new release, all of the identifiers present in your saved lists will be checked against the new database’s identifiers. When any discrepancies are found \(i.e. if any have now become synonyms or refer to more than one gene\), you will be asked what you want to do about these genes before using your list again. 

A message appears at the top of any page informing you that you have lists that need an update. To update your lists, you must be logged in to your user account. Within the Lists view page, lists that need to be updated will be shown first. The list upgrade system is the same as The Identifier Resolution page you see when you upload a list.

