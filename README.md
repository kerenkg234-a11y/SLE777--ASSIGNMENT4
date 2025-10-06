# SLE777--ASSIGNMENT4
Repository for AT4

# Analysis of Age and Sex Signature in Human Muscle Tissue and Cell

This repository contains an RMarkdown workflow for analysis using RNA-seq data in humans. The analysis explores age and sex phenotypes across tissue and cell samples. Fastq files from this analysis are available at NCBI GEO (GSE287342). Data for time-course and differentiation score analysis is available at NCBI GEO (GSE168897).

# Features

Differential Expression Analysis: Conducted using DESeq2.

Principal Component Analysis (PCA): Visualization of sample variance using PCAtools.

Volcano Plots: Created with EnhancedVolcano to visualize significant genes.

Gene Set Enrichment Analysis (GSEA): Using mitch and msigdbr.

Differentiation Score Analysis: Performed to assess the differentiation status of samples.

Comprehensive Visualization: Includes PCA, volcano plots, heatmaps, and enrichment maps to support data interpretation.

# Repository Contents

1_DE_analysis.Rmd
Differential expression analysis script using DESeq2.
Generates Figures 1 to 3 and Supplementary Figure 1.

2_timeCourse.Rmd
Time-course analysis accounting for cell differentiation over time.
Generates Figure 4 and Supplementary Figures 2 and 3.

3_signatures.Rmd
Multi-comparison analysis used to extract age and sex gene signatures.
Generates Figures 5 and 6 and Supplementary Figures 5 and 6.

4_differentiationScore.Rmd
Calculates differentiation scores and assigns them to samples.
Generates Supplementary Figure 4 and Table 2.

functions.R
Contains custom utility functions used across scripts.

# Prerequisites

This project requires R (version 4.0 or higher) and the following R packages:

Core Packages:
prettydoc, tidyverse (includes dplyr and ggplot2), DESeq2, RUVSeq, PCAtools, EnhancedVolcano, ComplexHeatmap, knitr, mitch, msigdbr

Visualization and Plotting:
ggrepel, gplots, ggpubr, enrichplot, cowplot, RColorBrewer, circlize, viridis

Bioinformatics and Annotation:
RNAseqQC, clusterProfiler, DOSE, org.Hs.eg.db, DEGreport

# Workflow Overview

Import and quality check of count data and metadata.

Normalization and filtering using DESeq2 and RUVSeq.

Differential expression analysis for age and sex phenotypes.

Visualization of global variance (PCA) and significant genes (volcano plots).

Gene set enrichment analysis (GSEA) to explore biological significance.

Differentiation score calculation and visualization.

# Figures and Tables

Figures 1–6 and Supplementary Figures 1–6 are generated as part of the analysis.
Supplementary Table 2 contains differentiation score data.
All figures and tables can be reproduced by running the corresponding RMarkdown files.

# Authors

Developed by Keren Reji
