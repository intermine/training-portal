# Gene Ontology Data

### How do I find the GO annotations for my set of genes?

{% hint style="info" %}
This assumes that you have successfully uploaded or created your list of genes. If you require help with this, please see [Lists - Upload a list](../lists/upload-a-list.md) section for more details. 
{% endhint %}

To find the GO term annotations for your genes, it's easier to start by creating a template search specifically for this purpose. 

1. From the HumanMine homepage, select the **‘Templates’** tab from the top navigation bar.
2. From the list of templates, we are looking for the [Gene → GO terms](http://bluegenes-staging.apps.intermine.org/humanmine/templates/Gene_GO) template. If you cannot see it immediately, enter the term **‘GO’** into the search box to filter the results. 
3. Click on the template name or **‘View &gt;&gt;’** at the bottom left corner to expand the template details, including the fillable form. 
4. Enter a gene or select a list you wish to run the search with, then press **‘View Rows’**. 

{% embed url="https://drive.google.com/file/d/1U1ZSvMJuYasSYedYKi2gLARIkrEGrjmW/view?usp=sharing" %}

### Modifying and filtering your search results

This template search returns GO term annotations for all three GO ontologies and other GO attributes, such as evidence code and qualifier. You may wish to further filter your results on some of these attributes or add additional attributes to the search, such as annotation extension or the GO ‘with’ attribute. The following examples illustrate how to do this. 

### How do I filter my results to show only GO annotations from the ‘biological process’ ontology?

The easiest way to filter your results is by using the filter functions in the results table. 

1. You can accomplish this by clicking on the graph icon![](../../../.gitbook/assets/bar-chart.png)in the **Ontology Term Namespace** column header. 
2. Then select **‘biological\_process’** using the checkbox to the left, and click the **‘Filter’** button. 
3. To return to your original results, either remove the filter by clicking on the blue filter icon![](../../../.gitbook/assets/screenshot-902-.png)in the column header or use the **UNDO** button above the results table. 

{% embed url="https://drive.google.com/file/d/1i39eZw1\_TdqhzPLYTc97LoaQ6GwsXwvB/view?usp=sharing" %}

### How do I filter my results to remove those with the IEA - Inferred from Electronic Annotation - evidence code? 

You can accomplish this in three ways:  

* **Using the column summary**

1. Click on the column summary/graph icon![](../../../.gitbook/assets/bar-chart.png)in the **Code** column header. 
2. Select all evidence codes except the **IEA** code.
3. Click **Filter**.

* **Using the Code column filter icon**

1. Click on the filter icon![](../../../.gitbook/assets/screenshot-902-.png)in the Code column header. 
2. Use the left drop-down menu to choose the **!=** option. 
3. Use the right drop-down list to select the **IEA** code.
4. Click **‘Apply’** to add the new filter. 

* **Using the Manage Filters button**

1. Click on the **‘Manage Filters’** button above the results table. 
2. Using the **‘Add a new filter’** drop-down menu, click the **GO Evidence Code** field. 
3. Click the blue plus sign to add a new filter, which will show a new drop-down list on the left of the **GO Evidence Code** field.
4. Choose the **!=** option 
5. Finally, click **‘Apply Changes’**. 

### How do I analyse my gene list for GO term enrichment?

Go term enrichment is calculated automatically for all gene lists - you have to navigate to the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) for your list. The GO term enrichment for your list will be displayed as a widget \(see [What is a widget?](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#widgets)\). For more information on the enrichment calculation, see the [InterMine documentation](http://intermine.readthedocs.org/en/latest/embedding/list-widgets/enrichment-widgets/).

### Other Gene Ontology searches

FlyMine includes many other Gene Ontology related searches. To see the full range of searches navigate to the [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) page and enter ‘GO’ into the filter box \(see [Finding the template search that you want](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#filtertemplatesearches)\). For example, you can find all genes annotated to a particular GO term using the [GOterm → Genes](http://www.flymine.org/query/template.do?name=GOTerm_Gene2&scope=all) template. This search is extended by the template [GO term name \[and children of this term\] → Genes in one specific organism](http://www.flymine.org/query/template.do?name=GO_Gene&scope=all), which will return genes annotated to the term given AND genes annotated to any children of this term. Various combinations of GO term and data searching are available, for example, [Gene → orthologues and GO terms of these orthologues](http://www.flymine.org/query/template.do?name=Gene_OrthologueGO&scope=all), will return the GO terms annotated to the orthologues of your gene\(s\). Remember, if you don’t see what you are looking for please [Contact Us](https://flymine.readthedocs.io/en/latest/contact/Documentationcontact.html#contact) - we can probably construct the search for you.

