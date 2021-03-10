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

1. query each set independently and create a list of genes at each step. 
2. Then 
   * Use the list intersection operation to create a stringent, high confidence set.
   * Or use the list union operation to create a set of lower stringency, which contains a gene even if it only shows expression in tissue x in one dataset.

It is possible to identify genes expressed solely in one tissue \(i.e. tissue-specific expression\). You will have to decide on your expression cut-off for datasets that provide only TPM or FPKM values. Simultaneously, for the E-MTAB-62 and Protein atlas localisation data, it is possible to make use of the cut-offs already applied to the data by filtering for UP \(E-MTAB-62\) or High and Medium \(protein atlas localisation\).

### How do I find which tissues my gene or list of genes are expressed in?

The easiest way to view the available expression data for a single gene is to look at the [Report Pages](../report-pages.md) for that gene. Gene report pages display graphs showing the expression of a particular gene in human tissues. For a list of genes, similar graphs are available on the [List analysis pages](../lists/list-analysis-pages.md). 

### How do I find genes expressed in a particular tissue?

Many template searches are available to analyse the various sources of expression data. These templates provide details of the specific dataset. However, due to the widely variant nature of the different expression sources, it is generally necessary to query any dataset independently to identify genes expressed in a tissue - or set of tissues - or identify the tissues that a particular gene or list of genes are expressed in. 

To view all template searches for expression data, you need to navigate to the [Templates](../template-search.md) tab and then filter the templates list by **“Expression”** using the **“Filter by category”** subtabs or the categories tags. 

```text
Place holder for a video (Expression Data 1)
```

### How do I find genes expressed ONLY in a particular tissue?

To accomplish this, you can use the [Tissue → Protein Atlas Expression](http://bluegenes-staging.apps.intermine.org/humanmine/templates/tissue_proteinatlas2) template, which returns a list of genes which are localised in a given human tissue. The template provide optional filters, such as the expression level and experimental confidence.

1. Use the drop-down list of tissues to select  the one you are interested in, such as Kidney. 
2. Click View Rows to view the results. 
3. You can now create a list of all the genes returned by your search, which should appear at the top of the [Lists view page](../lists/lists.md). If you are unsure how to save a list of genes, see [Save a result set for further analysis](https://app.gitbook.com/@user-documentation-intermine/s/user-documentation/content/user-documentation/results-tables#save-a-result-set-for-further-analysis). 

```text
Place holder for a video (Expression Data 2)
```

