# Lists

### Overview

A **list** in InterMine refers to multiple items of the same type - for example, a list of genes or a list of binding sites. A list cannot contain a mixture of types - e.g. genes and proteins. To access your lists library, click on the **Lists** tab in the main menu bar. 

![](../../../.gitbook/assets/lists-tab.png)

The following is a breakdown of what each key item in the **Lists view page** means: 

1. You need to be logged in to your InterMine account![](../../../.gitbook/assets/61205.png)to access your saved lists and perform specific tasks not available to guests, including copying, editing, and deleting lists.
2. You can filter lists by typing in any keyword in the search field.
3. You can analyse your lists using the given set operations. These operations are inactive by default, and you need two or more lists to activate them. Please check [List set operations](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#list-set-operations) ****for more details.
4. You can control the number of rows shown per page to 20, 50, or 100
5. You can sort lists by date, type, tags, etc. 
6. You can use ![](../../../.gitbook/assets/refresh.png)to refresh your lists
7. This icon![](../../../.gitbook/assets/download-removebg-preview.png)represents a public list; while the yellow user ![](../../../.gitbook/assets/61205.png) icon represents a private list/folder. 
8. You can create folders and subfolders to save your lists
9. Controls to copy, move or delete a given list or a group of lists

### Public lists![](../../../.gitbook/assets/download-removebg-preview.png) 

A public list is a list that has been created by InterMine developers and is available to all users. For example, HumanMine has public lists for Pax6 \(\(Paired Box 6\) gene targets. You can use these publicly available lists for analysis or run a particular search. 

![](../../../.gitbook/assets/public-list%20%281%29.png)

{% hint style="info" %}
You can't modify a public list. Instead, make your own copy of that list to be able to edit it. Please check [**Copying lists**](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#copying-lists) for more details.
{% endhint %}

### Creating lists

Lists can be created internally - for example, from [Results Tables](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#resultstables) or [Regions Search](../region-search.md). They also can be uploaded from an external source via [Upload a list](upload-a-list.md). 

{% hint style="info" %}
Remember that you need to have an account prior to copying or storing any lists.
{% endhint %}

### Viewing lists

By default, when you click on the **Lists** tab, all of your lists will be shown; private lists are only shown if you are logged in to your account. To filter your lists, you can use one of the provided filtering options, such as date, tags, etc., shown in the next screenshot. 

![](../../../.gitbook/assets/list-filters.png)

By default, all public and private lists/folders are shown, but it is possible to only view your private lists, public lists, lists saved in a particular folder first by using the dropdown menu.  

![](../../../.gitbook/assets/list-filtering-2.png)

![Displaying private lists only](../../../.gitbook/assets/private-lists-only%20%281%29.png)

{% hint style="info" %}
Remember to log in to your account to view and manage your private lists
{% endhint %}

### Managing lists

You can manage your lists through the **Lists** view page. While logged in to your account, you can delete, rename, and upgrade a list, if your identifiers have become outdated.

### List tags

Tags can be used to organise your lists into categories. You can add your preferred tags to your saved lists by clicking on the **Edit list** icon✏in the **Lists** view page. 

![](../../../.gitbook/assets/private-list-no-tag.png)

![](../../../.gitbook/assets/new-tag-cut.png)

![Adding a tag](../../../.gitbook/assets/mytag-cut.png)

You can then filter your lists by one of the available tags in the **Lists** view page. 

![](../../../.gitbook/assets/filtering-by-tag.png)

![](../../../.gitbook/assets/mytag-updated.png)

### Using lists in searches

You can run searches on a list, such as a [template search](../template-search.md) or a search you have built using the query builder. For example, you may want to run a search to find all the GO terms for a list of genes. You can use lists in your searches in the template form - in list option. Check [How do I run a template search with one of my lists or a public list?](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/template-search#how-do-i-run-a-template-search-with-one-of-my-lists-or-a-public-list) for more information.

### List analysis

All lists have an associated [List analysis page](list-analysis-pages.md), which provide a summary of your lists and several analysis tools. Besides, it is possible to carry out powerful analysis using lists' set operations, including union, intersect, subtract and symmetric difference. Please see [List set operations](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#list-set-operations) for more details.

### List set operations

Sets of lists can be analysed using the **Combine**, **Intersect**, **Subtract** and **Difference** functions. These set operations are available in the Lists view page. 

![Lists set operations](../../../.gitbook/assets/set-operations.png)

To use any of these functions:

> 1. Select two or more lists you wish to analyse
> 2. Select one of the functions
> 3. Provide a name for your resulting list
> 4. Click **Save New List**
> 5. Your results will appear as a new list at the top of the Lists view page

For example, you can combine two lists, public and private lists, and save the new list as **My\_New\_List**. 

![](../../../.gitbook/assets/combine-lists%20%281%29.png)

![](../../../.gitbook/assets/new-list.png)

The BlueGenes interface offers four operations on sets for constructing new lists from given lists

{% hint style="success" %}
**Combine lists**: this is more of a traditional ‘**add**’ function, in that the resulting list will contain **all objects** from all selected lists. The mathematical symbol for the Combine operation is$$A ∪ B$$. For example, if you have list A and list B, you can use the Combine function to create a new list containing all items in both lists - i.e. A + B. 
{% endhint %}

{% hint style="success" %}
**Intersect lists**: this function creates a list that includes only items **common** to all given lists. The mathematical symbol for the Intersect operation is $$A ∩ B$$. For example, if you have list A and list B, you can use the Intersect function to create a new list containing only elements that exist in both A and B.
{% endhint %}

{% hint style="success" %}
* **Difference lists**: this function performs a [**mathematical symmetric difference**](https://en.wikipedia.org/wiki/Symmetric_difference) ****on all selected lists, and the resulting list will contain only items unique to each of those lists. This operation is more like the opposite of an intersection operation, which is represented mathematically as$$A ∆ B $$. For example, if you have list A and list B, you can use the Difference function to create a new list that includes objects only appearing in either A or B.
{% endhint %}

{% hint style="success" %}
* **Subtract lists:** this is more of a traditional ‘**subtract**’ function, in that the resulting list will contain objects that exist in one \(_**or group**_\) of the lists only. The mathematical symbol for the Subtract operation is $$A ∩ B$$.  For example, if you have list A and list B, you can use the Subtract function to find unique items in list B. Note that this function gives you the option to perform the subtraction either way - i.e., A-B or B-A.
{% endhint %}

### Copying lists

Copying a list or several lists can be done from the [**Lists** **view page**](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#viewing-lists). 

{% hint style="info" %}
Remember to log in to your account to copy any list\(s\)
{% endhint %}

* To copy a single list, click on the copy ****icon![](../../../.gitbook/assets/download-1-.png)on the right of your list of interest. 

![](../../../.gitbook/assets/copy-a-list.png)

* To copy multiple lists at once, use the checkboxes on the left of each list to select one or more lists. Then, you can copy all selected lists using the **Copy All** option shown at the bottom of the page.

![](../../../.gitbook/assets/copy-several-lists.png)

You can click **Copy List\(s\)** to make a copy of the selected list\(s\) or click **Cancel** to exit the Copy list\(s\) window. 

{% hint style="info" %}
Please note that lists can also be copied to a particular folder or sub-folder. Check the [**Creating folders** ](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#creating-folders)section for more details about how to make new folders and sub-folders. 
{% endhint %}

![](../../../.gitbook/assets/copy-one.png)

![](../../../.gitbook/assets/copy-all.png)

For each copied list, a new list will be created with the same name as the original list and an underscore followed by a number. You should see a message at the top of the page informing you of the new list\(s\) created, and the copied list\(s\) will appear at the top of the **Lists** view page. The default name of the copied list\(s\) can be changed to any preferred name; please see [**Renaming lists**](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#renaming-lists) for more details. 

![](../../../.gitbook/assets/copied-list-default.png)

### Renaming lists

To rename a list, you must be logged in to your user account. Click on the Edit list✏icon on the far right of the list's name. 

![](../../../.gitbook/assets/my-copied-list-0.png)

A fillable form will be shown that you can use to change the title - the name of the list,  provide a description and add any tag\(s\). Click **Save** to proceed or **Cancel** to exit the **Edit list** window. 

![](../../../.gitbook/assets/rename-a-list-zoomed.png)

### Upgrading lists

to be added. 

### Downloading lists

Lists can be downloaded from the **Lists** view page. You can click on any list you want, and you will be taken to the list's detailed results table page. 

![](../../../.gitbook/assets/export-a-list.png)

Click the **Export** button on the right of the resulting table to download the results to your device. You can export the results ****in different formats, such as tsv, csv, or fasta.  

![](../../../.gitbook/assets/download-list-2%20%281%29.png)

### Deleting lists

You can delete a list or several lists from the **Lists** **view** page.

* To delete a single list, click on the delete ****icon on the right of your list of interest. 

![](../../../.gitbook/assets/delete-a-list%20%281%29.png)

* To delete multiple lists at once, use the checkboxes on the left of each list to select one or more lists. Then, you can delete all selected lists using the **Delete All** option shown at the bottom of the page.

![](../../../.gitbook/assets/delete-many-lists.png)

You can click Delete List\(s\) to remove selected list\(s\) permanently or click Cancel to exit the Delete list\(s\) window.

![](../../../.gitbook/assets/delete-one-list.png)

![](../../../.gitbook/assets/delete-all.png)

{% hint style="danger" %}
Please note that deleting a list is an irreversible action, and it only applies to your private lists!
{% endhint %}

### Creating folders

The BlueGenes application allows users to create folders and sub-folders to organise their lists. Lists can be either copied or moved into a folder or sub-folder. By default, all public and private lists are shown in the **Lists** view page, and no folders exist. 

![](../../../.gitbook/assets/create-folder-1%20%281%29.png)

{% hint style="info" %}
Folders can be created as part of copying, moving, or editing a list. 
{% endhint %}

* You can create new folders while [copying](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#copying-lists) a list or a group of lists. While the Copy list\(s\) window is active, you can type any preferred folder name in the **Choose folder** input field and enter to create a new folder.

![](../../../.gitbook/assets/create-folder-2.png)

Click on **Copy List\(s\)** to copy the desired list\(s\) inside the new folder, **My Folder**. 

{% hint style="info" %}
Click the arrow⬆icon to cancel copying the list into the new folder, and delete the newly created folder.  
{% endhint %}

![](../../../.gitbook/assets/create-folder-3.png)

{% hint style="info" %}
Please see the [Copying lists](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#copying-lists) section for more information about making a copy of a given list or group of lists.
{% endhint %}

* New folders can also be created when moving a list or a group of lists while the **Move list\(s\)** window is active. Just type in any preferred folder name in the Choose folder input field and enter to create a new folder.

![](../../../.gitbook/assets/create-folder-moving.png)

* You can also create new folders while editing a list using the ✏icon to the right of the desired list while the **Edit list** window is active. Just type in any preferred folder name in the Choose folder input field and enter to create a new folder.

![](../../../.gitbook/assets/create-folder-editing.png)

* Sub-folders can be created inside existing or new folders following the same previous steps.  

![](../../../.gitbook/assets/sub-folder-0.png)

Any new folders or sub-folders are shown at the top of the Lists view page. 

![](../../../.gitbook/assets/create-folder-4.png)

![](../../../.gitbook/assets/sub-folder-3.png)

To view the contents of any folder, click on the folder's name or the➕icon to the left of that folder. The contents of any folder are usually displayed between light blue lines. 

![](../../../.gitbook/assets/create-folder-6.png)

Folders and sub-folders can only be deleted by deleting their content. For example, if you wish to delete your newly created sub-folder, you can remove the content inside it, or **My\_Copied\_List.** You can take a look at [**Deleting lists**](https://user-documentation-intermine.gitbook.io/user-documentation/content/user-documentation/lists/lists#deleting-lists) to know how to delete a list or several lists. 

![](../../../.gitbook/assets/delete-subfolder.png)

![](../../../.gitbook/assets/delete-subfolder-1.png)

### TroubleShooting

#### I am being told to upgrade my lists - what does this mean?

Every time we make a new release of an InterMine database, it is possible that some of the gene models have changed, which means that some of your identifiers might become outdated. For example, a gene may have been split; in this case, an identifier may now refer to more than one gene. Often a gene model is just updated, and the old identifier becomes a synonym while the gene is assigned a new identifier. When we make a new release, all of the identifiers present in your saved lists will be checked against the new database’s identifiers. When any discrepancies are found \(i.e. if any have now become synonyms or refer to more than one gene\), you will be asked what you want to do about these genes before using your list again. 

A message appears at the top of any page informing you that you have lists that need an update. To update your lists, you must be logged in to your user account. Within the Lists view page, lists that need to be updated will be shown first. The list upgrade system is the same as The Identifier Resolution page you see when you upload a list.

