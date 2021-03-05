# Expression Data

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

