# The paper title "A systemic glial reservoir of sympatho-adrenal lineage potential linked to neuroblastoma"

## Overview
We compared schwann cell precursors (SCPs) from wild-type and Sox10 heterozygous mice to investigate why the reduction of Sox10 gene dose enhances SCP-derived SA cell generation.

## Data
gz files are available in GEO, Accession number: GSE304632

## Requirements
OS: Windows 11

R version: 4.2.0 (We have not verified whether running this code with a different version of R reproduces the same results as those reported in the paper)

dplyr version 1.1.4, Seurat version 5.4.0, cowplot version 1.2.0, ggplot2 version 4.0.1, patchwork version 1.3.2, Biomanager version 3.22, SeuratWrappers version 0.3.0, monocle3 version 1.2.9

## Installation guide
You can install packages just running the codes. (e.g, install.packages(c("dplyr", "ggplot2", "patchwork", "cowplot"))). 5-10 min are required for installation.

## Demo
Please download the attached RDS file (sox10_cluster7.rds) and run the following code:

sox10_cluster7 <- readRDS("sox10_cluster7.rds")

DimPlot(sox10_cluster7)

The expected output is a plot with a shape similar to Fig. 4a (including an outlier).
The expected run time is within 1 minute. 

## Notes
In the code (e.g., saveRDS and readRDS), the "directory" indicates an arbitrary file path for saving or loading data; therefore, please modify it to your own desired directory.
Please also modify the gene names according to your interests (e.g., FeaturePlot).
