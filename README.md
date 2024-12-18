## Comprehensive-Unbiased-RNAseq-Database-Uncovers-New-Human-Monocyte-Derived-Macrophage-Subtypes

This repository contains scripts associated with the manuscript "Leveraging a comprehensive unbiased RNAseq database to characterize human monocyte-derived macrophage gene expression profiles within commonly employed in vitro polarization methods" published in Scientific Reports at: https://doi.org/10.1038/s41598-024-78000-6.

Supplemental Figures and Supplemental Files associated with this manuscript are available at: https://doi.org/10.15139/S3/I4EDM7.

Author: Timothy Smyth et al.

These scripts are presented in separate folders corresponding to specific analyses.

1. Data Setup
  - Downloading, sorting, and extracting raw count data of human monocyte-derived macrophage (MDM) samples from the ARCHS4 database.
2. Sample and Gene Selection
  - Genes are filtered using edgeR function filterByExpr and samples are filtered using dendrogram clustering.
3. Differential Expression
  - Differential expression analysis using limma-voom. Differential expression was performed comparing each polarization state (M0, M1, M2) or between each polarization method within single polarization states. 
  - Extraction and visualization of top canonical pathways as determined by Ingenuity Pathway Analysis (IPA).
4. Random Forest
  - Random forest modeling was conducted to classify M0, LPS, IFNy, and LPS+IFNy MDMs and to determine the key genes responsible for classification in the models.
5. Heatmaps
  - Principal component analysis (PCA) and heatmap generation with partition around medoid (PAM) clustering of the top 1000 genes as determined by random forest modeling.
6. GO and GSVA Analysis
  - Gene ontology biological process term enrichment of the top 1000 genes as determined by random forest modeling.
  - Gene set variation analysis (GSVA) of gene sets based on enriched GO terms.
