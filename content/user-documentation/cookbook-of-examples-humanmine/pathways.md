# Pathways

### Where does the pathway data come from?

In FlyMine we load pathway data from both [Reactome](http://www.reactome.org/) and [KEGG](http://www.genome.jp/kegg/) . However, note that the KEGG data has not been updated since May 2011 due the current KEGG licensing requirement.

### How do I find which pathways my gene\(s\) is/are involved in?

Use the following template search:

[Gene → Pathway](http://www.flymine.org/query/template.do?name=Gene_Pathway&scope=alll)

### My gene is in pathway X, how can I find other genes involved in this pathway?

Use the following template search:

[Pathway → Genes](http://www.flymine.org/query/template.do?name=Pathway_Genes&scope=all)

### I am not sure of the exact name of the pathway, how can I find this?

Just start typing in the pathway name box - the type-ahead function will automatically show you matching pathways.

### Can I visualize this pathway data in InterMine?

We do not currently have any pathway visualization within FlyMine. However, linkouts enable you to view the pathways in either Reactome or Kegg.

### How do I find out if my genes or lists of genes have any pathways in common?

The underlying data model makes it possible to construct queries which effectively compare two lists for a specified attribute. Such a query is available as a template for comparing the pathways for two genes or two sets of genes. For two genes the query will return any pathways that are shared by the two genes. Similarly, if two lists are provided any pathways shared between any two genes in the lists are returned. The template is:

[Gene A → Pathways ← Gene B](http://www.flymine.org/query/template.do?name=ListPathway&scope=all)

