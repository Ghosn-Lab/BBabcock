# Batch Normalization Analyses
The analysis workflow is presented here in support of Babcock, et al. manuscript "Data Matrix Normalization and Merging Strategies Minimize
Batch-specific Systemic Variation in scRNA-Seq Data"

The preprint can be freely accessed at [bioRxiv](https://www.biorxiv.org/content/10.1101/2021.08.18.456898v1).

The complete analysis workflow used in this manuscript has been made available as an R notebook and included within this repository. Instructions for complete reproduction of the figures and data presented in the author's manuscript may be found within Batch_Workflow.Rmd. Some repetitive tasks in this workflow were stored for convenience as functions in the intial chunk of the notebook.

The workflow presented here begins with single-cell RNA-seq Digital Expression Matrices (DGEs), a matrix in the format of genes X barcodes, where values are UMI-demuxed transcript counts. DGEs may be generated from sequencing output (fastq) using any standard single-cell pre-processing workflow (we used [10X Cellranger V3](https://support.10xgenomics.com/single-cell-gene-expression/software/overview/welcome)).
