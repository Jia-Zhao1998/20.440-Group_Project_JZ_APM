# 20.440 Group Project
## Defining the contribution of adipose resident tissue macrophages to adipogenesis
Time: Spring 2024
Members: Jia Zhao; Adriana Payan-Medina

## Overview

The repo contains the code and data to reproduce all figures and results for the group project of 20.440 Analysis of Biological Network (MIT)

Resident tissue macrophages (RTMs) are present ubiquitously in every tissue and organ, yet how they support tissue and organ function is largely unknown. Since intercellular communication is critical for tissue homeostasis, the goal is to use computational methods to unveil cell-cell communication between fat resident tissue macrophages, called vasculature-associated macrophages (VAMs), and other cell types to decode complex cellular circuits and infer novel functions of tissue-resident macrophages. The use of scRNA-seq analysis was also conducted to validate and investigate adipose RTM function. 

## Citation/Method

**NicheNet**: a computational algorithm to model intercellular communication

> install.packages("devtools")
> 
> devtools::install_github("saeyslab/nichenetr")

Git repo of NicheNet: https://github.com/saeyslab/nichenetr/tree/master

Browaeys, R.; Saelens, W.; Saeys, Y. NicheNet: Modeling Intercellular Communication by Linking Ligands to Target Genes. Nat. Methods 2020, 17 (2), 159–162. https://doi.org/10.1038/s41592-019-0667-5.

**DESeq2**: find differentially expressed genes and plot

Love, M.I., Huber, W., Anders, S. Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2 Genome Biology 15(12):550 (2014)

**Scanpy**: cluster and visualize cell types using marker genes, identify differentially expressed genes 

Wolf, F., Angerer, P. & Theis, F. SCANPY: large-scale single-cell gene expression data analysis. Genome Biol 19, 15 (2018). https://doi.org/10.1186/s13059-017-1382-0

**scikit-learn**: clustering cell types and subtypes

Scikit-learn: Machine Learning in Python, Pedregosa et al., JMLR 12, pp. 2825-2830, 2011.


## Data

**RNA-seq data of VAMs and other resident cells: Silva_WAT_cMAF_vs_WT.csv** 

Moura Silva Hernandez; Kitoko Jamil Zola; Queiroz Camila Pereira; Kroehling Lina; Matheis Fanny; Yang Katharine Lu; Reis Bernardo S.; Ren-Fielding Christine; Littman Dan R.; Bozza Marcelo Torres; Mucida Daniel; Lafaille Juan J. C-MAF–Dependent Perivascular Macrophages Regulate Diet-Induced Metabolic Syndrome. Sci. Immunol. 2021, 6 (64), eabg7506. https://doi.org/10.1126/sciimmunol.abg7506.


**A Single-Cell Atlas of Human and Mouse White Adipose Tissue**

Emont, M. P.; Jacobs, C.; Essene, A. L.; Pant, D.; Tenen, D.; Colleluori, G.; Di Vincenzo, A.; Jørgensen, A. M.; Dashti, H.; Stefek, A.; McGonagle, E.; Strobel, S.; Laber, S.; Agrawal, S.; Westcott, G. P.; Kar, A.; Veregge, M. L.; Gulko, A.; Srinivasan, H.; Kramer, Z.; De Filippis, E.; Merkel, E.; Ducie, J.; Boyd, C. G.; Gourash, W.; Courcoulas, A.; Lin, S. J.; Lee, B. T.; Morris, D.; Tobias, A.; Khera, A. V.; Claussnitzer, M.; Pers, T. H.; Giordano, A.; Ashenberg, O.; Regev, A.; Tsai, L. T.; Rosen, E. D. A Single-Cell Atlas of Human and Mouse White Adipose Tissue. Nature 2022, 603 (7903), 926–933. https://doi.org/10.1038/s41586-022-04518-2.

## Folder structure


We have subfolders in this repo

- data: the raw data of single-cell RNAseq of human and mouse white adipose tissue
  - scRNA_HWAT: subfolder with human WAT scRNA-seq UMAP results, metadata, features, and barcodes. The Matrix file referenced in 'A Single-Cell Atlas of Human and Mouse White Adipose Tissue' was locally stored due to its considerable size and the uploading constraints of GitHub. However, it is openly accessible via the provided link.
- code: source files for producing the results and figures
- figure: the final figures included in the submission 
- raw: Intermediate data files produced by the scripts. These files are not git committed.

## Installation

### NicheNet Analysis


R version 4.3.3

RStudio version: 2023.12.1.402

Packages: Relevant codes are in **code/NicheNet_VAMs.Rmd**

> install.packages("devtools")
> 
> devtools::install_github("saeyslab/nichenetr")
> 
> install.packages("tidyverse")
> 
> install.packages("DESeq2")
> 
> install.packages("EnhancedVolcano")

### scRNA-seq Analysis

Python version 3.11.5

 Jupyter Notebook version 7.1.3

 Packages: Relevant codes are in **code/scRNA_cluster_DGE.ipynb**

> import pandas
> 
> import sklearn.cluster
> 
> import scanpy
>
> import matplotlib.pyplot
> 
> import numpy
> 
> import os
