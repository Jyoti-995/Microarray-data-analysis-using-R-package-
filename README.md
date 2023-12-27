# Analysis of the Differential Gene and Protein Expression 
The present study is designed to study effects of AC electric fields on corneal epithelial cell gene and protein expression profiles in vitro.Gene Ontology results, following gene and protein array data analysis, showed that AC EFs influence similar biological processes that are predominantly responsive to organic substance, chemical, or external stimuli. Both arrays activate cytokine–cytokine receptor interaction, MAPK and IL-17 signaling pathways. Further, in comparison to the gene array data, the protein array data show enrichment of diverse activated signaling pathways through several interconnecting networks.

# Methods
1. Microarray Data Analysis: 
The data is analysed using R.Raw data underwent robust multichip algorithm (RMA) normalization using the "oligo" R package. The normalized data were utilized for heatmap and PCA plot generation. Differential expression analysis employed the "limma" R package, defining genes with adjusted p-values < 0.05 and |log2FC| > 2 as differentially expressed. GO and KEGG enrichment analysis utilized the "clusterProfiler" R package. Additionally, Transcriptome Analysis Console (TAC) software (v.4.0.1.36) and ShinyGO enrichment tool were employed for data analysis and graphical representation.

2. Antibody MicroarrayAanalysis:
Proteins were extracted, quantified, and labeled with fluorescent dyes for differential expression analysis. Using the LIMMA package in R-Bioconductor, we applied a specialized invariant Lowess method for normalization and employed a one-factorial linear model for sample analysis. Two-sided t-tests or F-tests based on moderated statistics were conducted, and p-values were adjusted for multiple testing using Benjamini and Hochberg's false discovery rate control. Proteins with |logFC| > 0.2 and adjusted p-value < 0.05 were considered differential. Log-fold changes (logFC) were presented on a basis of 2. A clustering heatmap and volcano plot depicted the calibrated samples and differentially expressed genes, respectively. Out of 21,448 genes analyzed, only 5.35% showed differential expression (556 upregulated, 591 downregulated) in hTCEpi cells stimulated with AC EFs compared to untreated control cells.

# Results
Hierarchical illustration of differentially expressed genes in hTCEpi cells after treatment with AC EFs for 24 h.
![image](https://github.com/Jyoti-995/Microarray-data-analysis-using-R-package-/assets/123369518/6813f597-2541-4dd8-aea0-971ae6a04e9d)

Expression level analysis was performed by using Robust Multi array-average(RMA) and log fold change values. 

![image](https://github.com/Jyoti-995/Microarray-data-analysis-using-R-package-/assets/123369518/072084a6-a9b1-4e51-8646-b796adf5aa07)

![image](https://github.com/Jyoti-995/Microarray-data-analysis-using-R-package-/assets/123369518/f6b03110-7bb1-49f5-94c7-29229ef721e4)






