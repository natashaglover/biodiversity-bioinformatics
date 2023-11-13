## Aim

Use the gene `NCDN` as a case example and investigate how to know about a gene's function.

## Learning outcomes

* What can we learn about `NCDN` function determination in Uniprot?
* What does `NCDN` Gene Onthology (GO) annotation tells us about its function?
* What can we deduce from `NCDN` gene expression in several species?

## Introduction

We will start the hands-on part of this course by focusing on a single gene as a case study. In this case, we will use the gene `NCDN` (neurochondrin).

## Check about `NCDN` in Uniprot

Go to [Uniprot](https://www.uniprot.org/) and find the **human** gene `NCDN` page (`NCDN_HUMAN`). There is a lot of information within a Uniprot's protein page; let's first focus on the function description.

!!! hint
    Leave all the different species gene pages open in tabs. We will come back to them!

**Questions:**

* **What can we learn from the description of the human `NCDN`'s function?**
* **How was this information annotated?**

??? done "Answer"


Now go to the **mouse** gene `NCDN` Uniprot page (`NCDN_MOUSE`).

**Questions:**

* **What can we learn from the description of the mouse `NCDN`'s function?**
* **How was this information annotated?**

??? done "Answer"


Try it again with the **bovin** gene (`NCDN_BOVIN`), the **drosophila** gene page (`NCDN_DROME`) and the **xenopus** gene page (`NCDN_XENLA`).

**Questions:**

* **What can we learn about Uniprot's gene function assessment?**
* **In which species is most of the research on `NCDN` done?**

??? done "Answer"


Two other ways to shed light into a gene's function are checking its subcellular localization and its sequence features (domains, variants…). We can find information on both of these aspects in Uniprot. First, focus on the subcellular location. There is one section dedicated to this in all Uniprot gene pages. Explore all the ones we opened before.

**Questions:**

* **Is `NCDN` subcellular location informative on its function?**
* **From where was each information retrieved?**

??? done "Answer"


Now try the same with the sequence features. There is a new `Feature viewer` in Uniprot gene pages. Explore it for all the species above.

**Questions:**

* **Is the `NCDN` sequence informative?**
* **Does it mean that retrieving information from a protein sequence is meaningless?**

??? done "Answer"


## Learn about `NCDN`'s Gene Ontology annotation

Now, we will focus on `NCDN`'s Gene Ontology (GO) annotation. There are many tools that use GO annotation in different ways. In this practical, we will use some of the most established ones.

First, still in the Uniprot gene pages. Go to the GO annotation section on each page. Compare the GO terms in which `NCDN` is annotated in each species and the sources of such annotations.

**Question: What can we learn on GO annotations in non-model species?**

Go to the [AmiGO 2 website](https://amigo.geneontology.org/amigo/landing), in the top menu, select `Search` and then `Genes and gene products`. Search for our `NCDN` gene.

**Questions:**

* **For which species do we have information? Why?**
* **How can we get GO annotations for other species?**

??? done "Answer"


Now you can go to each species AmiGO 2 `NCDN` pages. Explore them a bit.

**Question: From where do they retrieve the evidence for the GO annotations?**

??? done "Answer"


## Look at expression of `NCDN` for several species in Bgee

We are now going to utilize the Bgee database in order to retrieve expression related information on our target gene (`NCDN`). You can access the webpage of Bgee in your browser by following [this link](https://www.bgee.org/).

You will arrive at the Bgee homepage where you can access the various tools of Bgee in the top toolbar, directly search for a gene in the middle search box or download expression data for various animal species by clicking on the correct species picture in the bottom of the page. For this step, we will be interested in continuing to explore the function of `NCDN` orthologs, now focusing on their expression. To do this, you will just need to search for a gene name (`NCDN`), a UniProt or an Ensembl identifier.

<figure>
  <img src="../../../assets/images/day3/session1/gene_search.gif" align="center"/>
</figure>

Doing this, you will be directed to the gene search result page where you can see that there are 49 genes in Bgee for the gene name `NCDN`.

**Question: Why are there multiple Ensembl identifiers for one gene name (`NCDN`)?**

??? done "Answer"


In this page, you will notably find a column for `Gene identifier` that represents the unique Ensembl identifiers for each species or the species scientific and common name in the column `Organism`. To continue, please select a species (for example **mouse**) and click on their Ensembl ID ([ENSMUSG00000028833](https://www.bgee.org/gene/ENSMUSG00000028833/)). This will lead you to the mouse specific gene page for `NCDN`; don't worry you will still be able to see other orthologs of `NCDN`.

<figure>
  <img src="../../../assets/images/day3/session1/gene_search.jpg" align="center"/>
</figure>

On the left, you have the headers that allow you to jump easily to different sections of the page such as Expression or Orthologs. Since in this exercise we want to know where `NCDN` is expressed, we will primarily focus on the expression section for now.

<figure>
  <img src="../../../assets/images/day3/session1/expression_celltype.jpg" align="center">
</figure>

In this expression tab, you will find all anatomical entities where Bgee has evidence that this gene is expressed. You will notably find the expression score that denotes how strongly the gene was expressed in that tissue (from 0 to 100). If you want to verify the given information, you can also access the data used to determine expression in the link to source data column or see which type of data was used in source (such as R for bulk RNA-seq or A for Affymetrix microarray).

**Question: Looking at the top entries in the expression table, in which organ(s) do you think this gene is generally expressed?**

??? done "Answer"


We can also investigate if this gene is expressed at different stages of development. To do so, you can unselect `Anat. entity and cell types` and tick the `Dev. stage` box on top of the expression tab and update the results.

<figure>
  <img src="../../../assets/images/day3/session1/expression_devstage.jpg" align="center">
</figure>

Here, we see that this gene seems to be expressed in late adults as well as the embryonic stage (for example, `Theiler stage 04`). If you are unsure what a developmental stage term means, clicking on the identifier (_e.g._ `MmusDv:0000008`) will take you to the description of this term in the developmental ontology. Interestingly, in this case, looking at the `Reported absence of expression` section (below in the same page), we can see that there are no developmental stages where the gene is not expressed at all, even though its expression is much lower outside the brain.

<figure>
  <img src="../../../assets/images/day3/session1/gene_noexpression.jpg" align="center">
</figure>

**Questions:**

* **Go back to the `Expression` section and the `Anat. entity and cell types` filter. Where is `NCDN` the least expressed?**
* **Play around by combining the filters for sex, strain, developmental stage or anatomical entities, which insights can you gather?**

??? done "Answer"


By clicking on the `Orthologs` section in the menu on the left or scrolling down to it, you can find the different orthologs for NCDN which are found in Bgee. This information is retrieved from the OMA SPARQL endpoint that you used on the first day. Orthologs for NCDN are found at 11 different taxon levels. You can see the Ensembl identifiers of orthologous genes at specific taxon levels by clicking the `See details` arrow.

<figure>
  <img src="../../../assets/images/day3/session1/gene_orthologs.jpg" align="center">
</figure>

**Question: Which is the higher taxon in which you can find human orthologs of mouse `NCDN`?**

??? done "Answer"


Unfold the orthologs (`See details`) to find the human `NCDN`, and open its page in a new tab.

**Question: Does the function of `NCDN` seem to have been conserved between mouse and human? What about more distant species?**

??? done "Answer"


Now we are going to compare the expression of the different orthologs of `NCDN` for Xenopus, Human, mouse, rat, guinea pig and macaque.

First, gather the Ensembl identifiers for those genes by looking at the orthologs tab!

* Rat (`ENSRNOG00000011751`)
* Xenopus (`ENSXETG00000009669`)
* Human (`ENSG00000020129`)
* Mouse (`ENSMUSG00000028833`)
* Guinea pig (`ENSCPOG00000023962`)
* Macaque (`ENSMMUG00000019812`).

We will learn to use Bgee expression comparison tool in order to gain novel insights on `NCDN` anatomical expression. To do this, click on the Analysis section of the top toolbar of Bgee and then on Expression comparison.

<figure>
  <img src="../../../assets/images/day3/session1/expression_comparison_tool.gif" align="center">
</figure>

Fill the orthologs identifiers in the gene list, with one gene per line and click the search button to launch Bgee's expression comparison tool.

<figure>
  <img src="../../../assets/images/day3/session1/expression_comparison_list.jpg" align="center" width=500>
</figure>

You will obtain the following results:

<figure>
  <img src="../../../assets/images/day3/session1/expression_comparison_results.jpg" align="center">
</figure>

**Question: Looking at the max expression scores, do the results seem consistent with the anatomical localization of `NCDN` expression when looking at in individual species?**

??? done "Answer"


The conservation score represents the ratio between genes being called present in the tissue and the total number of genes. In our case since we only used orthologs, this value gives us the ratio between species which have `NCDN` expressed in that tissue divided by the total number of species for which we have data in that condition (maximum 6).

**Question: With the help of the conservation score, can you see for which species and tissue there is a qualitative difference in the expression of `NCDN`?**

??? done "Answer"
