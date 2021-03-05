# Gene Ontology Data

### How do I find the GO annotations for my set of genes?

This assumes that you have successfully uploaded or created your set of genes. If you require help with this please see [Lists](https://flymine.readthedocs.io/en/latest/lists/overview/Documentationlists.html#lists)

To find the GO term annotations for your genes it is easiest to start with a specially created template search:

1. From the FlyMine homepage, select the ‘Templates’ tab from the navigation bar.
2. From the list of templates, we are looking for one called [Gene → GO terms](http://www.flymine.org/query/template.do?name=Gene_GO&scope=all). If you cannot see it immediately enter ‘GO’ into the filter box to narrow the search.
3. Click on the template name, this will display the template form. Enter the gene or select the list you wish to run the search with and press ‘Show results’.

Modifications:

This template search returns GO term annotations for all three GO ontologies along with other GO attributes, such as evidence code and qualifier. You may wish to further filter your results on some of these attributes, or add additional attributes to the search, such as annotation extension or the GO ‘with’ attribute. The following examples illustrate how to do this:

### How do I filter my results to show only GO annotations from the ‘biological process’ ontology?

The easiest way to filter your results is by using the filter functions in the results table. In the ontology term.Namespace column click on the column summary icon. Select ‘biological process’ and click filter. To return to your original results either remove the filter by clicking on the green ‘filter’ icon in this column header, or use the UNDO button above the results table:

### How do I filter my results to remove those with the IEA \(inferred from electronic annotation\) evidence code?

You can do this either through the column summary or the filter’ function:

1. Using the column summary:

Click on the column summary icon in the code column. Select all evidence codes except IEA and click filter.

1. Using the filter button:

Click on ‘Filters’ above the results table. Scroll down to the GO Evidence Code field and click ‘Choose’. Define your filter and click ‘Add filter:

### How do I analyse my gene list for GO term enrichment?

Go term enrichment is calculated automatically for all gene lists - you simply have to navigate to the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) for your list. The GO term enrichment for your list will be displayed as a widget \(see [What is a widget?](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#widgets)\). For more information on the enrichment calculation, see the [InterMine documentation](http://intermine.readthedocs.org/en/latest/embedding/list-widgets/enrichment-widgets/).

## Expression Data

### How do I find which tissues or developmental stages my gene\(s\) is/are expressed in?

For a single gene, the quickest way to view the available expression data is to look at the [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages) for that gene. Here you will find graphs showing the expression of the gene across development and the expression in adult fly tissues. In addition, tables showing _in situ_ mRNA expression data from BDGP and FlyFish are available.

For a list of genes, widgets \(graphs\) are available on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) showing expression in adult fly tissues \(FlyAtlas data\) and across development \(modENCODE RNA\_seq data, BDGP and FlyFish in situ hybridisation\).

### How do I find genes expressed ONLY in a particular tissue?

This is a three-step process:

1. Find and save the genes expressed in all tissues except the one you are interested in.

For this, you can use the template [Genes → Expression in a set of tissues](http://www.flymine.org/query/template.do?name=Gene_FlyAtlas_TissueList&scope=all). From the drop-down list of tissues select all tissues except the one you want to find the tissue-specific genes. The operator should be set to **ONE OF**:

Create a list of all the genes returned by your search \(If you are unsure how to save a list of genes see [Save a results set for further analysis](https://flymine.readthedocs.io/en/latest/results-tables/Documentationresultstables.html#makealist)\):

1. Find the genes expressed in the tissue you are interested in:

You can use the same template as above - just change the tissue selection to the one you are interested in. Again, save the set of genes returned by the search:

1. Find the genes expressed ONLY in the tissue you are interested in:

Now to find the genes that are expressed ONLY in the tissue you are interested in, you need to subtract the first list created above from the second list. To do this, navigate to the lists ‘view’ page. The two lists you have just created should be at the top of the list of lists. Select the two lists and then ‘Asymmetric Difference\` \(Note that you need to use Asymmetric difference rather than subtract - the icons on this page illustrate the difference between these two operations\). The Asymmetric difference provides options to subtract the lists either way - you need to select the single tissue list minus the all but one list - enter a name for your new list. The new list should appear at the top of the lists view page. In this example, as we are using the FlyAtlas data, we can check that we have created a tissue-specific expression set by looking at the FlyAtlas widget on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) for the list we have just created.

1. Similar searches.

The same workflow can of course be applied to finding other unique sets - for example, genes expressed only in a particular developmental stage. The template search [RNA\_seq → genes expressed in a set of tissues](http://www.flymine.org/query/template.do?name=modENCODE_RNA_seq_Tissues&scope=all) can be used to create various lists based on the modENCODE RNA\_seq data \(which includes a developmental stage, tissues and other conditions\).

