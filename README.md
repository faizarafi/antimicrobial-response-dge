# antimicrobial-response-dge
# Differential Gene Expression Analysis of Antibiotic-Treated *E. coli*

## Overview

This project involves a differential gene expression (DGE) analysis of *Escherichia coli* exposed to various antibiotics, aiming to identify genes and pathways involved in a potential universal antimicrobial stress response. The analysis was conducted entirely in R using RNA-seq raw count data from the Gene Expression Omnibus (series id: GSE215300). 

## Data:
This analysis utilizes a transcriptomic dataset of RNASeq counts of E. coli bacteria cells treated with antibiotics (GSE215300)3. The samples used in the dataset are E. coli (MG1655 strain) treated with no antibiotic (control), novobiocin (nov), rifampicin (Rif), or tetracycline (tet). The reads are obtained with these cultures using three library preparation methods: standard 5’ directional preparation, enrichment for VCE, or non-enrichment. Each sample has three biological replicates per combination of culture and library preparation methods, resulting in a total of 36 samples. The dataset has expression data of 4,464 genes for each sample.

## Methods

- **DESeq2** was used for normalization and differential expression analysis.
- **PCA** and **heatmaps** were generated to visualize sample clustering and differentially expressed genes.
- Gene ontology enrichment and Kegg pathway enrichment was performed to investigate functional categories affected by treatment.

## Repository Contents

- `dge_analysis.R`: R script for loading data, running DESeq2, and plotting
- `report_ecoli_transcriptomics.pdf`: Summary of results and methods (converted from `.Rmd` or `.docx`)

##  Dependencies

Key R packages:
- `DESeq2`
- `ggplot2`
- `pheatmap`
- `EnhancedVolcano` (optional)

