## Data-analysis-of-LiP-MS-data-for-high-throughput-applications
This repository contains code and data accompanying the  **advanced LiP-MS protocol**, published in Nature Protocol.

## LiP-MS Data analysis and visualization

The main goal of LiP-MS data analysis is the identification of **proteins** that are **structurally altered** in the condition of interest; by comparing the samples, it is possible to find out which protein regions are involved in the alteration. We introduce [MSstatsLiP](https://www.bioconductor.org/packages/release/bioc/html/MSstatsLiP.html), an R package dedicated to the analysis of LiP-MS data for the identification of structurally altered peptides and differentially abundant proteins.

Before the structural analysis, a LiP-MS dataset is assessed using several **quality control (QC) measures**. Briefly, the peptide intensity distribution of each run, the coefficient of variation across biological replicates, the fraction of half-tryptic peptides in each replicate, as well as the number of identified proteins and peptides, are evaluated.

LiP-MS data analysis consists of **differential analysis of peptide intensities** between conditions, performed on the LiP samples.  Both **fully tryptic** and **half tryptic peptides** can be used. 

In this **new version of the LiP protocol**, the differential analysis is performed using **linear mixed models** that integrate all quantitative information across all conditions, which increases the sensitivity. Any contribution of **protein abundance change is corrected** using the tryptic samples. Proteins whose structures are significantly different between conditions are identified in a differential analysis of the LiP samples; LiP peptides that change their amounts between conditions are identified based on the statistical significance and the fold change of their intensity. Similarly, proteins whose abundances are significantly different in two conditions are identified in a differential analysis of the fully tryptic peptides of the TrP samples.  <br> 
 
In all LiP-MS experiments the distribution of altered peptides can be visualized in **volcano plots** and quantified using **bar diagrams**. We have recently introduced a new visualization of structural alteration of an individual protein, in which we map the intensity of the altered peptide(s) along the sequence of the protein and visualize protein coverage in addition, generating  [structural barcodes](https://www.cell.com/cell/fulltext/S0092-8674(20)31691-3?_returnURL=https%3A%2F%2Flinkinghub.elsevier.com%2Fretrieve%2Fpii%2FS0092867420316913%3Fshowall%3Dtrue). 

## What you will find in this repository

Here you can find the scripts for:<br>

 • **Case-control study**, where protein structural alterations and abundance changes are compared between two conditions <br><br>
 • **Multiple dose analysis**, where protein lysates are exposed to a compound dosage dilution series <br><br>
 •  **LiP-MS data exploration** (CV, correlation, dendrogram clustering, PCA) and **visualization** including **structural barcodes** <br><br>
 •  **Proteolytic resistance analysis**: proteolytic resistance is calculated as the ratio of the intensity of fully tryptic peptides in the LiP condition to the TrP condition and can be compared across different conditions  <br>
 
## Data availability
• Zenodo:  <br> 
• PRIDE:  <br>


## How to cite
