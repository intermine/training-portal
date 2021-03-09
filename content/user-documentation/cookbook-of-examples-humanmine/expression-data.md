# Expression Data

### HumanMine tissue expression datasets

In HumanMine, we load several datasets that provide information about expression data in different tissues. These datasets use different experimental techniques and measurements, making it difficult to compare them directly, but we have specific queries and visualizations for each dataset. The table below summarises these datasets.

| **Data Set** | Source | **Measurement type** |
| :--- | :--- | :--- |
| Affymetrix array  | Array express E-MTAB-62  | T-statistic, P-value, UP, DOWN, notDE |
| RNA-seq | Array Express Illumina body map E-MTAB-513 | FPKM |
| RNA-seq | GTEx | TPM |
| RNA-seq | Protein Atlas | TPM |
| Protein localisation \(Ab Staining\) | Protein Atlas | High, Medium, Low, Not detected. |

To compare expressions between different datasets, it is easier to make use of the list operations. For example, if you want to find all genes expressed in the brain according to all the datasets, you need to:

1. query each set independently and create a list of the genes at each step. 
2. Then 
   * Use the list intersection operation to create a stringent, high confidence set.
   * Or use the list union operation to create a set of lower stringency, which contains a gene even if it only shows expression in tissue x in one dataset.

It is possible to identify genes expressed solely in one tissue \(i.e. tissue-specific expression\). You will have to decide on your expression cut-off for datasets that provide only TPM or FPKM values. Simultaneously, for the E-MTAB-62 and Protein atlas localisation data, it is possible to make use of the cut-offs already applied to the data by filtering for UP \(E-MTAB-62\) or High and Medium \(protein atlas localisation\).

### How do I find which tissues my gene or list of genes are expressed in?

The easiest way to view the available expression data for a single gene is to look at the [Report Pages](../report-pages.md) for that gene. Gene report pages display graphs showing the expression of a particular gene in human tissues. For a list of genes, similar graphs are available on the [List analysis pages](../lists/list-analysis-pages.md). 

### How do I find genes expressed in a particular tissue?

Many template searches are available to analyse the various sources of expression data. All templates provide details of the specific datase. However, due to the widely variant nature of the different expression sources, it is generally necessary to query any dataset independently to identify genes expressed in a tissue - or set of tissues - or identify the tissues that a particular gene or list of genes are expressed in. 

To view the full list, you need to navigate to the Templates tab and then filter for “Expression” to see the full list of templates. 

For example, data for expression over development is available from BDGP, FlyFish, the modENCODE RNA\_seq data and from the time course data published by Arbeitman et al. Although a template search is available to analyse the BDGP and FlyFish data together, the development stage ranges they used in their studies do not agree exactly.

The following templates searches specifically look for genes expressed at a particular developmental stage\(s\) or in a particular tissue\(s\):

[Tissue \[D. melanogaster\] → FlyAtlas data](http://www.flymine.org/query/template.do?name=Tissue_Flyatlas&scope=all) \(allows optional filtering on FlyAtlas values\)

[Microarray Time Course data from Arbeitman et al \(filter on stage and ratio\) → Genes \(D. melanogaster\)](http://www.flymine.org/query/template.do?name=TimeCourseData_Gene&scope=all).

[BDGP → Genes](http://www.flymine.org/query/template.do?name=BDGP_Gene&scope=all) \(searches for a specified expression term and developmental stage\).

[Stage \[D. melanogaster\] → FlyFish + BDGP in situ data](http://www.flymine.org/query/template.do?name=Stage_FlyFishBDGP&scope=all)

[FlyFish expression term + stage \[D. melanogaster\] → Genes](http://www.flymine.org/query/template.do?name=FlyFish_Genes&scope=all)

To see all template searches for expression data, navigate to the [Template Searches](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#templatesearches) and filter the list for ‘expression’ using the drop-down filter menu \(see [Finding the template search that you want](https://flymine.readthedocs.io/en/latest/templates/Documentationtemplatesearches.html#filtertemplatesearches)\).

### How do I find genes expressed ONLY in a particular tissue?

This is a three-step process:

1. Find and save the genes expressed in all tissues except the one you are interested in.

For this, you can use the template [Genes → Expression in a set of tissues](http://www.flymine.org/query/template.do?name=Gene_FlyAtlas_TissueList&scope=all). From the drop-down list of tissues, select all tissues except the one you want to find the tissue-specific genes. The operator should be set to **ONE OF**:

Create a list of all the genes returned by your search \(If you are unsure how to save a list of genes, see [Save a result set for further analysis](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/content/user-documentation/results-tables#save-a-result-set-for-further-analysis)\):

1. Find the genes expressed in the tissue you are interested in:

You can use the same template as above - change the tissue selection to the one you are interested in. Again, save the set of genes returned by the search:

1. Find the genes expressed ONLY in the tissue you are interested in:

To find the genes that are expressed ONLY in the tissue you are interested in, you need to subtract the first list created above from the second list. To do this, navigate to the lists ‘view’ page. The two lists you have just created should be at the top of the list of lists. Select the two lists and then ‘Asymmetric Difference\` \(Note that you need to use Asymmetric difference rather than subtract - the icons on this page illustrate the difference between these two operations\). The Asymmetric difference provides options to subtract the lists either way - you need to select the single tissue list minus the all but one list - enter a name for your new list. The new list should appear at the top of the lists view page. In this example, as we are using the FlyAtlas data, we can check that we have created a tissue-specific expression set by looking at the FlyAtlas widget on the [List analysis pages](https://flymine.readthedocs.io/en/latest/lists/analysis/Documentationlistanalysispages.html#listanalysispage) for the list we have just created.

1. Similar searches.

The same workflow can be applied to finding other unique sets. For example, genes expressed only in a particular developmental stage. The template search [RNA\_seq → genes expressed in a set of tissues](http://www.flymine.org/query/template.do?name=modENCODE_RNA_seq_Tissues&scope=all) can be used to create various lists based on the modENCODE RNA\_seq data \(which includes a developmental stage, tissues and other conditions\).

