+++
title = "Chapter 0: Overview"
description = ""
weight = 1
+++
{{< lead >}}
This tutorial is for users who use Python to get information of a mine or an organism. This tutorial consists of **14** parts.

We use [FlyMine](https://www.flymine.org/flymine) as an example.

We recommend you to use **Jupyter Notebook** to run following code. If you are new to Jupyter, you can visit [this](https://jupyter.org/).
{{< /lead >}}
## Text Tutorial
input:

```
from intermine import registry
registry.getMines("D. melanogaster")
```
**getMines(organism)** fetches the mine(s) of a particular organism, say 'D. melanogaster'. Before running following modules, don't forget to run pip install intermine in your terminal first.

output: 
```
FawMine
FlyMine
LocustMine
XenMine
```


Now that we have the mines, we can use getInfo(mine) to fetch all the information about a particular mine ie its description, version, organisms associated etc. Suppose we want to know more about flymine, here's what we do:

input:
```
registry.getInfo("flymine")
```

output:
```
Description: An integrated database for Drosophila genomics
URL: http://www.flymine.org/flymine
API Version: 30
Release Version: 49 2020 February
InterMine Version: 4.1.3
Organisms: 
D. melanogaster
Neighbours: 
Animals
```


Now that we are very interested after viewing information about 'flymine', **getData(mine)** can be used to extract the data sets corresponding to it, the way is as follows:

input:
```
registry.getData("flymine")
```

output:
```
Name: Affymetrix array: GeneChip Drosophila Genome 2.0 Array
Name: Affymetrix array: GeneChip Drosophila Genome Array
Name: Alleles and phenotypes
Name: Artificial deletions
Name: BDGP cDNA clone data set
Name: BDGP in situ data set
Name: BioGRID interaction data set
Name: Disease Ontology
Name: Disease models
Name: Drosophila species orthologues and paralogues
Name: E-FLYC-6
Name: Fly Anatomy Ontology
Name: Fly Development Ontology
Name: FlyAtlas
Name: FlyBase Contolled Vocabulary
Name: FlyBase Controlled Vocabulary
Name: FlyBase PubMed to gene mapping
Name: FlyBase data set for Drosophila ananassae
Name: FlyBase data set for Drosophila erecta
Name: FlyBase data set for Drosophila grimshawi
Name: FlyBase data set for Drosophila melanogaster
Name: FlyBase data set for Drosophila mojavensis
Name: FlyBase data set for Drosophila persimilis
Name: FlyBase data set for Drosophila pseudoobscura pseudoobscura
Name: FlyBase data set for Drosophila sechellia
Name: FlyBase data set for Drosophila simulans
Name: FlyBase data set for Drosophila virilis
Name: FlyBase data set for Drosophila willistoni
Name: FlyBase data set for Drosophila yakuba
Name: FlyBase fasta data set for Drosophila ananassae
Name: FlyBase fasta data set for Drosophila melanogaster
Name: FlyBase fasta data set for Drosophila pseudoobscura pseudoobscura
Name: FlyBase fasta data set for Drosophila simulans
Name: FlyBase fasta data set for Drosophila virilis
Name: FlyMine intergenic regions
Name: GO
Name: GO Annotation data set
Name: GO Annotation for Drosophila melanogaster
Name: HGNC identifiers
Name: HomoloGene homology predictions
Name: Human gene identifiers
Name: INDAC long oligo data set
Name: IntAct molecular interactions
Name: InterPro data set
Name: InterPro domain GO annotations
Name: KEGG pathways data set
Name: Mouse gene identifiers
Name: Mouse identifiers
Name: NCBI Entrez Gene identifiers
Name: NCBI PubMed to gene mapping
Name: OMIM diseases
Name: PSI Molecular Interactions
Name: Panther orthologue and paralogue predictions
Name: PubMed to gene mapping
Name: REDfly Drosophila transcription factor binding sites
Name: REDfly Drosophila transcriptional cis-regulatory modules
Name: RNAi screen phenotypes
Name: Rat gene identifiers
Name: Reactome pathways data set
Name: Sequence Ontology
Name: Swiss-Prot data set
Name: The Gene Ontology
Name: The Sequence Ontology
Name: The developmental transcriptome of Drosophila melanogaster.
Name: TrEMBL data set
Name: TreeFam data set
Name: UniProt data set
Name: Uniprot data set
Name: WormBase gene identifiers
Name: Wormbase gene identifiers
Name: fly-Fish data set
Name: miRBase Targets
Name: microRNA Targets
```

## Video Tutorial
<br/>

<iframe width="560" height="315" src="https://www.youtube.com/embed/-PYJrPunlp0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


## Try Live
<br/>

You can try live [here](https://mybinder.org/v2/gh/intermine/intermine-ws-python-docs/master?filepath=unsolved-exercises%2F00-tutorial.ipynb).