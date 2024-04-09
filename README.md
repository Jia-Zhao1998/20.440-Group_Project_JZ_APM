# 20.440 Group Project
Time: Spring 2024
Members: Jia Zhao; Adriana Payan-Medina

## Overview

The repo contains the code and data to reproduce one figure for the group project of 20.440 Analysis of Biological Network (MIT)

Tissue resident macrophages (TRMs) are present ubiquitously in every tissue and organ, yet how they support tissue and organ function is largely unknown. Since intercellular commnunication is critical for tissue homeostasis, the goal is to use computational methods to unveil cell-cell communication between fat tissue resident macrophages, called vasculature associated macrophages (VAMs), and other cell types to decode complex cellular circuits and infer novel functions of tissue resident macrophages. 

## Citation/Method

**NicheNet**: a computational algorithm to model intercellular communication

> install.packages("devtools")
> 
> devtools::install_github("saeyslab/nichenetr")

Git repo of NicheNet: https://github.com/saeyslab/nichenetr/tree/master

Browaeys, R.; Saelens, W.; Saeys, Y. NicheNet: Modeling Intercellular Communication by Linking Ligands to Target Genes. Nat. Methods 2020, 17 (2), 159–162. https://doi.org/10.1038/s41592-019-0667-5.

**DESeq2**: find differentially expressed genes and plot

Love, M.I., Huber, W., Anders, S. Moderated estimation of fold change and dispersion for RNA-seq data with DESeq2 Genome Biology 15(12):550 (2014)

## Data

**RNA-seq data of VAMs and other resident cells: Silva_WAT_cMAF_vs_WT.csv** 

Moura Silva Hernandez; Kitoko Jamil Zola; Queiroz Camila Pereira; Kroehling Lina; Matheis Fanny; Yang Katharine Lu; Reis Bernardo S.; Ren-Fielding Christine; Littman Dan R.; Bozza Marcelo Torres; Mucida Daniel; Lafaille Juan J. C-MAF–Dependent Perivascular Macrophages Regulate Diet-Induced Metabolic Syndrome. Sci. Immunol. 2021, 6 (64), eabg7506. https://doi.org/10.1126/sciimmunol.abg7506.![image](https://github.com/Jia-Zhao1998/JiaPSET6/assets/67213486/3a65aea6-b3d7-4e45-9b02-ee70328722ec)


**A Single-Cell Atlas of Human and Mouse White Adipose Tissue**

Emont, M. P.; Jacobs, C.; Essene, A. L.; Pant, D.; Tenen, D.; Colleluori, G.; Di Vincenzo, A.; Jørgensen, A. M.; Dashti, H.; Stefek, A.; McGonagle, E.; Strobel, S.; Laber, S.; Agrawal, S.; Westcott, G. P.; Kar, A.; Veregge, M. L.; Gulko, A.; Srinivasan, H.; Kramer, Z.; De Filippis, E.; Merkel, E.; Ducie, J.; Boyd, C. G.; Gourash, W.; Courcoulas, A.; Lin, S. J.; Lee, B. T.; Morris, D.; Tobias, A.; Khera, A. V.; Claussnitzer, M.; Pers, T. H.; Giordano, A.; Ashenberg, O.; Regev, A.; Tsai, L. T.; Rosen, E. D. A Single-Cell Atlas of Human and Mouse White Adipose Tissue. Nature 2022, 603 (7903), 926–933. https://doi.org/10.1038/s41586-022-04518-2.

## Folder structure


I have subfolders in this repo

- data: the raw data of single cell RNAseq of human and mouse white adipose tissue
- code: source files for producing the figure
- figure: the final figures
- raw: Intermediate data files produced by the scripts. These files are not git committed.

## Installation


R version 4.3.3

RStudio version: 2023.12.1.402

Packages: I included those relevant codes in **code/NicheNet_VAMs_PSET6.Rmd**

> install.packages("devtools")
> 
> devtools::install_github("saeyslab/nichenetr")
> 
> install.packages("tidyverse")
> 
> install.packages("DESeq2")
> 
> install.packages("EnhancedVolcano")
