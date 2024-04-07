# 20.440 Group Project
Time: Spring 2024
Members: Jia Zhao; Adriana Payan-Medina

## Overview

The repo contains the code and data to reproduce one figure for the group project of 20.440 Analysis of Biological Network (MIT)

The goal is to use computational methods to unveil cell-cell communication between tissue resident macrophages and other cell types to decode complex cellular circuits and infer novel functions of tissue resident macrophages. 

## Citation/Method

**NicheNet**: a computational algorithm to model intercellular communication

> install.packages("devtools")
> 
> devtools::install_github("saeyslab/nichenetr")

Git repo of NicheNet: https://github.com/saeyslab/nichenetr/tree/master

Browaeys, R.; Saelens, W.; Saeys, Y. NicheNet: Modeling Intercellular Communication by Linking Ligands to Target Genes. Nat. Methods 2020, 17 (2), 159–162. https://doi.org/10.1038/s41592-019-0667-5.

## Data

At a high level, how was the data generated?

**A Single-Cell Atlas of Human and Mouse White Adipose Tissue**

Emont, M. P.; Jacobs, C.; Essene, A. L.; Pant, D.; Tenen, D.; Colleluori, G.; Di Vincenzo, A.; Jørgensen, A. M.; Dashti, H.; Stefek, A.; McGonagle, E.; Strobel, S.; Laber, S.; Agrawal, S.; Westcott, G. P.; Kar, A.; Veregge, M. L.; Gulko, A.; Srinivasan, H.; Kramer, Z.; De Filippis, E.; Merkel, E.; Ducie, J.; Boyd, C. G.; Gourash, W.; Courcoulas, A.; Lin, S. J.; Lee, B. T.; Morris, D.; Tobias, A.; Khera, A. V.; Claussnitzer, M.; Pers, T. H.; Giordano, A.; Ashenberg, O.; Regev, A.; Tsai, L. T.; Rosen, E. D. A Single-Cell Atlas of Human and Mouse White Adipose Tissue. Nature 2022, 603 (7903), 926–933. https://doi.org/10.1038/s41586-022-04518-2.

## Folder structure

At a high level, what is in each folder and subfolder?

I have subfolders in this repo

- data: the raw data of single cell RNAseq of human and mouse white adipose tissue
- code: source files for producing the figure
- figure: the final figure for PSET6
- raw: Intermediate data files produced by the scripts. These files are not git committed.

## Installation

How do I run your code? What software and package versions do I need to install?
