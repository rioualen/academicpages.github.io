---
title: "Interactome-regulome integrative approach for genome-wide screening data analysis in a breast cancer stem cells study"
collection: talks
type: "Talk"
permalink: /talks/2014-09-07_ECCB_Strasbourg_poster
venue: "13th European Conference on Computational Biology (ECCB)"
date: 2014-09-07
location: "Strasbourg, France"
---

 * [Poster](http://rioualen.github.io/files/2014-09-07_ECCB_Strasbourg_poster.pdf)
 * [Website of the event](https://www.ebi.ac.uk/eccb/2014/eccb14.loria.fr/home.html)
 * [Proceedings](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4147932/)

**Interactome-regulome integrative approach for genome-wide screening data analysis in a breast cancer stem cells study**

C Rioualen,  Q Da Costa, G Pinna,  A Harel-Bellan,  E Charafe-Jauffret, C Ginestier, G Bidaut

Centre de Recherche en Cancérologie de Marseille, Inserm U1068, CNRS UMR7258, Aix-Marseille Université, Institut Paoli-Calmettes, Marseille, 13009, France.
Plateforme ARN interference PArI, CEA SACLAY, Gif-sur-Yvette, France. 

Background. Breast cancer (BC) is the deadliest cancer in women worldwide. It is believed that cancer stem cells (CSC) could explain its recurrence, due to their resistance to conventional treatments and their ability to generate metastases. Identifying their key signaling pathways could be a lead for the development of new efficient treatments against BC.
Method. A genome-wide screening of an siRNA library was performed to evaluate the effect of single-gene knockdowns on CSC population (increase or decrease). 18,500 genes were scored accordingly.
In order to isolate CSC-regulating pathways, we applied a network-based integrative approach using a heavily modified version of the ITI algorithm (Interactome-Transcriptome Integration, Garcia et al 2012). ITI has been initially developed in order to perform gene-expression-based tumor classification, using cancer cells expression and a map of publicly available protein-protein interactions data.
In order to isolate pathways involved in CSC evolution, we decided to include two changes in ITI: first, we used scores from the screening instead of gene expression profiles. Second, we added a regulation map (regulome made of TF-target couples), using interactions from public databases. 
In this new algorithm, the interactome and the regulome are separately investigated, using target genes as “seeds”. If the seed's score is above a given threshold it is put aside. Its neighboring nodes are aggregated recursively if they improve the subnetwork's score, calculated by averaging screening scores of genes it contains. It is then statistically validated by comparing its score to those of subnetworks generated with randomized data. Interactome and regulome subnetworks are then merged. Resulting “metasubnetworks” are believed to be regulation pathways involved in CSC survival or death.
Results. Our method showed promising results by confirming the implication of genes that scored high hits in the primary screening. It also revealed the potential implication of unsuspected genes or TF. RUNX1, which was already described as a master regulator of leukemic stem cells, seems to regulate breast CSC. RBM14 revealed low-hit interacting mates, which showed Gene Ontology term “intracellular estrogen receptor signaling pathway” enrichment. NCOR1 was associated with the death of CSC, and the interactome-regulome integration showed proximity with PRDX1.
Conclusion. This new integrative approach yielded very promising results by both confirming in vitro experiments, and unraveling new genes of interest. This method could help scientists save time and money by potentially avoiding an expensive secondary screening, and ultimately allow us to identify new targets in cancer treatment. At the era of personalized medicine, elaborating a new drug targeting CSCs could greatly improve BC clinical outcome.

Poster available [here](http://rioualen.github.io/files/2014-09-07_ECCB_Strasbourg_poster.pdf)


