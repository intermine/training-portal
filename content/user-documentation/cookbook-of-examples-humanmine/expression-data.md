# Expression Data

### HumanMine tissue expression datasets

In HumanMine, we load several datasets that provide information about expression data in different tissues. These datasets use different experimental techniques and measurements, making it difficult to compare them directly, but we have specific queries and visualizations for each dataset. The table below summarises these datasets

| **Data Set** | Source | **Measurement type** |
| :--- | :--- | :--- |
| Affymetrix array  | Array express E-MTAB-62  | T-statistic, p-value, UP, DOWN, notDE |
| RNA-seq | Array Express Illumina body map E-MTAB-513 | FPKM |
| RNA-seq | GTEx | TPM |
| RNA-seq | Protein Atlas | TPM |
| Protein localisation \(Ab staining\) | Protein Atlas | High, medium, low, not detected |

There are a number of templates that allow querying of each data set independently, allowing you to identify genes expressed in a tissue or set of tissues OR allowing you to identify the tissues that a particular gene or list of genes are expressed in. Navigate to the template tab and filter for “expression” to see the full list of templates - all templates provide details of the specific data set.

To compare expressions between the different data sets, it is easiest to make use of the list operations. For example, if you want to find all genes expressed in the brain according to all the data sets - query each set independently, create a list of the genes at each step and then use either the list intersect \(to create a stringent, high confidence set\) or the list union \(to create a set of lower stringency which contains a gene even if it only shows expression in tissue x in one dataset\).

It is possible to identify genes expressed solely in one tissue \(i.e tissue-specific expression\). For data sets that provide only TPM or FPKM values, you will have to decide on your expression cut-off, while for the E-MTAB-62 and Protein atlas localisation data it is possible to make use of the cut-offs already applied to the data by filtering for UP \(E-MTAB-62\) or High and medium \(protein atlas localisation\).

### How do I find which tissues my genes are expressed in?

For a single gene, the quickest way to view the available expression data is to look at the [Report Pages](https://flymine.readthedocs.io/en/latest/report-pages/Documentationreportpages.html#reportpages) for that gene. Here you will find graphs showing the expression of the gene across development and the expression in adult fly tissues. In addition, tables showing _in situ_ mRNA expression data from BDGP and FlyFish are available.

For a list of genes, widgets \(graphs\) are available on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) showing expression in adult fly tissues \(FlyAtlas data\) and across development \(modENCODE RNA\_seq data, BDGP and FlyFish in situ hybridisation\).

### How do I find genes expressed in a particular tissue or at a certain developmental stage?

A number of template searches are available to analyse the various sources of expression data. Due to the widely variant nature of the different expression sources, it is generally necessary to search each one separately - for example data for expression over development is available from BDGP, FlyFish, the modENCODE RNA\_seq data and from the time course data published by Arbeitman et al. Although a template search is available to analyse the BDGP and FlyFish data together, the development stage ranges they used in their studies do not agree exactly.

The following templates searches specifically look for genes expressed at a particular developmental stage\(s\) or in a particular tissue\(s\):

[Tissue \[D. melanogaster\] → FlyAtlas data](http://www.flymine.org/query/template.do?name=Tissue_Flyatlas&scope=all) \(allows optional filtering on FlyAtlas values\)

[Microarray Time Course data from Arbeitman et al \(filter on stage and ratio\) → Genes \(D. melanogaster\)](http://www.flymine.org/query/template.do?name=TimeCourseData_Gene&scope=all).

[BDGP → Genes](http://www.flymine.org/query/template.do?name=BDGP_Gene&scope=all) \(searches for a specified expression term and developmental stage\).

[Stage \[D. melanogaster\] → FlyFish + BDGP in situ data](http://www.flymine.org/query/template.do?name=Stage_FlyFishBDGP&scope=all)

[FlyFish expression term + stage \[D. melanogaster\] → Genes](http://www.flymine.org/query/template.do?name=FlyFish_Genes&scope=all)

To see all template searches for expression data navigate to the [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) and filter the list for ‘expression’ using the drop-down filter menu \(see [Finding the template search that you want](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#filtertemplatesearches)\).

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

