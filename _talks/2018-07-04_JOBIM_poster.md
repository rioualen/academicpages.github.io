---
title: "Characterization of Escherichia coli K-12 regulatory networks by bioinformatics integration of high-throughput data."
collection: talks
type: "Poster"
permalink: /talks/2018-07-04_JOBIM_poster
venue: "19th Open Days in Biology, Computer Science and Mathematics (JOBIM)"
date: 2018-07-04
location: "Palais du Pharo, Marseille, France"
---

* [Poster](http://rioualen.github.io/files/2018-07-04_JOBIM_poster.pdf)
* [Official website of the event](https://jobim2018.sciencesconf.org/)
* [Proceedings](https://jobim2018.sciencesconf.org/data/pages/Book_JOBIM2018_V_4.pdf)

**Characterization of Escherichia coli K-12 regulatory networks by bioinformatics integration of high-throughput data**

*Claire Rioualen, Julio Collado-Vides, Jacques van Helden*

* *Technologies avancées pour le génome et la clinique (TAGC), INSERM U1090 , Aix-Marseille Université, Marseille F-13288, France* [website](https://tagc.univ-amu.fr/)
* *Computational Genomics Research program, Center for Genomics Sciences - UNAM, México* [website](http://www.ccg.unam.mx/)

**Background.** 
Gene regulation is essential to any living organism, whether in physiological conditions or in response to environmental stimuli, and involves a variety of mechanisms. One of the most common ones is the binding of transcription factors on specific sites of the DNA, called TFBS.  By interacting with the recruitment of the RNA polymerase complex, it can have an impact on the transcription of the surrounding genes, whether positive or negative.
Those mechanisms can be characterized by using Next-Generation Sequencing (NGS) technologies. ChIP-seq1,2 allows to characterize DNA binding locations of transcription factors (TFs) at a genomic scale, using a reference genome. RNA-seq technology, or whole transcriptome shotgun sequencing, allows to quantify transcription of all the genes in a given cell, and compare the levels of transcription between different conditions. 

**Problematics.**
Escherichia coli K-12 is a model organism particularly adapted to the study of gene regulation mechanisms, and its genome is already well characterized. A milestone in the study of regulatory mechanisms was the description of the Lac operon using this strain (Jacob and Monod, 1961). Its genome was one of the first to be entirely sequenced and published (Blattner et al., 1997). Extensive information about TFs, their binding sites, target genes and operons has been manually curated and indexed for more than 20 years in dedicated databases such as RegulonDB (Gama-Castro et al., 2016) and EcoCyc (Keseler et al., 2017). 
However, so far NGS technologies have barely been applied to E.coli K-12, nor bacteria at large, and no guidelines exist on how to analyse such data in prokaryotic organisms. Furthermore, the existing tools for NGS data analysis were mostly developed for eukaryotic genomes, which have different characteristics of genome size and organization. 

**Methods.**
We have developed Snakemake-based workflows (Koster et al., 2012) as part of the SnakeChunks project (Rioualen et al., submitted), in order to analyse ChIP-seq and RNA-seq data targeting the same TFs in E.coli K-12. The modular structure of the workflows allows to use a variety of tools and parameters for each step of the analyses. It can thus be used to perform benchmarking of the crucial steps that are the peak-calling and the detection of differentially expressed genes. It has been shown in human datasets that the choice of tools has a great impact on the results (Pepke et al., 2009; Bailey et al., 2013), and most tools were primarily designed for the analysis of eukaryotic data. No such work has been realized in bacteria so far. 
Once peak-calling and differential gene expression analysis are properly performed, a lot of information can be extracted or deduced from the resulting data. TFs are characterized by their binding sites (TFBS) and target genes. However, most of E.coli’s TFs are poorly characterized: about a hundred of them don’t have any known binding sites, and another hundred have between one and three TFBSs. By using ChIP-seq data, many new TFBSs can be annotated genome-wide. Furthermore, these TFBSs allow to build weight matrices and thus associate binding motifs to each TF. The localization of TFBSs also allows to infer hypotheses about potential target genes. This can be confirmed by integration of RNA-seq data and analysis of differential expression. However, the association of ChIP-seq peaks and differentially-expressed genes is not a straightforward process, and many factors can interfere with the regulation of a target gene by its TF (Myers et al., 2013). In such cases, performing motifs discovery can unravel interactions with other TFs, whether cooperative or competitive. Finally, RNA-seq data allows to identify new transcription units (TUs), and potentially identify new operons altogether. These TUs and operons can be associated with annotated TSSs, as well as predicted ones (Mendoza-Vargas et al., 2009; Thomason et al., 2015). 

**Results.**
Preliminary results were obtained by reanalyzing a dataset combining ChIP-seq and RNA-seq and aimed at characterizing the Fumarate and Nitrate reductase Regulatory (FNR) transcription factor genome-wide (Myers et al., 2013). The analysis of RNA-seq data revealed that the expression of 484 genes was impacted by the deletion of FNR, which is consistent with the fact that this TF regulates many essential processes such as anaerobic growth and acid resistance in E.coli. However, the exhaustive curation of previously published experiments targeting FNR, available in RegulonDB (Gama-Castro et al., 2016), revealed that about 75% of the discovered genes had not yet been identified as FNR target genes, and 12% of them were corroborated by the ChIP-seq data. This is the case for the leuLABCD operon, for instance, which is known mainly for encoding the enzymes responsible for the biosynthesis of leucine from valine. Despite not being listed as a target of FNR, its genes show a lower expression in the FNR mutant, suggesting that FNR could potentially regulate its expression. This hypothesis is enforced by the ChIP-seq profiles, since we can observe a clear peak upstream of the operon. This interpretation relying on the integrated results of SnakeChunks workflows is consistent with  Myers and colleagues’ observations. This work was submitted to Current Protocols in Bioinformatics (Rioualen et al., under reviewing).

**Perspectives.**
Until today, most knowledge of regulation in E.coli K-12 has been accumulated through low-throughput experiments, and has been manually curated in RegulonDB (Gama-Castro et al., 2016). High-throughput data hasn’t been integrated yet, and though there are few datasets available at the moment, the amount is growing exponentially, which is why developing modular and reproducible workflows for the analysis of such data is becoming a necessity. It will allow, in a near future, to perform automated biocuration of any newly published data.
The next goal of this project is to make these workflows and tools accessible to all researchers, whether bioinformaticians, experimentalists, or biocurators, and allow them to analyse their own data and customize their choice of tools and parameters.
The combination of these large-scale experiments allows to answer many questions on gene regulatory mechanisms, and further characterizing E.coli would help understand its amazing adaptability, as well as explain why certains strains are pathogenic.
[RegulonDB database](http://regulondb.ccg.unam.mx)




